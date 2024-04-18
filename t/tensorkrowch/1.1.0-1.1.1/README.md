# Comparing `tmp/tensorkrowch-1.1.0.tar.gz` & `tmp/tensorkrowch-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorkrowch-1.1.0.tar", last modified: Sun Apr 14 00:29:11 2024, max compression
+gzip compressed data, was "tensorkrowch-1.1.1.tar", last modified: Thu Apr 18 22:43:14 2024, max compression
```

## Comparing `tensorkrowch-1.1.0.tar` & `tensorkrowch-1.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-04-14 00:29:11.506365 tensorkrowch-1.1.0/
--rw-rw-r--   0 jose      (1000) jose      (1000)     1086 2023-05-25 11:43:07.000000 tensorkrowch-1.1.0/LICENSE.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)       11 2024-03-06 17:59:45.000000 tensorkrowch-1.1.0/MANIFEST.in
--rw-r--r--   0 jose      (1000) jose      (1000)     8770 2024-04-14 00:29:11.506365 tensorkrowch-1.1.0/PKG-INFO
--rw-rw-r--   0 jose      (1000) jose      (1000)     6358 2024-04-14 00:27:40.000000 tensorkrowch-1.1.0/README.md
--rw-rw-r--   0 jose      (1000) jose      (1000)     1349 2024-04-14 00:06:08.000000 tensorkrowch-1.1.0/pyproject.toml
--rw-rw-r--   0 jose      (1000) jose      (1000)       38 2024-04-14 00:29:11.506365 tensorkrowch-1.1.0/setup.cfg
--rw-rw-r--   0 jose      (1000) jose      (1000)       38 2024-03-06 17:59:45.000000 tensorkrowch-1.1.0/setup.py
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-04-14 00:29:11.502365 tensorkrowch-1.1.0/tensorkrowch/
--rw-rw-r--   0 jose      (1000) jose      (1000)     1325 2024-04-14 00:27:40.000000 tensorkrowch-1.1.0/tensorkrowch/__init__.py
--rw-rw-r--   0 jose      (1000) jose      (1000)   197961 2024-04-14 00:06:08.000000 tensorkrowch-1.1.0/tensorkrowch/components.py
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-04-14 00:29:11.502365 tensorkrowch-1.1.0/tensorkrowch/decompositions/
--rw-rw-r--   0 jose      (1000) jose      (1000)       81 2024-04-14 00:28:38.000000 tensorkrowch-1.1.0/tensorkrowch/decompositions/__init__.py
--rw-rw-r--   0 jose      (1000) jose      (1000)     8830 2024-04-14 00:06:08.000000 tensorkrowch-1.1.0/tensorkrowch/decompositions/svd_decompositions.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    12476 2024-04-14 00:06:08.000000 tensorkrowch-1.1.0/tensorkrowch/embeddings.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    11806 2024-03-06 17:59:45.000000 tensorkrowch-1.1.0/tensorkrowch/initializers.py
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-04-14 00:29:11.502365 tensorkrowch-1.1.0/tensorkrowch/models/
--rw-rw-r--   0 jose      (1000) jose      (1000)      384 2024-04-14 00:06:08.000000 tensorkrowch-1.1.0/tensorkrowch/models/__init__.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    40695 2024-04-14 00:06:08.000000 tensorkrowch-1.1.0/tensorkrowch/models/mpo.py
--rw-rw-r--   0 jose      (1000) jose      (1000)   154694 2024-04-14 00:06:08.000000 tensorkrowch-1.1.0/tensorkrowch/models/mps.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    21219 2024-04-14 00:06:08.000000 tensorkrowch-1.1.0/tensorkrowch/models/mps_data.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    58350 2024-03-06 17:59:45.000000 tensorkrowch-1.1.0/tensorkrowch/models/peps.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    37360 2024-03-06 17:59:45.000000 tensorkrowch-1.1.0/tensorkrowch/models/tree.py
--rw-rw-r--   0 jose      (1000) jose      (1000)   160118 2024-04-14 00:06:08.000000 tensorkrowch-1.1.0/tensorkrowch/operations.py
--rw-rw-r--   0 jose      (1000) jose      (1000)     9156 2024-04-14 00:06:08.000000 tensorkrowch-1.1.0/tensorkrowch/utils.py
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-04-14 00:29:11.506365 tensorkrowch-1.1.0/tensorkrowch.egg-info/
--rw-r--r--   0 jose      (1000) jose      (1000)     8770 2024-04-14 00:29:11.000000 tensorkrowch-1.1.0/tensorkrowch.egg-info/PKG-INFO
--rw-rw-r--   0 jose      (1000) jose      (1000)      657 2024-04-14 00:29:11.000000 tensorkrowch-1.1.0/tensorkrowch.egg-info/SOURCES.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)        1 2024-04-14 00:29:11.000000 tensorkrowch-1.1.0/tensorkrowch.egg-info/dependency_links.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)      270 2024-04-14 00:29:11.000000 tensorkrowch-1.1.0/tensorkrowch.egg-info/requires.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)       13 2024-04-14 00:29:11.000000 tensorkrowch-1.1.0/tensorkrowch.egg-info/top_level.txt
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-04-18 22:43:14.802905 tensorkrowch-1.1.1/
+-rw-rw-r--   0 jose      (1000) jose      (1000)     1086 2023-05-25 11:43:07.000000 tensorkrowch-1.1.1/LICENSE.txt
+-rw-rw-r--   0 jose      (1000) jose      (1000)       11 2024-03-06 17:59:45.000000 tensorkrowch-1.1.1/MANIFEST.in
+-rw-r--r--   0 jose      (1000) jose      (1000)     8770 2024-04-18 22:43:14.802905 tensorkrowch-1.1.1/PKG-INFO
+-rw-rw-r--   0 jose      (1000) jose      (1000)     6358 2024-04-14 00:27:40.000000 tensorkrowch-1.1.1/README.md
+-rw-rw-r--   0 jose      (1000) jose      (1000)     1349 2024-04-14 00:06:08.000000 tensorkrowch-1.1.1/pyproject.toml
+-rw-rw-r--   0 jose      (1000) jose      (1000)       38 2024-04-18 22:43:14.802905 tensorkrowch-1.1.1/setup.cfg
+-rw-rw-r--   0 jose      (1000) jose      (1000)       38 2024-03-06 17:59:45.000000 tensorkrowch-1.1.1/setup.py
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-04-18 22:43:14.798905 tensorkrowch-1.1.1/tensorkrowch/
+-rw-rw-r--   0 jose      (1000) jose      (1000)     1382 2024-04-18 22:42:39.000000 tensorkrowch-1.1.1/tensorkrowch/__init__.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)   198461 2024-04-17 22:16:33.000000 tensorkrowch-1.1.1/tensorkrowch/components.py
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-04-18 22:43:14.798905 tensorkrowch-1.1.1/tensorkrowch/decompositions/
+-rw-rw-r--   0 jose      (1000) jose      (1000)       81 2024-04-14 00:28:38.000000 tensorkrowch-1.1.1/tensorkrowch/decompositions/__init__.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    10787 2024-04-14 08:34:34.000000 tensorkrowch-1.1.1/tensorkrowch/decompositions/svd_decompositions.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    13298 2024-04-17 18:24:11.000000 tensorkrowch-1.1.1/tensorkrowch/embeddings.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)     6401 2024-04-18 08:40:07.000000 tensorkrowch-1.1.1/tensorkrowch/initializers.py
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-04-18 22:43:14.798905 tensorkrowch-1.1.1/tensorkrowch/models/
+-rw-rw-r--   0 jose      (1000) jose      (1000)      384 2024-04-14 00:06:08.000000 tensorkrowch-1.1.1/tensorkrowch/models/__init__.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    50650 2024-04-18 20:01:59.000000 tensorkrowch-1.1.1/tensorkrowch/models/mpo.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)   174436 2024-04-18 22:39:56.000000 tensorkrowch-1.1.1/tensorkrowch/models/mps.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    21760 2024-04-14 08:41:17.000000 tensorkrowch-1.1.1/tensorkrowch/models/mps_data.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    58352 2024-04-18 22:38:24.000000 tensorkrowch-1.1.1/tensorkrowch/models/peps.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    37360 2024-03-06 17:59:45.000000 tensorkrowch-1.1.1/tensorkrowch/models/tree.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)   181888 2024-04-18 22:37:53.000000 tensorkrowch-1.1.1/tensorkrowch/operations.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)     9156 2024-04-14 00:06:08.000000 tensorkrowch-1.1.1/tensorkrowch/utils.py
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-04-18 22:43:14.798905 tensorkrowch-1.1.1/tensorkrowch.egg-info/
+-rw-r--r--   0 jose      (1000) jose      (1000)     8770 2024-04-18 22:43:14.000000 tensorkrowch-1.1.1/tensorkrowch.egg-info/PKG-INFO
+-rw-rw-r--   0 jose      (1000) jose      (1000)      657 2024-04-18 22:43:14.000000 tensorkrowch-1.1.1/tensorkrowch.egg-info/SOURCES.txt
+-rw-rw-r--   0 jose      (1000) jose      (1000)        1 2024-04-18 22:43:14.000000 tensorkrowch-1.1.1/tensorkrowch.egg-info/dependency_links.txt
+-rw-rw-r--   0 jose      (1000) jose      (1000)      270 2024-04-18 22:43:14.000000 tensorkrowch-1.1.1/tensorkrowch.egg-info/requires.txt
+-rw-rw-r--   0 jose      (1000) jose      (1000)       13 2024-04-18 22:43:14.000000 tensorkrowch-1.1.1/tensorkrowch.egg-info/top_level.txt
```

### Comparing `tensorkrowch-1.1.0/LICENSE.txt` & `tensorkrowch-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.1.0/PKG-INFO` & `tensorkrowch-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorkrowch
-Version: 1.1.0
+Version: 1.1.1
 Summary: Tensor Networks with PyTorch
 Author-email: José Ramón Pareja Monturiol <joserapa98@gmail.com>
 Maintainer-email: José Ramón Pareja Monturiol <joserapa98@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 José Ramón Pareja Monturiol
```

### Comparing `tensorkrowch-1.1.0/README.md` & `tensorkrowch-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.1.0/pyproject.toml` & `tensorkrowch-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.1.0/tensorkrowch/__init__.py` & `tensorkrowch-1.1.1/tensorkrowch/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 TensorKrowch
 ============
 
 Tensor Networks with PyTorch
 """
 
 # Version
-__version__ = '1.1.0'
+__version__ = '1.1.1'
 
 # Network components
 from tensorkrowch.components import Axis
 from tensorkrowch.components import AbstractNode, Node, ParamNode
 from tensorkrowch.components import StackNode, ParamStackNode
 from tensorkrowch.components import Edge, StackEdge
 from tensorkrowch.components import Successor, TensorNetwork
@@ -29,14 +29,15 @@
 from tensorkrowch.operations import (svd, svd_, svdr, svdr_, qr, qr_, rq, rq_,
                                      contract, contract_)
 
 # Node operations
 from tensorkrowch.operations import Operation
 from tensorkrowch.operations import get_shared_edges  # Not in docs
 
-from tensorkrowch.operations import permute, permute_, tprod, mul, add, sub
+from tensorkrowch.operations import (permute, permute_, tprod, mul, div, add,
+                                     sub, renormalize)
 from tensorkrowch.operations import (split, split_, contract_edges,
                                      contract_between, contract_between_,
                                      stack, unbind, einsum, stacked_einsum)
 
 # Models
 import tensorkrowch.models as models
```

### Comparing `tensorkrowch-1.1.0/tensorkrowch/components.py` & `tensorkrowch-1.1.1/tensorkrowch/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -810,14 +810,19 @@
         axis_num = self.get_axis_num(axis)
         return self._axes[axis_num]._node1
 
     def neighbours(self, axis: Optional[Ax] = None) -> Union[Optional['AbstractNode'],
                                                              List['AbstractNode']]:
         """
         Returns the neighbours of the node, the nodes to which it is connected.
+        
+        If ``self`` is a ``resultant`` node, this will return the neighbours of
+        the ``leaf`` nodes from which ``self`` inherits the edges. Therefore,
+        one cannot check if two ``resultant`` nodes are connected by looking
+        into their neighbours lists. To do that, use :meth:`is_connected_to`.
 
         Parameters
         ----------
         axis : int, str or Axis, optional
             Axis for which to retrieve the neighbour.
 
         Returns
@@ -1849,15 +1854,16 @@
                     axis_num.append(self.get_axis_num(ax))
             else:
                 axis_num.append(self.get_axis_num(axis))
         return self.tensor.std(dim=axis_num)
 
     def norm(self,
              p: Union[int, float] = 2,
-             axis: Optional[Union[Ax, Sequence[Ax]]] = None) -> Tensor:
+             axis: Optional[Union[Ax, Sequence[Ax]]] = None,
+             keepdim: bool = False) -> Tensor:
         """
         Returns the norm of all elements in the node's tensor. If an ``axis`` is
         specified, the norm is over that axis. If ``axis`` is a sequence of axes,
         reduce over all of them.
 
         This is not a node :class:`Operation`, hence it returns a ``torch.Tensor``
         instead of a :class:`Node`.
@@ -1866,14 +1872,17 @@
 
         Parameters
         ----------
         p : int, float
             The order of the norm.
         axis : int, str, Axis or list[int, str or Axis], optional
             Axis or sequence of axes over which to reduce.
+        keepdim : bool
+            Boolean indicating whether the output tensor have dimensions
+            retained or not.
 
         Returns
         -------
         torch.Tensor
         
         Examples
         --------
@@ -1891,15 +1900,15 @@
         axis_num = []
         if axis is not None:
             if isinstance(axis, (list, tuple)):
                 for ax in axis:
                     axis_num.append(self.get_axis_num(ax))
             else:
                 axis_num.append(self.get_axis_num(axis))
-        return self.tensor.norm(p=p, dim=axis_num)
+        return self.tensor.norm(p=p, dim=axis_num, keepdim=keepdim)
 
     def numel(self) -> Tensor:
         """
         Returns the total number of elements in the node's tensor.
 
         See also `torch.numel() <https://pytorch.org/docs/stable/generated/torch.numel.html>`_.
```

### Comparing `tensorkrowch-1.1.0/tensorkrowch/decompositions/svd_decompositions.py` & `tensorkrowch-1.1.1/tensorkrowch/decompositions/svd_decompositions.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 import torch
 
 
 def vec_to_mps(vec: torch.Tensor,
                n_batches: int = 0,
                rank: Optional[int] = None,
                cum_percentage: Optional[float] = None,
-               cutoff: Optional[float] = None) -> List[torch.Tensor]:
+               cutoff: Optional[float] = None,
+               renormalize: bool = False) -> List[torch.Tensor]:
     r"""
     Splits a vector into a sequence of MPS tensors via consecutive SVD
     decompositions. The resultant tensors can be used to instantiate a
     :class:`~tensorkrowch.models.MPS` with ``boundary = "obc"``.
     
     The number of resultant tensors and their respective physical dimensions
     depend on the shape of the input vector. That is, if one expects to recover
@@ -63,14 +64,22 @@
 
         .. math::
 
             \frac{\sum_{i \in \{kept\}}{s_i}}{\sum_{i \in \{all\}}{s_i}} \ge
             cum\_percentage
     cutoff : float, optional
         Quantity that lower bounds singular values in order to be kept.
+    renormalize : bool
+            Indicates whether nodes should be renormalized after SVD/QR
+            decompositions. If not, it may happen that the norm explodes as it
+            is being accumulated from all nodes. Renormalization aims to avoid
+            this undesired behavior by extracting the norm of each node on a
+            logarithmic scale after SVD/QR decompositions are computed. Finally,
+            the normalization factor is evenly distributed among all nodes of
+            the MPS.
 
     Returns
     -------
     List[torch.Tensor]
     """
     if not isinstance(vec, torch.Tensor):
         raise TypeError('`vec` should be torch.Tensor type')
@@ -78,72 +87,86 @@
     if n_batches > len(vec.shape):
         raise ValueError(
             '`n_batches` should be between 0 and the rank of `vec`')
     
     batches_shape = vec.shape[:n_batches]
     phys_dims = torch.tensor(vec.shape[n_batches:])
     
+    log_norm = 0
     prev_bond = 1
     tensors = []
     for i in range(len(phys_dims) - 1):
-        vec = vec.view(*batches_shape,
-                       prev_bond * phys_dims[i],
-                       phys_dims[(i + 1):].prod())
+        vec = vec.reshape(*batches_shape,
+                          prev_bond * phys_dims[i],
+                          phys_dims[(i + 1):].prod())
         
         u, s, vh = torch.linalg.svd(vec, full_matrices=False)
         
         lst_ranks = []
         
         if rank is None:
-            rank = s.shape[-1]
-            lst_ranks.append(rank)
+            aux_rank = s.shape[-1]
+            lst_ranks.append(aux_rank)
         else:
             lst_ranks.append(min(max(1, int(rank)), s.shape[-1]))
             
         if cum_percentage is not None:
             s_percentages = s.cumsum(-1) / \
                 (s.sum(-1, keepdim=True).expand(s.shape) + 1e-10) # To avoid having all 0's
             cum_percentage_tensor = cum_percentage * torch.ones_like(s)
             cp_rank = torch.lt(
                 s_percentages,
                 cum_percentage_tensor
-                ).view(-1, s.shape[-1]).all(dim=0).sum()
+                ).view(-1, s.shape[-1]).any(dim=0).sum()
             lst_ranks.append(max(1, cp_rank.item() + 1))
             
         if cutoff is not None:
             cutoff_tensor = cutoff * torch.ones_like(s)
             co_rank = torch.ge(
                 s,
                 cutoff_tensor
-                ).view(-1, s.shape[-1]).all(dim=0).sum()
+                ).view(-1, s.shape[-1]).any(dim=0).sum()
             lst_ranks.append(max(1, co_rank.item()))
         
         # Select rank from specified restrictions
-        rank = min(lst_ranks)
+        aux_rank = min(lst_ranks)
         
-        u = u[..., :rank]
+        u = u[..., :aux_rank]
         if i > 0:
-            u = u.reshape(*batches_shape, prev_bond, phys_dims[i], rank)
+            u = u.reshape(*batches_shape, prev_bond, phys_dims[i], aux_rank)
             
-        s = s[..., :rank]
-        vh = vh[..., :rank, :]
-        vh = torch.diag_embed(s) @ vh
+        s = s[..., :aux_rank]
+        vh = vh[..., :aux_rank, :]
+        
+        if renormalize:
+            aux_norm = s.norm(dim=-1, keepdim=True)
+            if not aux_norm.isinf().any() and (aux_norm > 0).any():
+                s = s / aux_norm
+                log_norm += aux_norm.log()
         
         tensors.append(u)
-        prev_bond = rank
+        prev_bond = aux_rank
         vec = torch.diag_embed(s) @ vh
         
     tensors.append(vec)
+    
+    if log_norm is not 0:
+        rescale = (log_norm / len(tensors)).exp()
+        for vec in tensors:
+            vec *= rescale.view(*vec.shape[:n_batches],
+                                *([1] * len(vec.shape[n_batches:])))
+    
     return tensors
 
 
 def mat_to_mpo(mat: torch.Tensor,
                rank: Optional[int] = None,
                cum_percentage: Optional[float] = None,
-               cutoff: Optional[float] = None) -> List[torch.Tensor]:
+               cutoff: Optional[float] = None,
+               renormalize: bool = False) -> List[torch.Tensor]:
     r"""
     Splits a matrix into a sequence of MPO tensors via consecutive SVD
     decompositions. The resultant tensors can be used to instantiate a
     :class:`~tensorkrowch.models.MPO` with ``boundary = "obc"``.
     
     The number of resultant tensors and their respective input/output dimensions
     depend on the shape of the input matrix. That is, if one expects to recover
@@ -175,77 +198,97 @@
 
         .. math::
 
             \frac{\sum_{i \in \{kept\}}{s_i}}{\sum_{i \in \{all\}}{s_i}} \ge
             cum\_percentage
     cutoff : float, optional
         Quantity that lower bounds singular values in order to be kept.
+    renormalize : bool
+            Indicates whether nodes should be renormalized after SVD/QR
+            decompositions. If not, it may happen that the norm explodes as it
+            is being accumulated from all nodes. Renormalization aims to avoid
+            this undesired behavior by extracting the norm of each node on a
+            logarithmic scale after SVD/QR decompositions are computed. Finally,
+            the normalization factor is evenly distributed among all nodes of
+            the MPS.
 
     Returns
     -------
     List[torch.Tensor]
     """
     if not isinstance(mat, torch.Tensor):
         raise TypeError('`mat` should be torch.Tensor type')
     if not len(mat.shape) % 2 == 0:
         raise ValueError('`mat` have an even number of dimensions')
     
     in_out_dims = torch.tensor(mat.shape)
     if len(in_out_dims) == 2:
         return [mat]
     
+    log_norm = 0
     prev_bond = 1
     tensors = []
     for i in range(0, len(in_out_dims) - 2, 2):
-        mat = mat.view(prev_bond * in_out_dims[i] * in_out_dims[i + 1],
-                       in_out_dims[(i + 2):].prod())
+        mat = mat.reshape(prev_bond * in_out_dims[i] * in_out_dims[i + 1],
+                          in_out_dims[(i + 2):].prod())
         
         u, s, vh = torch.linalg.svd(mat, full_matrices=False)
         
         lst_ranks = []
         
         if rank is None:
-            rank = s.shape[-1]
-            lst_ranks.append(rank)
+            aux_rank = s.shape[-1]
+            lst_ranks.append(aux_rank)
         else:
             lst_ranks.append(min(max(1, int(rank)), s.shape[-1]))
             
         if cum_percentage is not None:
             s_percentages = s.cumsum(-1) / \
                 (s.sum(-1, keepdim=True).expand(s.shape) + 1e-10) # To avoid having all 0's
             cum_percentage_tensor = cum_percentage * torch.ones_like(s)
             cp_rank = torch.lt(
                 s_percentages,
                 cum_percentage_tensor
-                ).view(-1, s.shape[-1]).all(dim=0).sum()
+                ).view(-1, s.shape[-1]).any(dim=0).sum()
             lst_ranks.append(max(1, cp_rank.item() + 1))
             
         if cutoff is not None:
             cutoff_tensor = cutoff * torch.ones_like(s)
             co_rank = torch.ge(
                 s,
                 cutoff_tensor
-                ).view(-1, s.shape[-1]).all(dim=0).sum()
+                ).view(-1, s.shape[-1]).any(dim=0).sum()
             lst_ranks.append(max(1, co_rank.item()))
         
         # Select rank from specified restrictions
-        rank = min(lst_ranks)
+        aux_rank = min(lst_ranks)
         
-        u = u[..., :rank]
+        u = u[..., :aux_rank]
         if i == 0:
-            u = u.reshape(in_out_dims[i], in_out_dims[i + 1], rank)
-            u = u.permute(0, 2, 1) # left x input x right
+            u = u.reshape(in_out_dims[i], in_out_dims[i + 1], aux_rank)
+            u = u.permute(0, 2, 1) # input x right x output
         else:
-            u = u.reshape(prev_bond, in_out_dims[i], in_out_dims[i + 1], rank)
+            u = u.reshape(prev_bond, in_out_dims[i], in_out_dims[i + 1], aux_rank)
             u = u.permute(0, 1, 3, 2) # left x input x right x output
             
-        s = s[..., :rank]
-        vh = vh[..., :rank, :]
-        vh = torch.diag_embed(s) @ vh
+        s = s[..., :aux_rank]
+        vh = vh[..., :aux_rank, :]
+        
+        if renormalize:
+            aux_norm = s.norm(dim=-1)
+            if not aux_norm.isinf() and (aux_norm > 0):
+                s = s / aux_norm
+                log_norm += aux_norm.log()
         
         tensors.append(u)
-        prev_bond = rank
+        prev_bond = aux_rank
         mat = torch.diag_embed(s) @ vh
     
-    mat = mat.reshape(rank, in_out_dims[-2], in_out_dims[-1])
+    mat = mat.reshape(aux_rank, in_out_dims[-2], in_out_dims[-1])
     tensors.append(mat)
+    
+    if renormalize:
+        rescale = (log_norm / len(tensors)).exp()
+        for mat in tensors:
+            mat *= rescale
+    
     return tensors
```

### Comparing `tensorkrowch-1.1.0/tensorkrowch/embeddings.py` & `tensorkrowch-1.1.1/tensorkrowch/embeddings.py`

 * *Files 4% similar despite different names*

```diff
@@ -319,14 +319,26 @@
             [1., 1., 0.],
             [1., 1., 1.]])
     
     >>> b = torch.rand(100, 5)
     >>> emb_b = tk.embeddings.discretize(b, level=3)
     >>> emb_b.shape
     torch.Size([100, 5, 3])
+    
+    To embed a data tensor with elements between 0 and 1 as basis vectors, one
+    can concatenate :func:`discretize` with :func:`basis`.
+    
+    >>> a = torch.rand(100, 10)
+    >>> emb_a = tk.embeddings.discretize(a, level=1, base=5)
+    >>> emb_a.shape
+    torch.Size([100, 10, 1])
+    
+    >>> emb_a = tk.embeddings.basis(emb_a.squeeze(2).int(), dim=5)
+    >>> emb_a.shape
+    torch.Size([100, 10, 5])
     """
     if not isinstance(data, torch.Tensor):
         raise TypeError('`data` should be torch.Tensor type')
     if not torch.ge(data, torch.zeros_like(data)).all():
         raise ValueError('Elements of `data` should be between 0 and 1')
     if not torch.le(data, torch.ones_like(data)).all():
         raise ValueError('Elements of `data` should be between 0 and 1')
@@ -408,14 +420,26 @@
             [0, 0, 0, 1, 0],
             [0, 0, 0, 0, 1]])
     
     >>> b = torch.randint(low=0, high=10, size=(100, 5))
     >>> emb_b = tk.embeddings.basis(b, dim=10)
     >>> emb_b.shape
     torch.Size([100, 5, 10])
+    
+    To embed a data tensor with elements between 0 and 1 as basis vectors, one
+    can concatenate :func:`discretize` with :func:`basis`.
+    
+    >>> a = torch.rand(100, 10)
+    >>> emb_a = tk.embeddings.discretize(a, level=1, base=5)
+    >>> emb_a.shape
+    torch.Size([100, 10, 1])
+    
+    >>> emb_a = tk.embeddings.basis(emb_a.squeeze(2).int(), dim=5)
+    >>> emb_a.shape
+    torch.Size([100, 10, 5])
     """
     if not isinstance(data, torch.Tensor):
         raise TypeError('`data` should be torch.Tensor type')
     if torch.is_floating_point(data):
         raise ValueError('`data` should be a tensor of integers')
     if not torch.ge(data, torch.zeros_like(data)).all():
         raise ValueError('Elements of `data` should be between 0 and (dim - 1)')
```

### Comparing `tensorkrowch-1.1.0/tensorkrowch/models/mpo.py` & `tensorkrowch-1.1.1/tensorkrowch/models/mpo.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,16 @@
         + UMPO
 """
 
 import warnings
 from typing import (List, Optional, Sequence,
                     Text, Tuple, Union)
 
+from math import sqrt
+
 import torch
 
 import tensorkrowch.operations as op
 from tensorkrowch.components import AbstractNode, Node, ParamNode
 from tensorkrowch.components import TensorNetwork
 from tensorkrowch.models import MPSData
 
@@ -407,41 +409,41 @@
             Initialization method.
         device : torch.device, optional
             Device where to initialize the tensors if ``init_method`` is provided.
         kwargs : float
             Keyword arguments for the different initialization methods. See
             :meth:`~tensorkrowch.AbstractNode.make_tensor`.
         """
-        if self._boundary == 'obc':
-            self._left_node.set_tensor(init_method='copy', device=device)
-            self._right_node.set_tensor(init_method='copy', device=device)
-
         if tensors is not None:
             if len(tensors) != self._n_features:
                 raise ValueError('`tensors` should be a sequence of `n_features`'
                                  ' elements')
             
             if self._boundary == 'obc':
                 tensors = tensors[:]
+                
+                if device is None:
+                    device = tensors[0].device
+                
                 if len(tensors) == 1:
                     tensors[0] = tensors[0].reshape(1,
                                                     tensors[0].shape[0],
                                                     1,
                                                     tensors[0].shape[1])
                     
                 else:
                     # Left node
                     aux_tensor = torch.zeros(*self._mats_env[0].shape,
-                                             device=tensors[0].device)
+                                             device=device)
                     aux_tensor[0] = tensors[0]
                     tensors[0] = aux_tensor
                     
                     # Right node
                     aux_tensor = torch.zeros(*self._mats_env[-1].shape,
-                                             device=tensors[-1].device)
+                                             device=device)
                     aux_tensor[..., 0, :] = tensors[-1]
                     tensors[-1] = aux_tensor
                 
             for tensor, node in zip(tensors, self._mats_env):
                 node.tensor = tensor
                 
         elif init_method is not None:
@@ -456,14 +458,18 @@
                     if i == 0:
                         # Left node
                         aux_tensor[0] = node.tensor[0]
                     elif i == (self._n_features - 1):
                         # Right node
                         aux_tensor[..., 0, :] = node.tensor[..., 0, :]
                     node.tensor = aux_tensor
+        
+        if self._boundary == 'obc':
+            self._left_node.set_tensor(init_method='copy', device=device)
+            self._right_node.set_tensor(init_method='copy', device=device)
     
     def set_data_nodes(self) -> None:
         """
         Creates ``data`` nodes and connects each of them to the ``"input"``
         edge of each node.
         """      
         input_edges = [node['input'] for node in self._mats_env]
@@ -539,63 +545,80 @@
         if net._boundary == 'obc':
             net._left_node = net._left_node.parameterize(set_param)
             net._right_node = net._right_node.parameterize(set_param)
             
         return net
     
     def _input_contraction(self,
-                           nodes_env: List[Node],
+                           nodes_env: List[AbstractNode],
+                           input_nodes: List[AbstractNode],
                            inline_input: bool = False) -> Tuple[
                                                        Optional[List[Node]],
                                                        Optional[List[Node]]]:
         """Contracts input data nodes with MPO nodes."""
         if inline_input:
-            mats_result = [node['input'].contract() for node in nodes_env]
+            mats_result = [
+                in_node @ node
+                for node, in_node in zip(nodes_env, input_nodes)
+                ]
             return mats_result
 
         else:
             if nodes_env:
                 stack = op.stack(nodes_env)
-                stack_data = op.stack(
-                    [node.neighbours('input') for node in nodes_env])
+                stack_data = op.stack(input_nodes)
 
                 stack ^ stack_data
 
                 result = stack_data @ stack
                 mats_result = op.unbind(result)
                 return mats_result
             else:
                 return []
 
     @staticmethod
-    def _inline_contraction(nodes: List[Node]) -> Node:
+    def _inline_contraction(mats_env: List[AbstractNode],
+                            renormalize: bool = False) -> Node:
         """Contracts sequence of MPO nodes (matrices) inline."""
-        result_node = nodes[0]
-        for node in nodes[1:]:
+        result_node = mats_env[0]
+        for node in mats_env[1:]:
             result_node @= node
+            
+            if renormalize:
+                right_axes = []
+                for ax_name in result_node.axes_names:
+                    if 'right' in ax_name:
+                        right_axes.append(ax_name)
+                if right_axes:
+                    result_node = result_node.renormalize(axis=right_axes)
+            
         return result_node
 
     def _contract_envs_inline(self,
-                              mats_env: List[Node],
+                              mats_env: List[AbstractNode],
+                              renormalize: bool = False,
                               mps: Optional[MPSData] = None) -> Node:
         """Contracts nodes environments inline."""
         if (mps is not None) and (mps._boundary == 'obc'):
             mats_env[0] = mps._left_node @ mats_env[0]
             mats_env[-1] = mats_env[-1] @ mps._right_node
         
         if self._boundary == 'obc':
             mats_env = [self._left_node] + mats_env
             mats_env = mats_env + [self._right_node]
-        return self._inline_contraction(mats_env)
+        return self._inline_contraction(mats_env=mats_env,
+                                        renormalize=renormalize)
 
-    def _aux_pairwise(self, nodes: List[Node]) -> Tuple[List[Node],
+    def _aux_pairwise(self,
+                      mats_env: List[AbstractNode],
+                      renormalize: bool = False) -> Tuple[List[Node],
     List[Node]]:
         """Contracts a sequence of MPO nodes (matrices) pairwise."""
-        length = len(nodes)
-        aux_nodes = nodes
+        length = len(mats_env)
+        aux_nodes = mats_env
         if length > 1:
             half_length = length // 2
             nice_length = 2 * half_length
 
             even_nodes = aux_nodes[0:nice_length:2]
             odd_nodes = aux_nodes[1:nice_length:2]
             leftover = aux_nodes[nice_length:]
@@ -603,40 +626,56 @@
             stack1 = op.stack(even_nodes)
             stack2 = op.stack(odd_nodes)
 
             stack1 ^ stack2
 
             aux_nodes = stack1 @ stack2
             aux_nodes = op.unbind(aux_nodes)
+            
+            if renormalize:
+                for i in range(len(aux_nodes)):
+                    axes = []
+                    for ax_name in aux_nodes[i].axes_names:
+                        if ('left' in ax_name) or ('right' in ax_name):
+                            axes.append(ax_name)
+                    if axes:
+                        aux_nodes[i] = aux_nodes[i].renormalize(axis=axes)
 
             return aux_nodes, leftover
-        return nodes, []
+        return mats_env, []
 
     def _pairwise_contraction(self,
-                              mats_nodes: List[Node],
-                              mps: Optional[MPSData] = None) -> Node:
+                              mats_env: List[Node],
+                              mps: Optional[MPSData] = None,
+                              renormalize: bool = False) -> Node:
         """Contracts nodes environments pairwise."""
-        length = len(mats_nodes)
-        aux_nodes = mats_nodes
+        length = len(mats_env)
+        aux_nodes = mats_env
         if length > 1:
             leftovers = []
             while length > 1:
-                aux1, aux2 = self._aux_pairwise(aux_nodes)
+                aux1, aux2 = self._aux_pairwise(mats_env=aux_nodes,
+                                                renormalize=renormalize)
                 aux_nodes = aux1
                 leftovers = aux2 + leftovers
                 length = len(aux1)
 
             aux_nodes = aux_nodes + leftovers
-            return self._pairwise_contraction(aux_nodes, mps)
-
-        return self._contract_envs_inline(aux_nodes, mps)
+            return self._pairwise_contraction(mats_env=aux_nodes,
+                                              renormalize=renormalize,
+                                              mps=mps)
+
+        return self._contract_envs_inline(mats_env=aux_nodes,
+                                          renormalize=renormalize,
+                                          mps=mps)
     
     def contract(self,
                  inline_input: bool = False,
                  inline_mats: bool = False,
+                 renormalize: bool = False,
                  mps: Optional[MPSData] = None) -> Node:
         """
         Contracts the whole MPO with input data nodes. The input can be in the
         form of an :class:`MPSData`, which may be convenient for tensorizing
         vector-matrix multiplication in the form of MPS-MPO contraction.
         
         If the ``MPO`` is contracted with a ``MPSData``, MPS nodes will become
@@ -670,14 +709,22 @@
             Boolean indicating whether input ``data`` nodes should be contracted
             with the ``MPO`` nodes inline (one contraction at a time) or in a
             single stacked contraction.
         inline_mats : bool
             Boolean indicating whether the sequence of matrices (resultant
             after contracting the input ``data`` nodes) should be contracted
             inline or as a sequence of pairwise stacked contrations.
+        renormalize : bool
+            Indicates whether nodes should be renormalized after contraction.
+            If not, it may happen that the norm explodes or vanishes, as it
+            is being accumulated from all nodes. Renormalization aims to avoid
+            this undesired behavior by extracting the norm of each node on a
+            logarithmic scale. The renormalization only occurs when multiplying
+            sequences of matrices, once the `input` contractions have been
+            already performed, including contracting against ``MPSData``.
         mps : MPSData, optional
             MPS that is to be contracted with the MPO. New data can be
             put into the MPS via :meth:`MPSData.add_data`, and the MPS-MPO
             contraction is performed by calling ``mpo(mps=mps_data)``, without
             passing the input data again, as it is already stored in the MPS
             cores.
 
@@ -695,20 +742,27 @@
             # Move MPSData ndoes to self
             mps._mats_env[0].move_to_network(self)
             
             # Connect mps nodes to mpo nodes
             for mps_node, mpo_node in zip(mps._mats_env, self._mats_env):
                 mps_node['feature'] ^ mpo_node['input']
                 
-        mats_env = self._input_contraction(self._mats_env, inline_input)
+        mats_env = self._input_contraction(
+            nodes_env=self._mats_env,
+            input_nodes=[node.neighbours('input') for node in self._mats_env],
+            inline_input=inline_input)
         
         if inline_mats:
-            result = self._contract_envs_inline(mats_env, mps)
+            result = self._contract_envs_inline(mats_env=mats_env,
+                                                renormalize=renormalize,
+                                                mps=mps)
         else:
-            result = self._pairwise_contraction(mats_env, mps)
+            result = self._pairwise_contraction(mats_env=mats_env,
+                                                renormalize=renormalize,
+                                                mps=mps)
             
         # Contract periodic edge
         if result.is_connected_to(result):
             result @= result
         
         # Put batch edges in first positions
         batch_edges = []
@@ -720,14 +774,179 @@
                 other_edges.append(i)
         
         all_edges = batch_edges + other_edges
         if all_edges != list(range(len(all_edges))):
             result = op.permute(result, tuple(all_edges))
         
         return result
+    
+    @torch.no_grad()
+    def canonicalize(self,
+                     oc: Optional[int] = None,
+                     mode: Text = 'svd',
+                     rank: Optional[int] = None,
+                     cum_percentage: Optional[float] = None,
+                     cutoff: Optional[float] = None,
+                     renormalize: bool = False) -> None:
+        r"""
+        Turns MPO into `canonical` form via local SVD/QR decompositions in the
+        same way this transformation is applied to :class:`~tensorkrowch.models.MPS`.
+        
+        To specify the new bond dimensions, the arguments ``rank``,
+        ``cum_percentage`` or ``cutoff`` can be specified. These will be used
+        equally for all SVD computations.
+        
+        If none of them are specified, the bond dimensions won't be modified
+        if possible. Only when the bond dimension is bigger than the physical
+        dimension multiplied by the other bond dimension of the node, it will
+        be cropped to that size.
+        
+        Parameters
+        ----------
+        oc : int
+            Position of the orthogonality center. It should be between 0 and 
+            ``n_features - 1``.
+        mode : {"svd", "svdr", "qr"}
+            Indicates which decomposition should be used to split a node after
+            contracting it. See more at :func:`~tensorkrowch.svd_`,
+            :func:`~tensorkrowch.svdr_`, :func:`~tensorkrowch.qr_`.
+            If mode is "qr", operation :func:`~tensorkrowch.qr_` will be
+            performed on nodes at the left of the output node, whilst operation
+            :func:`~tensorkrowch.rq_` will be used for nodes at the right.
+        rank : int, optional
+            Number of singular values to keep.
+        cum_percentage : float, optional
+            Proportion that should be satisfied between the sum of all singular
+            values kept and the total sum of all singular values.
+            
+            .. math::
+            
+                \frac{\sum_{i \in \{kept\}}{s_i}}{\sum_{i \in \{all\}}{s_i}} \ge
+                cum\_percentage
+        cutoff : float, optional
+            Quantity that lower bounds singular values in order to be kept.
+        renormalize : bool
+            Indicates whether nodes should be renormalized after SVD/QR
+            decompositions. If not, it may happen that the norm explodes as it
+            is being accumulated from all nodes. Renormalization aims to avoid
+            this undesired behavior by extracting the norm of each node on a
+            logarithmic scale after SVD/QR decompositions are computed. Finally,
+            the normalization factor is evenly distributed among all nodes of
+            the MPO.
+            
+        Examples
+        --------
+        >>> mpo = tk.models.MPO(n_features=4,
+        ...                     in_dim=2,
+        ...                     out_dim=2,
+        ...                     bond_dim=5)
+        >>> mpo.canonicalize(rank=3)
+        >>> mpo.bond_dim
+        [3, 3, 3]
+        """
+        self.reset()
+
+        prev_auto_stack = self._auto_stack
+        self.auto_stack = False
+
+        if oc is None:
+            oc = self._n_features - 1
+        elif (oc < 0) or (oc >= self._n_features):
+            raise ValueError('Orthogonality center position `oc` should be '
+                             'between 0 and `n_features` - 1')
+        
+        log_norm = 0
+        
+        nodes = self._mats_env[:]
+        if self._boundary == 'obc':
+            nodes[0].tensor[1:] = torch.zeros_like(
+                nodes[0].tensor[1:])
+            nodes[-1].tensor[..., 1:, :] = torch.zeros_like(
+                nodes[-1].tensor[..., 1:, :])
+        
+        # If mode is svd or svr and none of the args is provided, the ranks are
+        # kept as they were originally
+        keep_rank = False
+        if (rank is None) and (cum_percentage is None) and (cutoff is None):
+            keep_rank = True
+        
+        for i in range(oc):
+            if mode == 'svd':
+                result1, result2 = nodes[i]['right'].svd_(
+                    side='right',
+                    rank=nodes[i]['right'].size() if keep_rank else rank,
+                    cum_percentage=cum_percentage,
+                    cutoff=cutoff)
+            elif mode == 'svdr':
+                result1, result2 = nodes[i]['right'].svdr_(
+                    side='right',
+                    rank=nodes[i]['right'].size() if keep_rank else rank,
+                    cum_percentage=cum_percentage,
+                    cutoff=cutoff)
+            elif mode == 'qr':
+                result1, result2 = nodes[i]['right'].qr_()
+            else:
+                raise ValueError('`mode` can only be "svd", "svdr" or "qr"')
+            
+            if renormalize:
+                aux_norm = result2.norm() / sqrt(result2.shape[0])
+                if not aux_norm.isinf() and (aux_norm > 0):
+                    result2.tensor = result2.tensor / aux_norm
+                    log_norm += aux_norm.log()
+
+            result1 = result1.parameterize()
+            nodes[i] = result1
+            nodes[i + 1] = result2
+
+        for i in range(len(nodes) - 1, oc, -1):
+            if mode == 'svd':
+                result1, result2 = nodes[i]['left'].svd_(
+                    side='left',
+                    rank=nodes[i]['left'].size() if keep_rank else rank,
+                    cum_percentage=cum_percentage,
+                    cutoff=cutoff)
+            elif mode == 'svdr':
+                result1, result2 = nodes[i]['left'].svdr_(
+                    side='left',
+                    rank=nodes[i]['left'].size() if keep_rank else rank,
+                    cum_percentage=cum_percentage,
+                    cutoff=cutoff)
+            elif mode == 'qr':
+                result1, result2 = nodes[i]['left'].rq_()
+            else:
+                raise ValueError('`mode` can only be "svd", "svdr" or "qr"')
+            
+            if renormalize:
+                aux_norm = result1.norm() / sqrt(result1.shape[0])
+                if not aux_norm.isinf() and (aux_norm > 0):
+                    result1.tensor = result1.tensor / aux_norm
+                    log_norm += aux_norm.log()
+
+            result2 = result2.parameterize()
+            nodes[i] = result2
+            nodes[i - 1] = result1
+
+        nodes[oc] = nodes[oc].parameterize()
+        
+        # Rescale
+        if log_norm != 0:
+            rescale = (log_norm / len(nodes)).exp()
+        
+        if renormalize and (log_norm != 0):
+            for node in nodes:
+                node.tensor = node.tensor * rescale
+        
+        # Update variables
+        if self._boundary == 'obc':
+            self._bond_dim = [node['right'].size() for node in nodes[:-1]]
+        else:
+            self._bond_dim = [node['right'].size() for node in nodes]
+        self._mats_env = nodes
+
+        self.auto_stack = prev_auto_stack
 
 
 class UMPO(MPO):  # MARK: UMPO
     """
     Class for Uniform (translationally invariant) Matrix Product Operators. It is
     the uniform version of :class:`MPO`, that is, all nodes share the same
     tensor. Thus this class cannot have different input/output or bond dimensions
@@ -881,16 +1100,14 @@
             Initialization method.
         device : torch.device, optional
             Device where to initialize the tensors if ``init_method`` is provided.
         kwargs : float
             Keyword arguments for the different initialization methods. See
             :meth:`~tensorkrowch.AbstractNode.make_tensor`.
         """
-        node = self.uniform_memory
-        
         if tensors is not None:
             self.uniform_memory.tensor = tensors[0]
         
         elif init_method is not None:
             self.uniform_memory.set_tensor(init_method=init_method,
                                            device=device,
                                            **kwargs)
@@ -963,7 +1180,18 @@
         
         # Tensor addresses have to be reassigned to reference
         # the uniform memory
         for node in net._mats_env:
             node.set_tensor_from(net.uniform_memory)
             
         return net
+    
+    def canonicalize(self,
+                     oc: Optional[int] = None,
+                     mode: Text = 'svd',
+                     rank: Optional[int] = None,
+                     cum_percentage: Optional[float] = None,
+                     cutoff: Optional[float] = None,
+                     renormalize: bool = False) -> None:
+        """:meta private:"""
+        raise NotImplementedError(
+            '`canonicalize` not implemented for UMPO')
```

### Comparing `tensorkrowch-1.1.0/tensorkrowch/models/mps.py` & `tensorkrowch-1.1.1/tensorkrowch/models/mps.py`

 * *Files 9% similar despite different names*

```diff
@@ -533,17 +533,17 @@
                 aux_bond_dim = [1]
                 
             self._left_node = ParamNode(shape=(aux_bond_dim[0],),
                                         axes_names=('right',),
                                         name='left_node',
                                         network=self)
             self._right_node = ParamNode(shape=(aux_bond_dim[-1],),
-                                    axes_names=('left',),
-                                    name='right_node',
-                                    network=self)
+                                         axes_names=('left',),
+                                         name='right_node',
+                                         network=self)
             
             aux_bond_dim = aux_bond_dim + [aux_bond_dim[-1]] + [aux_bond_dim[0]]
         
         for i in range(self._n_features):
             node = ParamNode(shape=(aux_bond_dim[i - 1],
                                     self._phys_dim[i],
                                     aux_bond_dim[i]),
@@ -562,43 +562,96 @@
                     self._mats_env[-1]['right'] ^ periodic_edge
             else:
                 if i == 0:
                     self._left_node['right'] ^ self._mats_env[-1]['left']
                 if i == self._n_features - 1:
                     self._mats_env[-1]['right'] ^ self._right_node['left']
     
-    def _make_unitaries(self, device: Optional[torch.device] = None) -> List[torch.Tensor]:
+    def _make_canonical(self, device: Optional[torch.device] = None) -> List[torch.Tensor]:
         """
         Creates random unitaries to initialize the MPS in canonical form with
-        orthogonality center at the rightmost node."""
+        orthogonality center at the rightmost node. Unitaries in nodes are
+        scaled so that the total norm squared of the initial MPS is the product
+        of all the physical dimensions.
+        """
         tensors = []
         for i, node in enumerate(self._mats_env):
             if self._boundary == 'obc':
                 if i == 0:
                     node_shape = node.shape[1:]
                     aux_shape = node_shape
+                    phys_dim = node_shape[0]
                 elif i == (self._n_features - 1):
                     node_shape = node.shape[:2]
                     aux_shape = node_shape
+                    phys_dim = node_shape[1]
                 else:
                     node_shape = node.shape
                     aux_shape = (node.shape[:2].numel(), node.shape[2])
+                    phys_dim = node_shape[1]
             else:
                 node_shape = node.shape
                 aux_shape = (node.shape[:2].numel(), node.shape[2])
+                phys_dim = node_shape[1]
             size = max(aux_shape[0], aux_shape[1])
             
             tensor = random_unitary(size, device=device)
             tensor = tensor[:min(aux_shape[0], size), :min(aux_shape[1], size)]
             tensor = tensor.reshape(*node_shape)
             
+            if i == (self._n_features - 1):
+                if self._boundary == 'obc':
+                    tensor = tensor.t() / tensor.norm() * sqrt(phys_dim)
+                else:
+                    tensor = tensor / tensor.norm() * sqrt(phys_dim)
+            else:
+                tensor = tensor * sqrt(phys_dim)
+            
             tensors.append(tensor)
-        
-        if self._boundary == 'obc':
-            tensors[-1] = tensors[-1] / tensors[-1].norm()
+        return tensors
+    
+    def _make_unitaries(self, device: Optional[torch.device] = None) -> List[torch.Tensor]:
+        """
+        Creates random unitaries to initialize the MPS nodes as stacks of
+        unitaries.
+        """
+        tensors = []
+        for i, node in enumerate(self._mats_env):
+            units = []
+            size = max(node.shape[0], node.shape[2])
+            if self._boundary == 'obc':
+                if i == 0:
+                    size_1 = 1
+                    size_2 = min(node.shape[2], size)
+                elif i == (self._n_features - 1):
+                    size_1 = min(node.shape[0], size)
+                    size_2 = 1
+                else:
+                    size_1 = min(node.shape[0], size)
+                    size_2 = min(node.shape[2], size)
+            else:
+                size_1 = min(node.shape[0], size)
+                size_2 = min(node.shape[2], size)
+            
+            for _ in range(node.shape[1]):
+                tensor = random_unitary(size, device=device)
+                tensor = tensor[:size_1, :size_2]
+                units.append(tensor)
+            
+            units = torch.stack(units, dim=1)
+            
+            if self._boundary == 'obc':
+                if i == 0:
+                    tensors.append(units.squeeze(0))
+                elif i == (self._n_features - 1):
+                    tensors.append(units.squeeze(-1))
+                else:
+                    tensors.append(units)
+            else:    
+                tensors.append(units)
         return tensors
 
     def initialize(self,
                    tensors: Optional[Sequence[torch.Tensor]] = None,
                    init_method: Optional[Text] = 'randn',
                    device: Optional[torch.device] = None,
                    **kwargs: float) -> None:
@@ -613,60 +666,69 @@
           the given method, ``device`` and ``kwargs``.
         
         * ``"randn_eye"``: Nodes are initialized as in this
           `paper <https://arxiv.org/abs/1605.03795>`_, adding identities at the
           top of random gaussian tensors. In this case, ``std`` should be
           specified with a low value, e.g., ``std = 1e-9``.
         
-        * ``"unit"``: Nodes are initialized as random unitaries, so that the
-          MPS is in canonical form, with the orthogonality center at the
-          rightmost node.
+        * ``"unit"``: Nodes are initialized as stacks of random unitaries. This,
+          combined (at least) with an embedding of the inputs as elements of
+          the computational basis (:func:`~tensorkrowch.embeddings.discretize`
+          combined with :func:`~tensorkrowch.embeddings.basis`)
+        
+        * ``"canonical"```: MPS is initialized in canonical form with a squared
+          norm `close` to the product of all the physical dimensions (if bond
+          dimensions are bigger than the powers of the physical dimensions,
+          the norm could vary). Th orthogonality center is at the rightmost
+          node.
         
         Parameters
         ----------
         tensors : list[torch.Tensor] or tuple[torch.Tensor], optional
             Sequence of tensors to set in each of the MPS nodes. If ``boundary``
             is ``"obc"``, all tensors should be rank-3, except the first and
             last ones, which can be rank-2, or rank-1 (if the first and last are
             the same). If ``boundary`` is ``"pbc"``, all tensors should be
             rank-3.
-        init_method : {"zeros", "ones", "copy", "rand", "randn", "randn_eye", "unit"}, optional
+        init_method : {"zeros", "ones", "copy", "rand", "randn", "randn_eye", "unit", "canonical"}, optional
             Initialization method.
         device : torch.device, optional
             Device where to initialize the tensors if ``init_method`` is provided.
         kwargs : float
             Keyword arguments for the different initialization methods. See
             :meth:`~tensorkrowch.AbstractNode.make_tensor`.
         """
-        if self._boundary == 'obc':
-            self._left_node.set_tensor(init_method='copy', device=device)
-            self._right_node.set_tensor(init_method='copy', device=device)
-        
         if init_method == 'unit':
             tensors = self._make_unitaries(device=device)
+        elif init_method == 'canonical':
+            tensors = self._make_canonical(device=device)
 
         if tensors is not None:
             if len(tensors) != self._n_features:
-                raise ValueError('`tensors` should be a sequence of `n_features`'
-                                 ' elements')
+                raise ValueError(
+                    '`tensors` should be a sequence of `n_features` elements')
             
             if self._boundary == 'obc':
                 tensors = tensors[:]
+                
+                if device is None:
+                    device = tensors[0].device
+                
                 if len(tensors) == 1:
                     tensors[0] = tensors[0].reshape(1, -1, 1)
                 else:
                     # Left node
                     aux_tensor = torch.zeros(*self._mats_env[0].shape,
-                                             device=tensors[0].device)
+                                             device=device)
                     aux_tensor[0] = tensors[0]
                     tensors[0] = aux_tensor
                     
                     # Right node
                     aux_tensor = torch.zeros(*self._mats_env[-1].shape,
-                                             device=tensors[-1].device)
+                                             device=device)
                     aux_tensor[..., 0] = tensors[-1]
                     tensors[-1] = aux_tensor
                 
             for tensor, node in zip(tensors, self._mats_env):
                 node.tensor = tensor
                 
         elif init_method is not None:
@@ -692,14 +754,18 @@
                         # Left node
                         aux_tensor[0] = node.tensor[0]
                         node.tensor = aux_tensor
                     elif i == (self._n_features - 1):
                         # Right node
                         aux_tensor[..., 0] = node.tensor[..., 0]
                         node.tensor = aux_tensor
+        
+        if self._boundary == 'obc':
+            self._left_node.set_tensor(init_method='copy', device=device)
+            self._right_node.set_tensor(init_method='copy', device=device)
 
     def set_data_nodes(self) -> None:
         """
         Creates ``data`` nodes and connects each of them to the ``"input"``
         edge of each input node.
         """      
         input_edges = [node['input'] for node in self.in_env]
@@ -783,15 +849,15 @@
                            input_nodes: List[AbstractNode],
                            inline_input: bool = False) -> Tuple[
                                                        Optional[List[Node]],
                                                        Optional[List[Node]]]:
         """Contracts input data nodes with MPS input nodes."""
         if inline_input:
             mats_result = [
-                node @ in_node
+                in_node @ node
                 for node, in_node in zip(nodes_env, input_nodes)
                 ]
             return mats_result
 
         else:
             if nodes_env:
                 stack = op.stack(nodes_env)
@@ -803,43 +869,69 @@
                 mats_result = op.unbind(result)
                 return mats_result
             else:
                 return []
 
     @staticmethod
     def _inline_contraction(mats_env: List[AbstractNode],
+                            renormalize: bool = False,
                             from_left: bool = True) -> Node:
         """Contracts sequence of MPS nodes (matrices) inline."""
         if from_left:
             result_node = mats_env[0]
             for node in mats_env[1:]:
                 result_node @= node
+                
+                if renormalize:
+                    right_axes = []
+                    for ax_name in result_node.axes_names:
+                        if 'right' in ax_name:
+                            right_axes.append(ax_name)
+                    if right_axes:
+                        result_node = result_node.renormalize(axis=right_axes)
+            
             return result_node
+        
         else:
             result_node = mats_env[-1]
             for node in mats_env[-2::-1]:
                 result_node = node @ result_node
+                
+                if renormalize:
+                    left_axes = []
+                    for ax_name in result_node.axes_names:
+                        if 'left' in ax_name:
+                            left_axes.append(ax_name)
+                    if left_axes:
+                        result_node = result_node.renormalize(axis=left_axes)
+            
             return result_node
 
-    def _contract_envs_inline(self, mats_env: List[AbstractNode]) -> Node:
+    def _contract_envs_inline(self,
+                              mats_env: List[AbstractNode],
+                              renormalize: bool = False) -> Node:
         """Contracts nodes environments inline."""
         from_left = True
         if self._boundary == 'obc':
             if mats_env[0].neighbours('left') is self._left_node:
                 mats_env = [self._left_node] + mats_env
             if mats_env[-1].neighbours('right') is self._right_node:
                 mats_env = mats_env + [self._right_node]
                 from_left = False
-        return self._inline_contraction(mats_env=mats_env, from_left=from_left)
-
-    def _aux_pairwise(self, nodes: List[AbstractNode]) -> Tuple[List[Node],
+        return self._inline_contraction(mats_env=mats_env,
+                                        renormalize=renormalize,
+                                        from_left=from_left)
+
+    def _aux_pairwise(self,
+                      mats_env: List[AbstractNode],
+                      renormalize: bool = False) -> Tuple[List[Node],
     List[Node]]:
         """Contracts a sequence of MPS nodes (matrices) pairwise."""
-        length = len(nodes)
-        aux_nodes = nodes
+        length = len(mats_env)
+        aux_nodes = mats_env
         if length > 1:
             half_length = length // 2
             nice_length = 2 * half_length
 
             even_nodes = aux_nodes[0:nice_length:2]
             odd_nodes = aux_nodes[1:nice_length:2]
             leftover = aux_nodes[nice_length:]
@@ -847,38 +939,53 @@
             stack1 = op.stack(even_nodes)
             stack2 = op.stack(odd_nodes)
 
             stack1['right'] ^ stack2['left']
 
             aux_nodes = stack1 @ stack2
             aux_nodes = op.unbind(aux_nodes)
+            
+            if renormalize:
+                for i in range(len(aux_nodes)):
+                    axes = []
+                    for ax_name in aux_nodes[i].axes_names:
+                        if ('left' in ax_name) or ('right' in ax_name):
+                            axes.append(ax_name)
+                    if axes:
+                        aux_nodes[i] = aux_nodes[i].renormalize(axis=axes)
 
             return aux_nodes, leftover
-        return nodes, []
+        return mats_env, []
 
-    def _pairwise_contraction(self, mats_env: List[AbstractNode]) -> Node:
+    def _pairwise_contraction(self,
+                              mats_env: List[AbstractNode],
+                              renormalize: bool = False) -> Node:
         """Contracts nodes environments pairwise."""
         length = len(mats_env)
         aux_nodes = mats_env
         if length > 1:
             leftovers = []
             while length > 1:
-                aux1, aux2 = self._aux_pairwise(aux_nodes)
+                aux1, aux2 = self._aux_pairwise(mats_env=aux_nodes,
+                                                renormalize=renormalize)
                 aux_nodes = aux1
                 leftovers = aux2 + leftovers
                 length = len(aux1)
 
             aux_nodes = aux_nodes + leftovers
-            return self._pairwise_contraction(aux_nodes)
+            return self._pairwise_contraction(mats_env=aux_nodes,
+                                              renormalize=renormalize)
 
-        return self._contract_envs_inline(aux_nodes)
+        return self._contract_envs_inline(mats_env=aux_nodes,
+                                          renormalize=renormalize)
 
     def contract(self,
                  inline_input: bool = False,
                  inline_mats: bool = False,
+                 renormalize: bool = False,
                  marginalize_output: bool = False,
                  embedding_matrices: Optional[
                                         Union[torch.Tensor,
                                               Sequence[torch.Tensor]]] = None,
                  mpo: Optional[MPO] = None
                  ) -> Node:
         """
@@ -932,14 +1039,23 @@
             Boolean indicating whether input ``data`` nodes should be contracted
             with the ``MPS`` input nodes inline (one contraction at a time) or
             in a single stacked contraction.
         inline_mats : bool
             Boolean indicating whether the sequence of matrices (resultant
             after contracting the input ``data`` nodes) should be contracted
             inline or as a sequence of pairwise stacked contrations.
+        renormalize : bool
+            Indicates whether nodes should be renormalized after contraction.
+            If not, it may happen that the norm explodes or vanishes, as it
+            is being accumulated from all nodes. Renormalization aims to avoid
+            this undesired behavior by extracting the norm of each node on a
+            logarithmic scale. The renormalization only occurs when multiplying
+            sequences of matrices, once the `input` contractions have been
+            already performed, including contracting against embedding matrices
+            or MPOs when ``marginalize_output = True``.
         marginalize_output : bool
             Boolean indicating whether output nodes should be marginalized. If
             ``True``, after contracting all the input nodes with their
             neighbouring data nodes, this resultant network is contracted with
             itself connecting output nodes to itselves at ``"input"`` edges. If
             ``False``, output nodes are left with their ``"input"`` edges
             disconnected.
@@ -998,22 +1114,39 @@
         out_regions = self.out_regions
         
         mats_in_env = self._input_contraction(
             nodes_env=self.in_env,
             input_nodes=[node.neighbours('input') for node in self.in_env],
             inline_input=inline_input)
         
+        # NOTE: to leave the input edges open and marginalize output
+        # data_nodes = []
+        # for node in self.in_env:
+        #     data_node = node.neighbours('input')
+        #     if data_node:
+        #         data_nodes.append(data_node)
+        
+        # if data_nodes:
+        #     mats_in_env = self._input_contraction(
+        #         nodes_env=self.in_env,
+        #         input_nodes=data_nodes,
+        #         inline_input=inline_input)
+        # else:
+        #     mats_in_env = self.in_env
+        
         in_results = []
         for region in in_regions:      
             if inline_mats:
                 result = self._contract_envs_inline(
-                    mats_env=mats_in_env[:len(region)])
+                    mats_env=mats_in_env[:len(region)],
+                    renormalize=renormalize)
             else:
                 result = self._pairwise_contraction(
-                    mats_env=mats_in_env[:len(region)])
+                    mats_env=mats_in_env[:len(region)],
+                    renormalize=renormalize)
             
             mats_in_env = mats_in_env[len(region):]
             in_results.append(result)
         
         if not out_regions:
             # If there is only input region, in_results has only 1 node
             result = in_results[0]
@@ -1039,15 +1172,16 @@
                 if (self._boundary == 'obc'):
                     nodes_out_env[-1] = nodes_out_env[-1] @ self._right_node
             else:
                 nodes_out_env[-1] = nodes_out_env[-1] @ in_results[-1]
             
             if not marginalize_output:
                 # Contract all output nodes sequentially
-                result = self._inline_contraction(mats_env=nodes_out_env)
+                result = self._inline_contraction(mats_env=nodes_out_env,
+                                                  renormalize=renormalize)
             
             else:
                 # Copy output nodes sharing tensors
                 copied_nodes = []
                 for node in nodes_out_env:
                     copied_node = node.__class__(shape=node._shape,
                                               axes_names=node.axes_names,
@@ -1144,15 +1278,16 @@
                 # Contract output nodes with copies
                 mats_out_env = self._input_contraction(
                     nodes_env=nodes_out_env,
                     input_nodes=copied_nodes,
                     inline_input=True)
                 
                 # Contract resultant matrices
-                result = self._inline_contraction(mats_env=mats_out_env)
+                result = self._inline_contraction(mats_env=mats_out_env,
+                                                  renormalize=renormalize)
             
         # Contract periodic edge
         if result.is_connected_to(result):
             result @= result
         
         # Put batch edges in first positions
         batch_edges = []
@@ -1185,18 +1320,20 @@
             self.unset_data_nodes()
         self.in_features = []
         
         result = self.forward(marginalize_output=True)
         result = result.sqrt()
         return result
 
-    def partial_density(self, trace_sites: Sequence[int] = []) -> torch.Tensor:
-        """
+    def partial_density(self,
+                        trace_sites: Sequence[int] = [],
+                        renormalize: bool = True) -> torch.Tensor:
+        r"""
         Returns de partial density matrix, tracing out the sites specified
-        by ``trace_sites``.
+        by ``trace_sites``: :math:`\rho_A`.
         
         This method internally sets ``out_features = trace_sites``, and calls
         the :meth:`~tensorkrowch.TensorNetwork.forward` method with
         ``marginalize_output = True``. Therefore, it may alter the behaviour
         of the MPS if it is not :meth:`~tensorkrowch.TensorNetwork.reset`
         afterwards. Also, if the MPS was contracted before with other arguments,
         it should be ``reset`` before calling ``partial_density`` to avoid
@@ -1212,14 +1349,22 @@
         Parameters
         ----------
         trace_sites : list[int] or tuple[int]
             Sequence of nodes' indices in the MPS. These indices specify the
             nodes that should be traced to compute the density matrix. If
             it is empty ``[]``, the total density matrix will be returned,
             though this may be costly if :attr:`n_features` is big.
+        renormalize : bool
+            Indicates whether nodes should be renormalized after contraction.
+            If not, it may happen that the norm explodes or vanishes, as it
+            is being accumulated from all nodes. Renormalization aims to avoid
+            this undesired behavior by extracting the norm of each node on a
+            logarithmic scale. The renormalization only occurs when multiplying
+            sequences of matrices, once the `input` contractions have been
+            already performed.
         
         Examples
         --------
         >>> mps = tk.models.MPS(n_features=4,
         ...                     phys_dim=[2, 3, 4, 5],
         ...                     bond_dim=5)
         >>> density = mps.partial_density(trace_sites=[0, 2])
@@ -1263,45 +1408,56 @@
             elif n_dims > 1:
                 data = [
                     basis(dat, dim=dim).squeeze(-2).float().to(self.in_env[0].device)
                     for dat, dim in zip(data, dims)
                     ]
             
             self.n_batches = len(dims)
-            result = self.forward(data, marginalize_output=True)
+            result = self.forward(data,
+                                  renormalize=renormalize,
+                                  marginalize_output=True)
             
         else:
-            result = self.forward(marginalize_output=True)
+            result = self.forward(renormalize=renormalize,
+                                  marginalize_output=True)
         
         return result
     
     @torch.no_grad()
-    def mi(self,
-           middle_site: int,
-           renormalize: bool = False) -> Union[float, Tuple[float]]:
+    def entropy(self,
+                middle_site: int,
+                renormalize: bool = False) -> Union[float, Tuple[float]]:
         r"""
-        Computes the Mutual Information between subsystems :math:`A` and
-        :math:`B`, :math:`\textrm{MI}(A:B)`, where :math:`A` goes from site
+        Computes the reduced von Neumann Entropy between subsystems :math:`A`
+        and :math:`B`, :math:`S(\rho_A)`, where :math:`A` goes from site
         0 to ``middle_site``, and :math:`B` goes from ``middle_site + 1`` to
         ``n_features - 1``.
         
-        To compute the mutual information, the MPS is put into canonical form
+        To compute the reduced entropy, the MPS is put into canonical form
         with orthogonality center at ``middle_site``. Bond dimensions are not
         changed if possible. Only when the bond dimension is bigger than the
         physical dimension multiplied by the other bond dimension of the node,
         it will be cropped to that size.
         
         If the MPS is not normalized, it may happen that the computation of the
-        mutual information fails due to errors in the Singular Value
+        reduced entropy fails due to errors in the Singular Value
         Decompositions. To avoid this, it is recommended to set
         ``renormalize = True``. In this case, the norm of each node after the
         SVD is extracted in logarithmic form, and accumulated. As a result,
-        the function will return the tuple ``(mi, log_norm)``, which is a sort
-        of `scaled` mutual information. The actual mutual information could be
-        obtained as ``exp(log_norm) * mi``.
+        the function will return the tuple ``(entropy, log_norm)``, which is a
+        sort of `scaled` reduced entropy. This is, indeed, the reduced entropy
+        of a distribution, since the schmidt values are normalized to sum up
+        to 1.
+        
+        The actual reduced entropy, without rescaling, could be obtained as:
+        
+        .. math::
+        
+            \exp(\texttt{log_norm})^2 \cdot S(\rho_A) - 
+            \exp(\texttt{log_norm})^2 \cdot 2 \cdot \texttt{log_norm}
         
         Parameters
         ----------
         middle_site : int
             Position that separates regios :math:`A` and :math:`B`. It should
             be between 0 and ``n_features - 2``.
         renormalize : bool
@@ -1360,26 +1516,32 @@
                 if not aux_norm.isinf() and (aux_norm > 0):
                     result1.tensor = result1.tensor / aux_norm
                     log_norm += aux_norm.log()
 
             result2 = result2.parameterize()
             nodes[i] = result2
             nodes[i - 1] = result1
-
+        
+        if renormalize:
+            aux_norm = nodes[middle_site].norm()
+            if not aux_norm.isinf() and (aux_norm > 0):
+                nodes[middle_site].tensor = nodes[middle_site].tensor / aux_norm
+                log_norm += aux_norm.log()
+        
         nodes[middle_site] = nodes[middle_site].parameterize()
         
         # Compute mutual information
         middle_tensor = nodes[middle_site].tensor.clone()
         _, s, _ = torch.linalg.svd(
             middle_tensor.reshape(middle_tensor.shape[:-1].numel(), # left x input
                                   middle_tensor.shape[-1]),         # right
             full_matrices=False)
         
         s = s[s > 0]
-        mutual_info = -(s * (s.log() + log_norm)).sum()
+        entropy = -(s.pow(2) * s.pow(2).log()).sum()
         
         # Rescale
         if log_norm != 0:
             rescale = (log_norm / len(nodes)).exp()
         
         if renormalize and (log_norm != 0):
             for node in nodes:
@@ -1391,17 +1553,17 @@
         else:
             self._bond_dim = [node['right'].size() for node in nodes]
         self._mats_env = nodes
 
         self.auto_stack = prev_auto_stack
         
         if renormalize:
-            return mutual_info, log_norm
+            return entropy, log_norm
         else:
-            return mutual_info
+            return entropy
 
     @torch.no_grad()
     def canonicalize(self,
                      oc: Optional[int] = None,
                      mode: Text = 'svd',
                      rank: Optional[int] = None,
                      cum_percentage: Optional[float] = None,
@@ -1881,25 +2043,47 @@
                                    network=self,
                                    virtual=True)
         self.uniform_memory = uniform_memory
         
         for node in self._mats_env:
             node.set_tensor_from(uniform_memory)
     
-    def _make_unitaries(self, device: Optional[torch.device] = None) -> torch.Tensor:
-        """Initializes MPS in canonical form."""
+    def _make_canonical(self, device: Optional[torch.device] = None) -> List[torch.Tensor]:
+        """
+        Creates random unitaries to initialize the MPS in canonical form with
+        orthogonality center at the rightmost node. Unitaries in nodes are
+        scaled so that the total norm squared of the initial MPS is the product
+        of all the physical dimensions.
+        """
         node = self.uniform_memory
         node_shape = node.shape
         aux_shape = (node.shape[:2].numel(), node.shape[2])
         
         size = max(aux_shape[0], aux_shape[1])
+        phys_dim = node_shape[1]
         
         tensor = random_unitary(size, device=device)
         tensor = tensor[:min(aux_shape[0], size), :min(aux_shape[1], size)]
         tensor = tensor.reshape(*node_shape)
+        tensor = tensor * sqrt(phys_dim)
+        return tensor
+    
+    def _make_unitaries(self, device: Optional[torch.device] = None) -> List[torch.Tensor]:
+        """
+        Creates random unitaries to initialize the MPS nodes as stacks of
+        unitaries.
+        """
+        node = self.uniform_memory
+        node_shape = node.shape
+        
+        units = []
+        for _ in range(node_shape[1]):
+            tensor = random_unitary(node_shape[0], device=device)
+            units.append(tensor)
+        tensor = torch.stack(units, dim=1)
         return tensor
 
     def initialize(self,
                    tensors: Optional[Sequence[torch.Tensor]] = None,
                    init_method: Optional[Text] = 'randn',
                    device: Optional[torch.device] = None,
                    **kwargs: float) -> None:
@@ -1914,35 +2098,44 @@
           the given method, ``device`` and ``kwargs``.
         
         * ``"randn_eye"``: Tensor is initialized as in this
           `paper <https://arxiv.org/abs/1605.03795>`_, adding identities at the
           top of a random gaussian tensor. In this case, ``std`` should be
           specified with a low value, e.g., ``std = 1e-9``.
         
-        * ``"unit"``: Tensor is initialized as a random unitary, so that the
-          MPS is in canonical form.
+        * ``"unit"``: Tensor is initialized as a stack of random unitaries. This,
+          combined (at least) with an embedding of the inputs as elements of
+          the computational basis (:func:`~tensorkrowch.embeddings.discretize`
+          combined with :func:`~tensorkrowch.embeddings.basis`)
+        
+        * ``"canonical"```: MPS is initialized in canonical form with a squared
+          norm `close` to the product of all the physical dimensions (if bond
+          dimensions are bigger than the powers of the physical dimensions,
+          the norm could vary).
         
         Parameters
         ----------
         tensors : list[torch.Tensor] or tuple[torch.Tensor], optional
             Sequence of a single tensor to set in each of the MPS nodes. The
             tensor should be rank-3, with its first and last dimensions being
             equal.
-        init_method : {"zeros", "ones", "copy", "rand", "randn", "randn_eye", "unit"}, optional
+        init_method : {"zeros", "ones", "copy", "rand", "randn", "randn_eye", "unit", "canonical"}, optional
             Initialization method.
         device : torch.device, optional
             Device where to initialize the tensors if ``init_method`` is provided.
         kwargs : float
             Keyword arguments for the different initialization methods. See
             :meth:`~tensorkrowch.AbstractNode.make_tensor`.
         """
         node = self.uniform_memory
         
         if init_method == 'unit':
             tensors = [self._make_unitaries(device=device)]
+        elif init_method == 'canonical':
+            tensors = [self._make_canonical(device=device)]
         
         if tensors is not None:
             node.tensor = tensors[0]
         
         elif init_method is not None:
             add_eye = False
             if init_method == 'randn_eye':
@@ -2256,80 +2449,290 @@
         return self._out_position
     
     @property
     def out_node(self) -> ParamNode:
         """Returns the output node."""
         return self._mats_env[self._out_position]
     
+    def _make_canonical(self, device: Optional[torch.device] = None) -> List[torch.Tensor]:
+        """
+        Creates random unitaries to initialize the MPS in canonical form with
+        orthogonality center at the rightmost node. Unitaries in nodes are
+        scaled so that the total norm squared of the initial MPS is the product
+        of all the physical dimensions.
+        """
+        # Left nodes
+        left_tensors = []
+        for i, node in enumerate(self._mats_env[:self._out_position]):
+            if self._boundary == 'obc':
+                if i == 0:
+                    node_shape = node.shape[1:]
+                    aux_shape = node_shape
+                    phys_dim = node_shape[0]
+                else:
+                    node_shape = node.shape
+                    aux_shape = (node.shape[:2].numel(), node.shape[2])
+                    phys_dim = node_shape[1]
+            else:
+                node_shape = node.shape
+                aux_shape = (node.shape[:2].numel(), node.shape[2])
+                phys_dim = node_shape[1]
+            size = max(aux_shape[0], aux_shape[1])
+            
+            tensor = random_unitary(size, device=device)
+            tensor = tensor[:min(aux_shape[0], size), :min(aux_shape[1], size)]
+            tensor = tensor.reshape(*node_shape)
+            
+            left_tensors.append(tensor * sqrt(phys_dim))
+        
+        # Output node
+        out_tensor = torch.randn(self.out_node.shape, device=device)
+        phys_dim = out_tensor.shape[1]
+        if self._boundary == 'obc':
+            if self._out_position == 0:
+                out_tensor = out_tensor[0]
+            if self._out_position == (self._n_features - 1):
+                out_tensor = out_tensor[..., 0]
+        out_tensor = out_tensor / out_tensor.norm() * sqrt(phys_dim)
+        
+        # Right nodes
+        right_tensors = []
+        for i, node in enumerate(self._mats_env[-1:self._out_position:-1]):
+            if self._boundary == 'obc':
+                if i == 0:
+                    node_shape = node.shape[:2]
+                    aux_shape = node_shape
+                    phys_dim = node_shape[1]
+                else:
+                    node_shape = node.shape
+                    aux_shape = (node.shape[0], node.shape[1:].numel())
+                    phys_dim = node_shape[1]
+            else:
+                node_shape = node.shape
+                aux_shape = (node.shape[0], node.shape[1:].numel())
+                phys_dim = node_shape[1]
+            size = max(aux_shape[0], aux_shape[1])
+            
+            tensor = random_unitary(size, device=device)
+            tensor = tensor[:min(aux_shape[0], size), :min(aux_shape[1], size)]
+            tensor = tensor.reshape(*node_shape)
+            
+            right_tensors.append(tensor * sqrt(phys_dim))
+        right_tensors.reverse()
+        
+        # All tensors
+        tensors = left_tensors + [out_tensor] + right_tensors
+        return tensors
+    
+    def _make_unitaries(self, device: Optional[torch.device] = None) -> List[torch.Tensor]:
+        """
+        Creates random unitaries to initialize the MPS nodes as stacks of
+        unitaries.
+        """
+        # Left_nodes
+        left_tensors = []
+        for i, node in enumerate(self._mats_env[:self._out_position]):
+            units = []
+            size = max(node.shape[0], node.shape[2])
+            if self._boundary == 'obc':
+                if i == 0:
+                    size_1 = 1
+                    size_2 = min(node.shape[2], size)
+                else:
+                    size_1 = min(node.shape[0], size)
+                    size_2 = min(node.shape[2], size)
+            else:
+                size_1 = min(node.shape[0], size)
+                size_2 = min(node.shape[2], size)
+            
+            for _ in range(node.shape[1]):
+                tensor = random_unitary(size, device=device)
+                tensor = tensor[:size_1, :size_2]
+                units.append(tensor)
+            
+            units = torch.stack(units, dim=1)
+            
+            if self._boundary == 'obc':
+                if i == 0:
+                    left_tensors.append(units.squeeze(0))
+                else:
+                    left_tensors.append(units)
+            else:    
+                left_tensors.append(units)
+        
+        # Output node
+        out_tensor = torch.randn(self.out_node.shape, device=device)
+        if self._boundary == 'obc':
+            if self._out_position == 0:
+                out_tensor = out_tensor[0]
+            if self._out_position == (self._n_features - 1):
+                out_tensor = out_tensor[..., 0]
+        
+        # Right nodes
+        right_tensors = []
+        for i, node in enumerate(self._mats_env[-1:self._out_position:-1]):
+            units = []
+            size = max(node.shape[0], node.shape[2])
+            if self._boundary == 'obc':
+                if i == 0:
+                    size_1 = min(node.shape[0], size)
+                    size_2 = 1
+                else:
+                    size_1 = min(node.shape[0], size)
+                    size_2 = min(node.shape[2], size)
+            else:
+                size_1 = min(node.shape[0], size)
+                size_2 = min(node.shape[2], size)
+            
+            for _ in range(node.shape[1]):
+                tensor = random_unitary(size, device=device).t()
+                tensor = tensor[:size_1, :size_2]
+                units.append(tensor)
+            
+            units = torch.stack(units, dim=1)
+            
+            if self._boundary == 'obc':
+                if i == 0:
+                    right_tensors.append(units.squeeze(-1))
+                else:
+                    right_tensors.append(units)
+            else:    
+                right_tensors.append(units)
+        right_tensors.reverse()
+        
+        # All tensors
+        tensors = left_tensors + [out_tensor] + right_tensors
+        return tensors
+
     def initialize(self,
                    tensors: Optional[Sequence[torch.Tensor]] = None,
                    init_method: Optional[Text] = 'randn',
                    device: Optional[torch.device] = None,
                    **kwargs: float) -> None:
         """
-        Initializes all the nodes of the :class:`MPSLayer`. It can be called when
+        Initializes all the nodes of the :class:`MPS`. It can be called when
         instantiating the model, or to override the existing nodes' tensors.
         
         There are different methods to initialize the nodes:
         
         * ``{"zeros", "ones", "copy", "rand", "randn"}``: Each node is
           initialized calling :meth:`~tensorkrowch.AbstractNode.set_tensor` with
           the given method, ``device`` and ``kwargs``.
         
         * ``"randn_eye"``: Nodes are initialized as in this
           `paper <https://arxiv.org/abs/1605.03795>`_, adding identities at the
           top of random gaussian tensors. In this case, ``std`` should be
           specified with a low value, e.g., ``std = 1e-9``.
         
-        * ``"unit"``: Nodes are initialized as random unitaries, so that the
-          MPS is in canonical form, with the orthogonality center at the
-          rightmost node.
+        * ``"unit"``: Nodes are initialized as stacks of random unitaries. This,
+          combined (at least) with an embedding of the inputs as elements of
+          the computational basis (:func:`~tensorkrowch.embeddings.discretize`
+          combined with :func:`~tensorkrowch.embeddings.basis`)
+        
+        * ``"canonical"```: MPS is initialized in canonical form with a squared
+          norm `close` to the product of all the physical dimensions (if bond
+          dimensions are bigger than the powers of the physical dimensions,
+          the norm could vary). Th orthogonality center is at the rightmost
+          node.
         
         Parameters
         ----------
         tensors : list[torch.Tensor] or tuple[torch.Tensor], optional
             Sequence of tensors to set in each of the MPS nodes. If ``boundary``
             is ``"obc"``, all tensors should be rank-3, except the first and
             last ones, which can be rank-2, or rank-1 (if the first and last are
             the same). If ``boundary`` is ``"pbc"``, all tensors should be
             rank-3.
-        init_method : {"zeros", "ones", "copy", "rand", "randn", "randn_eye", "unit"}, optional
+        init_method : {"zeros", "ones", "copy", "rand", "randn", "randn_eye", "unit", "canonical"}, optional
             Initialization method.
         device : torch.device, optional
             Device where to initialize the tensors if ``init_method`` is provided.
         kwargs : float
             Keyword arguments for the different initialization methods. See
             :meth:`~tensorkrowch.AbstractNode.make_tensor`.
         """
-        if self._boundary == 'obc':
-            self._left_node.set_tensor(init_method='copy', device=device)
-            self._right_node.set_tensor(init_method='copy', device=device)
+        if init_method == 'unit':
+            tensors = self._make_unitaries(device=device)
+        elif init_method == 'canonical':
+            tensors = self._make_canonical(device=device)
+    
+    def initialize(self,
+                   tensors: Optional[Sequence[torch.Tensor]] = None,
+                   init_method: Optional[Text] = 'randn',
+                   device: Optional[torch.device] = None,
+                   **kwargs: float) -> None:
+        """
+        Initializes all the nodes of the :class:`MPSLayer`. It can be called when
+        instantiating the model, or to override the existing nodes' tensors.
+        
+        There are different methods to initialize the nodes:
+        
+        * ``{"zeros", "ones", "copy", "rand", "randn"}``: Each node is
+          initialized calling :meth:`~tensorkrowch.AbstractNode.set_tensor` with
+          the given method, ``device`` and ``kwargs``.
+        
+        * ``"randn_eye"``: Nodes are initialized as in this
+          `paper <https://arxiv.org/abs/1605.03795>`_, adding identities at the
+          top of random gaussian tensors. In this case, ``std`` should be
+          specified with a low value, e.g., ``std = 1e-9``.
+        
+        * ``"unit"``: Nodes are initialized as stacks of random unitaries. This,
+          combined (at least) with an embedding of the inputs as elements of
+          the computational basis (:func:`~tensorkrowch.embeddings.discretize`
+          combined with :func:`~tensorkrowch.embeddings.basis`)
+        
+        * ``"canonical"```: MPS is initialized in canonical form with a squared
+          norm `close` to the product of all the physical dimensions (if bond
+          dimensions are bigger than the powers of the physical dimensions,
+          the norm could vary). Th orthogonality center is at the output node.
         
+        Parameters
+        ----------
+        tensors : list[torch.Tensor] or tuple[torch.Tensor], optional
+            Sequence of tensors to set in each of the MPS nodes. If ``boundary``
+            is ``"obc"``, all tensors should be rank-3, except the first and
+            last ones, which can be rank-2, or rank-1 (if the first and last are
+            the same). If ``boundary`` is ``"pbc"``, all tensors should be
+            rank-3.
+        init_method : {"zeros", "ones", "copy", "rand", "randn", "randn_eye", "unit", "canonical"}, optional
+            Initialization method.
+        device : torch.device, optional
+            Device where to initialize the tensors if ``init_method`` is provided.
+        kwargs : float
+            Keyword arguments for the different initialization methods. See
+            :meth:`~tensorkrowch.AbstractNode.make_tensor`.
+        """
         if init_method == 'unit':
             tensors = self._make_unitaries(device=device)
+        elif init_method == 'canonical':
+            tensors = self._make_canonical(device=device)
 
         if tensors is not None:
             if len(tensors) != self._n_features:
                 raise ValueError('`tensors` should be a sequence of `n_features`'
                                  ' elements')
             
             if self._boundary == 'obc':
                 tensors = tensors[:]
+                
+                if device is None:
+                    device = tensors[0].device
+                
                 if len(tensors) == 1:
                     tensors[0] = tensors[0].reshape(1, -1, 1)
                 else:
                     # Left node
                     aux_tensor = torch.zeros(*self._mats_env[0].shape,
-                                             device=tensors[0].device)
+                                             device=device)
                     aux_tensor[0] = tensors[0]
                     tensors[0] = aux_tensor
                     
                     # Right node
                     aux_tensor = torch.zeros(*self._mats_env[-1].shape,
-                                             device=tensors[-1].device)
+                                             device=device)
                     aux_tensor[..., 0] = tensors[-1]
                     tensors[-1] = aux_tensor
                 
             for tensor, node in zip(tensors, self._mats_env):
                 node.tensor = tensor
                 
         elif init_method is not None:
@@ -2361,14 +2764,18 @@
                         # Left node
                         aux_tensor[0] = node.tensor[0]
                         node.tensor = aux_tensor
                     elif i == (self._n_features - 1):
                         # Right node
                         aux_tensor[..., 0] = node.tensor[..., 0]
                         node.tensor = aux_tensor
+        
+        if self._boundary == 'obc':
+            self._left_node.set_tensor(init_method='copy', device=device)
+            self._right_node.set_tensor(init_method='copy', device=device)
 
     def copy(self, share_tensors: bool = False) -> 'MPSLayer':
         """
         Creates a copy of the :class:`MPSLayer`.
 
         Parameters
         ----------
@@ -2604,28 +3011,56 @@
         self.uniform_memory = uniform_memory
         
         in_nodes = self._mats_env[:self._out_position] + \
             self._mats_env[(self._out_position + 1):]
         for node in in_nodes:
             node.set_tensor_from(uniform_memory)
     
+    def _make_canonical(self, device: Optional[torch.device] = None) -> List[torch.Tensor]:
+        """
+        Creates random unitaries to initialize the MPS in canonical form with
+        orthogonality center at the rightmost node. Unitaries in nodes are
+        scaled so that the total norm squared of the initial MPS is the product
+        of all the physical dimensions.
+        """
+        # Uniform node
+        node = self.uniform_memory
+        node_shape = node.shape
+        aux_shape = (node.shape[:2].numel(), node.shape[2])
+        
+        size = max(aux_shape[0], aux_shape[1])
+        phys_dim = node_shape[1]
+        
+        uni_tensor = random_unitary(size, device=device)
+        uni_tensor = uni_tensor[:min(aux_shape[0], size), :min(aux_shape[1], size)]
+        uni_tensor = uni_tensor.reshape(*node_shape)
+        uni_tensor = uni_tensor * sqrt(phys_dim)
+        
+        # Output node
+        out_tensor = torch.randn(self.out_node.shape, device=device)
+        out_tensor = out_tensor / out_tensor.norm() * sqrt(out_tensor.shape[1])
+        
+        return [uni_tensor, out_tensor]
+    
     def _make_unitaries(self, device: Optional[torch.device] = None) -> List[torch.Tensor]:
-        """Initializes MPS in canonical form."""
+        """
+        Creates random unitaries to initialize the MPS nodes as stacks of
+        unitaries.
+        """
         tensors = []
         for node in [self.uniform_memory, self.out_node]:
             node_shape = node.shape
-            aux_shape = (node.shape[:2].numel(), node.shape[2])
             
-            size = max(aux_shape[0], aux_shape[1])
+            units = []
+            for _ in range(node_shape[1]):
+                tensor = random_unitary(node_shape[0], device=device)
+                units.append(tensor)
             
-            tensor = random_unitary(size, device=device)
-            tensor = tensor[:min(aux_shape[0], size), :min(aux_shape[1], size)]
-            tensor = tensor.reshape(*node_shape)
-            
-            tensors.append(tensor)
+            tensors.append(torch.stack(units, dim=1))
+        
         return tensors
 
     def initialize(self,
                    tensors: Optional[Sequence[torch.Tensor]] = None,
                    init_method: Optional[Text] = 'randn',
                    device: Optional[torch.device] = None,
                    **kwargs: float) -> None:
@@ -2639,35 +3074,44 @@
           initialized calling :meth:`~tensorkrowch.AbstractNode.set_tensor` with
           the given method, ``device`` and ``kwargs``.
         
         * ``"randn_eye"``: Tensor is initialized as in this
           `paper <https://arxiv.org/abs/1605.03795>`_, adding identities at the
           top of a random gaussian tensor. In this case, ``std`` should be
           specified with a low value, e.g., ``std = 1e-9``.
-        
-        * ``"unit"``: Tensor is initialized as a random unitary, so that the
-          MPS is in canonical form.
+          
+        * ``"unit"``: Tensor is initialized as a stack of random unitaries. This,
+          combined (at least) with an embedding of the inputs as elements of
+          the computational basis (:func:`~tensorkrowch.embeddings.discretize`
+          combined with :func:`~tensorkrowch.embeddings.basis`)
+        
+        * ``"canonical"```: MPS is initialized in canonical form with a squared
+          norm `close` to the product of all the physical dimensions (if bond
+          dimensions are bigger than the powers of the physical dimensions,
+          the norm could vary).
         
         Parameters
         ----------
         tensors : list[torch.Tensor] or tuple[torch.Tensor], optional
             Sequence of a 2 tensors, the first one will be the uniform tensor
             that will be set in all input nodes, and the second one will be the
             output node's tensor. Both tensors should be rank-3, with all their
             first and last dimensions being equal.
-        init_method : {"zeros", "ones", "copy", "rand", "randn", "randn_eye", "unit"}, optional
+        init_method : {"zeros", "ones", "copy", "rand", "randn", "randn_eye", "unit", "canonical"}, optional
             Initialization method.
         device : torch.device, optional
             Device where to initialize the tensors if ``init_method`` is provided.
         kwargs : float
             Keyword arguments for the different initialization methods. See
             :meth:`~tensorkrowch.AbstractNode.make_tensor`.
         """
         if init_method == 'unit':
             tensors = self._make_unitaries(device=device)
+        elif init_method == 'canonical':
+            tensors = self._make_canonical(device=device)
         
         if tensors is not None:
             self.uniform_memory.tensor = tensors[0]
             self.out_node.tensor = tensors[-1]
         
         elif init_method is not None:
             for i, node in enumerate([self.uniform_memory, self.out_node]):
@@ -2904,15 +3348,15 @@
         result = result.view(*result.shape[:-1], h_out, w_out)
         # batch_size (x out_channels ...) x height_out x width_out
 
         return result
 
 
 class ConvMPS(AbstractConvClass, MPS):  # MARK: ConvMPS
-    """
+    r"""
     Convolutional version of :class:`MPS`, where the input data is assumed to
     be a batch of images.
     
     Input data as well as initialization parameters are described in `torch.nn.Conv2d
     <https://pytorch.org/docs/stable/generated/torch.nn.Conv2d.html>`_.
 
     Parameters
@@ -3009,15 +3453,15 @@
     @property
     def in_channels(self) -> int:
         """Returns ``in_channels``. Same as ``phys_dim`` in :class:`MPS`."""
         return self._in_channels
 
     @property
     def kernel_size(self) -> Tuple[int, int]:
-        """
+        r"""
         Returns ``kernel_size``. Number of nodes is given by
         :math:`kernel\_size_0 \cdot kernel\_size_1`.
         """
         return self._kernel_size
 
     @property
     def stride(self) -> Tuple[int, int]:
@@ -3174,15 +3618,15 @@
     @property
     def in_channels(self) -> int:
         """Returns ``in_channels``. Same as ``phys_dim`` in :class:`MPS`."""
         return self._in_channels
 
     @property
     def kernel_size(self) -> Tuple[int, int]:
-        """
+        r"""
         Returns ``kernel_size``. Number of nodes is given by
         :math:`kernel\_size_0 \cdot kernel\_size_1`.
         """
         return self._kernel_size
 
     @property
     def stride(self) -> Tuple[int, int]:
@@ -3241,15 +3685,15 @@
         else:
             new_mps.uniform_memory.tensor = self.uniform_memory.tensor.clone()
         
         return new_mps
 
 
 class ConvMPSLayer(AbstractConvClass, MPSLayer):  # MARK: ConvMPSLayer
-    """
+    r"""
     Convolutional version of :class:`MPSLayer`, where the input data is assumed to
     be a batch of images.
     
     Input data as well as initialization parameters are described in `torch.nn.Conv2d
     <https://pytorch.org/docs/stable/generated/torch.nn.Conv2d.html>`_.
 
     Parameters
@@ -3364,15 +3808,15 @@
     @property
     def out_channels(self) -> int:
         """Returns ``out_channels``. Same as ``out_dim`` in :class:`MPSLayer`."""
         return self._out_channels
 
     @property
     def kernel_size(self) -> Tuple[int, int]:
-        """
+        r"""
         Returns ``kernel_size``. Number of nodes is given by
         :math:`kernel\_size_0 \cdot kernel\_size_1 + 1`.
         """
         return self._kernel_size
 
     @property
     def stride(self) -> Tuple[int, int]:
@@ -3435,15 +3879,15 @@
             for new_node, node in zip(new_mps._mats_env, self._mats_env):
                 new_node.tensor = node.tensor.clone()
         
         return new_mps
 
 
 class ConvUMPSLayer(AbstractConvClass, UMPSLayer):  # MARK: ConvUMPSLayer
-    """
+    r"""
     Convolutional version of :class:`UMPSLayer`, where the input data is assumed to
     be a batch of images.
     
     Input data as well as initialization parameters are described in `torch.nn.Conv2d
     <https://pytorch.org/docs/stable/generated/torch.nn.Conv2d.html>`_.
 
     Parameters
@@ -3551,15 +3995,15 @@
     @property
     def out_channels(self) -> int:
         """Returns ``out_channels``. Same as ``out_dim`` in :class:`UMPSLayer`."""
         return self._out_channels
 
     @property
     def kernel_size(self) -> Tuple[int, int]:
-        """
+        r"""
         Returns ``kernel_size``. Number of nodes is given by
         :math:`kernel\_size_0 \cdot kernel\_size_1 + 1`.
         """
         return self._kernel_size
 
     @property
     def stride(self) -> Tuple[int, int]:
```

### Comparing `tensorkrowch-1.1.0/tensorkrowch/models/mps_data.py` & `tensorkrowch-1.1.1/tensorkrowch/models/mps_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -369,15 +369,14 @@
             :meth:`~tensorkrowch.AbstractNode.make_tensor`.
         """
         if self._boundary == 'obc':
             self._left_node.set_tensor(init_method='copy', device=device)
             self._right_node.set_tensor(init_method='copy', device=device)
                 
         if init_method is not None:
-                
             for i, node in enumerate(self._mats_env):
                 node.set_tensor(init_method=init_method,
                                 device=device,
                                 **kwargs)
                 
                 if self._boundary == 'obc':
                     aux_tensor = torch.zeros(*node.shape, device=device)
@@ -431,32 +430,45 @@
                     raise ValueError(
                         f'Physical dimension {data_tensor.shape[-2]} of '
                         f'data tensor at position {i} does not coincide '
                         f'with the corresponding physical dimension '
                         f'{node.shape[-2]} of the MPS')
         
         data = data[:]
+        device = data[0].device
         for i, node in enumerate(self._mats_env):
             if self._boundary == 'obc':
-                aux_tensor = torch.zeros(*node.shape,
-                                         device=data[i].device)
+                aux_tensor = torch.zeros(*node.shape, device=device)
                 if (i == 0) and (i == (self._n_features - 1)):
                     aux_tensor = torch.zeros(*data[i].shape[:-1],
                                              *node.shape[-3:],
-                                             device=data[i].device)
+                                             device=device)
                     aux_tensor[..., 0, :, 0] = data[i]
                     data[i] = aux_tensor
                 elif i == 0:
                     aux_tensor = torch.zeros(*data[i].shape[:-2],
                                              *node.shape[-3:-1],
                                              data[i].shape[-1],
-                                             device=data[i].device)
+                                             device=device)
                     aux_tensor[..., 0, :, :] = data[i]
                     data[i] = aux_tensor
                 elif i == (self._n_features - 1):
                     aux_tensor = torch.zeros(*data[i].shape[:-1],
                                              *node.shape[-2:],
-                                             device=data[i].device)
+                                             device=device)
                     aux_tensor[..., 0] = data[i]
                     data[i] = aux_tensor
                     
-            node._direct_set_tensor(data[i])
+            node._direct_set_tensor(data[i])
+        
+        # Send left and right nodes to correct device
+        if self._boundary == 'obc':
+            if self._left_node.device != device:
+                self._left_node.tensor = self._left_node.tensor.to(device)
+            if self._right_node.device != device:
+                self._right_node.tensor = self._right_node.tensor.to(device)
+        
+        # Update bond dim
+        if self._boundary == 'obc':
+            self._bond_dim = [node['right'].size() for node in self._mats_env[:-1]]
+        else:
+            self._bond_dim = [node['right'].size() for node in self._mats_env]
```

### Comparing `tensorkrowch-1.1.0/tensorkrowch/models/peps.py` & `tensorkrowch-1.1.1/tensorkrowch/models/peps.py`

 * *Files 0% similar despite different names*

```diff
@@ -1272,15 +1272,15 @@
     @property
     def in_channels(self) -> int:
         """Returns ``in_channels``. Same as ``in_dim`` in :class:`PEPS`."""
         return self._in_channels
 
     @property
     def kernel_size(self) -> Tuple[int, int]:
-        """
+        r"""
         Returns ``kernel_size``. Number of rows and columns in the 2D grid is
         given by :math:`kernel\_size_0` and :math:`kernel\_size_1`, respectively.
         """
         return self._kernel_size
 
     @property
     def stride(self) -> Tuple[int, int]:
@@ -1450,15 +1450,15 @@
     @property
     def in_channels(self) -> int:
         """Returns ``in_channels``. Same as ``in_dim`` in :class:`UPEPS`."""
         return self._in_channels
 
     @property
     def kernel_size(self) -> Tuple[int, int]:
-        """
+        r"""
         Returns ``kernel_size``. Number of rows and columns in the 2D grid is
         given by :math:`kernel\_size_0` and :math:`kernel\_size_1`, respectively.
         """
         return self._kernel_size
 
     @property
     def stride(self) -> Tuple[int, int]:
```

### Comparing `tensorkrowch-1.1.0/tensorkrowch/models/tree.py` & `tensorkrowch-1.1.1/tensorkrowch/models/tree.py`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.1.0/tensorkrowch/operations.py` & `tensorkrowch-1.1.1/tensorkrowch/operations.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         * unbind
         * einsum
         * stacked_einsum
 """
 
 import types
 from typing import Callable
+from numbers import Number
 
 from itertools import starmap
 import opt_einsum
 
 from tensorkrowch.components import *
 from tensorkrowch.utils import (inverse_permutation, is_permutation,
                                 list2slice, permute_list)
@@ -396,15 +397,15 @@
 
 
 def _tprod_next(successor: Successor,
                 node1: AbstractNode,
                 node2: AbstractNode) -> Node:
     tensor1 = node1._direct_get_tensor(successor.node_ref[0],
                                        successor.index[0])
-    tensor2 = node1._direct_get_tensor(successor.node_ref[1],
+    tensor2 = node2._direct_get_tensor(successor.node_ref[1],
                                        successor.index[1])
     new_tensor = torch.outer(tensor1.flatten(),
                              tensor2.flatten()).view(*(list(node1._shape) + 
                                                        list(node2._shape)))
     child = successor.child
     child._direct_set_tensor(new_tensor)
 
@@ -484,413 +485,980 @@
 
 AbstractNode.__mod__ = tprod_node
 
 
 ###################################   MUL    ##################################
 # MARK: mul
 def _check_first_mul(node1: AbstractNode,
-                     node2: AbstractNode) -> Optional[Successor]:
-    args = (node1, node2)
+                     node2: Union[AbstractNode,
+                                  torch.Tensor,
+                                  Number]) -> Optional[Successor]:
+    if isinstance(node2, AbstractNode):
+        args = (node1, node2)
+    else:
+        args = (node1,)
     successors = node1._successors.get('mul')
     if not successors:
         return None
     return successors.get(args)
 
 
-def _mul_first(node1: AbstractNode, node2: AbstractNode) -> Node:
-    if node1._network != node2._network:
-        raise ValueError('Nodes must be in the same network')
+def _mul_first(node1: AbstractNode,
+               node2: Union[AbstractNode,
+                            torch.Tensor,
+                            Number]) -> Node:
+    is_node2 = False
+    if isinstance(node2, AbstractNode):
+        is_node2 = True
+        if node1._network != node2._network:
+            raise ValueError('Nodes must be in the same network')
 
-    new_tensor = node1.tensor * node2.tensor
+    if is_node2:
+        new_tensor = node1.tensor * node2.tensor
+    else:
+        new_tensor = node1.tensor * node2
+    
     new_node = Node._create_resultant(axes_names=node1.axes_names,
                                       name='mul',
                                       network=node1._network,
                                       tensor=new_tensor,
                                       edges=node1._edges,
                                       node1_list=node1.is_node1())
 
     # Create successor
     net = node1._network
-    args = (node1, node2)
-    successor = Successor(node_ref=(node1.node_ref(),
-                                    node2.node_ref()),
-                          index=(node1._tensor_info['index'],
-                                 node2._tensor_info['index']),
-                          child=new_node)
+    
+    if is_node2:
+        args = (node1, node2)
+        successor = Successor(node_ref=(node1.node_ref(),
+                                        node2.node_ref()),
+                              index=(node1._tensor_info['index'],
+                                     node2._tensor_info['index']),
+                              child=new_node,
+                              hints=is_node2)
+    else:
+        args = (node1,)
+        successor = Successor(node_ref=(node1.node_ref(),),
+                              index=(node1._tensor_info['index'],),
+                              child=new_node,
+                              hints=is_node2)
 
     # Add successor to parent
     if 'mul' in node1._successors:
         node1._successors['mul'].update({args: successor})
     else:
         node1._successors['mul'] = {args: successor}
 
     # Add operation to list of performed operations of TN
     net._seq_ops.append(('mul', args))
 
     # Record in inverse_memory while tracing
     if net._tracing:
         node1._record_in_inverse_memory()
-        node2._record_in_inverse_memory()
+        
+        if is_node2:
+            node2._record_in_inverse_memory()
 
     return new_node
 
 
 def _mul_next(successor: Successor,
               node1: AbstractNode,
-              node2: AbstractNode) -> Node:
+              node2: Union[AbstractNode,
+                           torch.Tensor,
+                           Number]) -> Node:
+    is_node2 = successor.hints
     tensor1 = node1._direct_get_tensor(successor.node_ref[0],
                                        successor.index[0])
-    tensor2 = node1._direct_get_tensor(successor.node_ref[1],
-                                       successor.index[1])
+    if is_node2:
+        tensor2 = node2._direct_get_tensor(successor.node_ref[1],
+                                           successor.index[1])
+    else:
+        tensor2 = node2
+    
     new_tensor = tensor1 * tensor2
     child = successor.child
     child._direct_set_tensor(new_tensor)
 
     # Record in inverse_memory while contracting, if network is traced
     # (to delete memory if possible)
     if node1._network._traced:
-        node1._check_inverse_memory(successor.node_ref)
-        node2._check_inverse_memory(successor.node_ref)
-
+        node1._check_inverse_memory(successor.node_ref[0])
+        
+        if is_node2:
+            node2._check_inverse_memory(successor.node_ref[1])
+    
     return child
 
 
 mul_op = Operation('mul', _check_first_mul, _mul_first, _mul_next)
 
 
-def mul(node1: AbstractNode, node2: AbstractNode) -> Node:
+def mul(node1: AbstractNode,
+        node2: Union[AbstractNode,
+                     torch.Tensor,
+                     Number]) -> Node:
     """
     Element-wise product between two nodes. It can also be performed using the
     operator ``*``.
     
+    It also admits to take as ``node2`` a number or tensor, that will be
+    multiplied by the ``node1`` tensor as ``node1.tensor * node2``. If this
+    is used like this in the :meth:`~tensorkrowch.TensorNetwork.contract` method
+    of a  :class:`~tensorkrowch.TensorNetwork`, this will have to be called
+    explicitly to contract the network, rather than relying on its internal
+    call via the :meth:`~tensorkrowch.TensorNetwork.forward`.
+    
     Nodes ``resultant`` from this operation are called ``"mul"``. The node
     that keeps information about the :class:`Successor` is ``node1``.
 
     Parameters
     ----------
     node1 : Node or ParamNode
         First node to be multiplied. Its edges will appear in the resultant node.
-    node2 : Node or ParamNode
-        Second node to be multiplied.
+    node2 : Node, ParamNode, torch.Tensor or number
+        Second node to be multiplied. It can also be a number or tensor with
+        appropiate shape.
 
     Returns
     -------
     Node
     
     Examples
     --------
     >>> net = tk.TensorNetwork()
     >>> nodeA = tk.randn((2, 3), network=net)
     >>> nodeB = tk.randn((2, 3), network=net)
     >>> result = nodeA * nodeB
     >>> result.shape
     torch.Size([2, 3])
+    
+    >>> net = tk.TensorNetwork()
+    >>> nodeA = tk.randn((2, 3), network=net)
+    >>> tensorB = torch.randn(2, 3)
+    >>> result = nodeA * tensorB
+    >>> result.shape
+    torch.Size([2, 3])
     """
     return mul_op(node1, node2)
 
 
 mul_node = copy_func(mul)
 mul_node.__doc__ = \
     """
     Element-wise product between two nodes. It can also be performed using the
     operator ``*``.
     
+    It also admits to take as ``node2`` a number or tensor, that will be
+    multiplied by the ``self`` tensor as ``self.tensor * node2``. If this
+    is used like this in the :meth:`~tensorkrowch.TensorNetwork.contract` method
+    of a  :class:`~tensorkrowch.TensorNetwork`, this will have to be called
+    explicitly to contract the network, rather than relying on its internal
+    call via the :meth:`~tensorkrowch.TensorNetwork.forward`.
+    
     Nodes ``resultant`` from this operation are called ``"mul"``. The node
     that keeps information about the :class:`Successor` is ``self``.
 
     Parameters
     ----------
-    node2 : Node or ParamNode
-        Second node to be multiplied.
+    node2 : Node, ParamNode, torch.Tensor or number
+        Second node to be multiplied. It can also be a number or tensor with
+        appropiate shape.
 
     Returns
     -------
     Node
     
     Examples
     --------
     >>> net = tk.TensorNetwork()
     >>> nodeA = tk.randn((2, 3), network=net)
     >>> nodeB = tk.randn((2, 3), network=net)
     >>> result = nodeA.mul(nodeB)
     >>> result.shape
     torch.Size([2, 3])
+    
+    >>> net = tk.TensorNetwork()
+    >>> nodeA = tk.randn((2, 3), network=net)
+    >>> tensorB = torch.randn(2, 3)
+    >>> result = nodeA.mul(tensorB)
+    >>> result.shape
+    torch.Size([2, 3])
     """
 
 AbstractNode.__mul__ = mul_node
 
 
+###################################   DIV    ##################################
+# MARK: div
+def _check_first_div(node1: AbstractNode,
+                     node2: Union[AbstractNode,
+                                  torch.Tensor,
+                                  Number]) -> Optional[Successor]:
+    if isinstance(node2, AbstractNode):
+        args = (node1, node2)
+    else:
+        args = (node1,)
+    successors = node1._successors.get('div')
+    if not successors:
+        return None
+    return successors.get(args)
+
+
+def _div_first(node1: AbstractNode,
+               node2: Union[AbstractNode,
+                            torch.Tensor,
+                            Number]) -> Node:
+    is_node2 = False
+    if isinstance(node2, AbstractNode):
+        is_node2 = True
+        if node1._network != node2._network:
+            raise ValueError('Nodes must be in the same network')
+
+    if is_node2:
+        new_tensor = node1.tensor / node2.tensor
+    else:
+        new_tensor = node1.tensor / node2
+    
+    new_node = Node._create_resultant(axes_names=node1.axes_names,
+                                      name='div',
+                                      network=node1._network,
+                                      tensor=new_tensor,
+                                      edges=node1._edges,
+                                      node1_list=node1.is_node1())
+
+    # Create successor
+    net = node1._network
+    
+    if is_node2:
+        args = (node1, node2)
+        successor = Successor(node_ref=(node1.node_ref(),
+                                        node2.node_ref()),
+                              index=(node1._tensor_info['index'],
+                                     node2._tensor_info['index']),
+                              child=new_node,
+                              hints=is_node2)
+    else:
+        args = (node1,)
+        successor = Successor(node_ref=(node1.node_ref(),),
+                              index=(node1._tensor_info['index'],),
+                              child=new_node,
+                              hints=is_node2)
+
+    # Add successor to parent
+    if 'div' in node1._successors:
+        node1._successors['div'].update({args: successor})
+    else:
+        node1._successors['div'] = {args: successor}
+
+    # Add operation to list of performed operations of TN
+    net._seq_ops.append(('div', args))
+
+    # Record in inverse_memory while tracing
+    if net._tracing:
+        node1._record_in_inverse_memory()
+        
+        if is_node2:
+            node2._record_in_inverse_memory()
+
+    return new_node
+
+
+def _div_next(successor: Successor,
+              node1: AbstractNode,
+              node2: Union[AbstractNode,
+                           torch.Tensor,
+                           Number]) -> Node:
+    is_node2 = successor.hints
+    tensor1 = node1._direct_get_tensor(successor.node_ref[0],
+                                       successor.index[0])
+    if is_node2:
+        tensor2 = node2._direct_get_tensor(successor.node_ref[1],
+                                           successor.index[1])
+    else:
+        tensor2 = node2
+    
+    new_tensor = tensor1 / tensor2
+    child = successor.child
+    child._direct_set_tensor(new_tensor)
+
+    # Record in inverse_memory while contracting, if network is traced
+    # (to delete memory if possible)
+    if node1._network._traced:
+        node1._check_inverse_memory(successor.node_ref[0])
+        
+        if is_node2:
+            node2._check_inverse_memory(successor.node_ref[1])
+    
+    return child
+
+
+div_op = Operation('div', _check_first_div, _div_first, _div_next)
+
+
+def div(node1: AbstractNode,
+        node2: Union[AbstractNode,
+                     torch.Tensor,
+                     Number]) -> Node:
+    """
+    Element-wise division between two nodes. It can also be performed using the
+    operator ``/``.
+    
+    It also admits to take as ``node2`` a number or tensor, that will
+    divide the ``node1`` tensor as ``node1.tensor / node2``. If this
+    is used like this in the :meth:`~tensorkrowch.TensorNetwork.contract` method
+    of a  :class:`~tensorkrowch.TensorNetwork`, this will have to be called
+    explicitly to contract the network, rather than relying on its internal
+    call via the :meth:`~tensorkrowch.TensorNetwork.forward`.
+    
+    Nodes ``resultant`` from this operation are called ``"div"``. The node
+    that keeps information about the :class:`Successor` is ``node1``.
+
+    Parameters
+    ----------
+    node1 : Node or ParamNode
+        First node to be divided. Its edges will appear in the resultant node.
+    node2 : Node, ParamNode, torch.Tensor or number
+        Second node, the divisor. It can also be a number or tensor with
+        appropiate shape.
+
+    Returns
+    -------
+    Node
+    
+    Examples
+    --------
+    >>> net = tk.TensorNetwork()
+    >>> nodeA = tk.randn((2, 3), network=net)
+    >>> nodeB = tk.randn((2, 3), network=net)
+    >>> result = nodeA / nodeB
+    >>> result.shape
+    torch.Size([2, 3])
+    
+    >>> net = tk.TensorNetwork()
+    >>> nodeA = tk.randn((2, 3), network=net)
+    >>> tensorB = torch.randn(2, 3)
+    >>> result = nodeA / tensorB
+    >>> result.shape
+    torch.Size([2, 3])
+    """
+    return div_op(node1, node2)
+
+
+div_node = copy_func(div)
+div_node.__doc__ = \
+    """
+    Element-wise division between two nodes. It can also be performed using the
+    operator ``/``.
+    
+    It also admits to take as ``node2`` a number or tensor, that will
+    divide the ``self`` tensor as ``self.tensor / node2``. If this
+    is used like this in the :meth:`~tensorkrowch.TensorNetwork.contract` method
+    of a  :class:`~tensorkrowch.TensorNetwork`, this will have to be called
+    explicitly to contract the network, rather than relying on its internal
+    call via the :meth:`~tensorkrowch.TensorNetwork.forward`.
+    
+    Nodes ``resultant`` from this operation are called ``"div"``. The node
+    that keeps information about the :class:`Successor` is ``self``.
+
+    Parameters
+    ----------
+    node2 : Node, ParamNode, torch.Tensor or number
+        Second node, the divisor. It can also be a number or tensor with
+        appropiate shape.
+
+    Returns
+    -------
+    Node
+    
+    Examples
+    --------
+    >>> net = tk.TensorNetwork()
+    >>> nodeA = tk.randn((2, 3), network=net)
+    >>> nodeB = tk.randn((2, 3), network=net)
+    >>> result = nodeA.div(nodeB)
+    >>> result.shape
+    torch.Size([2, 3])
+    
+    >>> net = tk.TensorNetwork()
+    >>> nodeA = tk.randn((2, 3), network=net)
+    >>> tensorB = torch.randn(2, 3)
+    >>> result = nodeA.div(tensorB)
+    >>> result.shape
+    torch.Size([2, 3])
+    """
+
+AbstractNode.__truediv__ = div_node
+
+
 ###################################   ADD    ##################################
 # MARK: add
 def _check_first_add(node1: AbstractNode,
-                     node2: AbstractNode) -> Optional[Successor]:
-    args = (node1, node2)
+                     node2: Union[AbstractNode,
+                                  torch.Tensor,
+                                  Number]) -> Optional[Successor]:
+    if isinstance(node2, AbstractNode):
+        args = (node1, node2)
+    else:
+        args = (node1,)
     successors = node1._successors.get('add')
     if not successors:
         return None
     return successors.get(args)
 
 
-def _add_first(node1: AbstractNode, node2: AbstractNode) -> Node:
-    if node1._network != node2._network:
-        raise ValueError('Nodes must be in the same network')
+def _add_first(node1: AbstractNode,
+               node2: Union[AbstractNode,
+                            torch.Tensor,
+                            Number]) -> Node:
+    is_node2 = False
+    if isinstance(node2, AbstractNode):
+        is_node2 = True
+        if node1._network != node2._network:
+            raise ValueError('Nodes must be in the same network')
 
-    new_tensor = node1.tensor + node2.tensor
+    if is_node2:
+        new_tensor = node1.tensor + node2.tensor
+    else:
+        new_tensor = node1.tensor + node2
+    
     new_node = Node._create_resultant(axes_names=node1.axes_names,
                                       name='add',
                                       network=node1._network,
                                       tensor=new_tensor,
                                       edges=node1._edges,
                                       node1_list=node1.is_node1())
 
     # Create successor
     net = node1._network
-    args = (node1, node2)
-    successor = Successor(node_ref=(node1.node_ref(),
-                                    node2.node_ref()),
-                          index=(node1._tensor_info['index'],
-                                 node2._tensor_info['index']),
-                          child=new_node)
+    
+    if is_node2:
+        args = (node1, node2)
+        successor = Successor(node_ref=(node1.node_ref(),
+                                        node2.node_ref()),
+                              index=(node1._tensor_info['index'],
+                                     node2._tensor_info['index']),
+                              child=new_node,
+                              hints=is_node2)
+    else:
+        args = (node1,)
+        successor = Successor(node_ref=(node1.node_ref(),),
+                              index=(node1._tensor_info['index'],),
+                              child=new_node,
+                              hints=is_node2)
 
     # Add successor to parent
     if 'add' in node1._successors:
         node1._successors['add'].update({args: successor})
     else:
         node1._successors['add'] = {args: successor}
 
     # Add operation to list of performed operations of TN
     net._seq_ops.append(('add', args))
 
     # Record in inverse_memory while tracing
     if net._tracing:
         node1._record_in_inverse_memory()
-        node2._record_in_inverse_memory()
+        
+        if is_node2:
+            node2._record_in_inverse_memory()
 
     return new_node
 
 
 def _add_next(successor: Successor,
               node1: AbstractNode,
-              node2: AbstractNode) -> Node:
+              node2: Union[AbstractNode,
+                           torch.Tensor,
+                           Number]) -> Node:
+    is_node2 = successor.hints
     tensor1 = node1._direct_get_tensor(successor.node_ref[0],
                                        successor.index[0])
-    tensor2 = node1._direct_get_tensor(successor.node_ref[1],
-                                       successor.index[1])
+    if is_node2:
+        tensor2 = node2._direct_get_tensor(successor.node_ref[1],
+                                           successor.index[1])
+    else:
+        tensor2 = node2
+    
     new_tensor = tensor1 + tensor2
     child = successor.child
     child._direct_set_tensor(new_tensor)
 
     # Record in inverse_memory while contracting, if network is traced
     # (to delete memory if possible)
     if node1._network._traced:
-        node1._check_inverse_memory(successor.node_ref)
-        node2._check_inverse_memory(successor.node_ref)
+        node1._check_inverse_memory(successor.node_ref[0])
+        
+        if is_node2:
+            node2._check_inverse_memory(successor.node_ref[1])
 
     return child
 
 
 add_op = Operation('add', _check_first_add, _add_first, _add_next)
 
 
-def add(node1: AbstractNode, node2: AbstractNode) -> Node:
+def add(node1: AbstractNode,
+        node2: Union[AbstractNode,
+                     torch.Tensor,
+                     Number]) -> Node:
     """
     Element-wise addition between two nodes. It can also be performed using the
     operator ``+``.
     
+    It also admits to take as ``node2`` a number or tensor, that will be
+    added to the ``node1`` tensor as ``node1.tensor + node2``. If this
+    is used like this in the :meth:`~tensorkrowch.TensorNetwork.contract` method
+    of a  :class:`~tensorkrowch.TensorNetwork`, this will have to be called
+    explicitly to contract the network, rather than relying on its internal
+    call via the :meth:`~tensorkrowch.TensorNetwork.forward`.
+    
     Nodes ``resultant`` from this operation are called ``"add"``. The node
     that keeps information about the :class:`Successor` is ``node1``.
 
     Parameters
     ----------
     node1 : Node or ParamNode
         First node to be added. Its edges will appear in the resultant node.
-    node2 : Node or ParamNode
-        Second node to be added.
+    node2 : Node, ParamNode, torch.Tensor or numeric
+        Second node to be added. It can also be a number or tensor with
+        appropiate shape.
 
     Returns
     -------
     Node
     
     Examples
     --------
     >>> net = tk.TensorNetwork()
     >>> nodeA = tk.randn((2, 3), network=net)
     >>> nodeB = tk.randn((2, 3), network=net)
     >>> result = nodeA + nodeB
     >>> result.shape
     torch.Size([2, 3])
+    
+    >>> net = tk.TensorNetwork()
+    >>> nodeA = tk.randn((2, 3), network=net)
+    >>> tensorB = torch.randn(2, 3)
+    >>> result = nodeA + tensorB
+    >>> result.shape
+    torch.Size([2, 3])
     """
     return add_op(node1, node2)
 
 
 add_node = copy_func(add)
 add_node.__doc__ = \
     """
     Element-wise addition between two nodes. It can also be performed using the
     operator ``+``.
     
+    It also admits to take as ``node2`` a number or tensor, that will be
+    added to the ``self`` tensor as ``self.tensor + node2``. If this
+    is used like this in the :meth:`~tensorkrowch.TensorNetwork.contract` method
+    of a  :class:`~tensorkrowch.TensorNetwork`, this will have to be called
+    explicitly to contract the network, rather than relying on its internal
+    call via the :meth:`~tensorkrowch.TensorNetwork.forward`.
+    
     Nodes ``resultant`` from this operation are called ``"add"``. The node
     that keeps information about the :class:`Successor` is ``self``.
 
     Parameters
     ----------
-    node2 : Node or ParamNode
-        Second node to be multiplied.
+    node2 : Node, ParamNode, torch.Tensor or number
+        Second node to be added. It can also be a number or tensor with
+        appropiate shape.
 
     Returns
     -------
     Node
     
     Examples
     --------
     >>> net = tk.TensorNetwork()
     >>> nodeA = tk.randn((2, 3), network=net)
     >>> nodeB = tk.randn((2, 3), network=net)
     >>> result = nodeA.add(nodeB)
     >>> result.shape
     torch.Size([2, 3])
+    
+    >>> net = tk.TensorNetwork()
+    >>> nodeA = tk.randn((2, 3), network=net)
+    >>> tensorB = torch.randn(2, 3)
+    >>> result = nodeA.add(tensorB)
+    >>> result.shape
+    torch.Size([2, 3])
     """
 
 AbstractNode.__add__ = add_node
 
 
 ###################################   SUB    ##################################
 # MARK: sub
 def _check_first_sub(node1: AbstractNode,
-                     node2: AbstractNode) -> Optional[Successor]:
-    args = (node1, node2)
+                     node2: Union[AbstractNode,
+                                  torch.Tensor,
+                                  Number]) -> Optional[Successor]:
+    if isinstance(node2, AbstractNode):
+        args = (node1, node2)
+    else:
+        args = (node1,)
     successors = node1._successors.get('sub')
     if not successors:
         return None
     return successors.get(args)
 
 
-def _sub_first(node1: AbstractNode, node2: AbstractNode) -> Node:
-    if node1._network != node2._network:
-        raise ValueError('Nodes must be in the same network')
+def _sub_first(node1: AbstractNode,
+               node2: Union[AbstractNode,
+                            torch.Tensor,
+                            Number]) -> Node:
+    is_node2 = False
+    if isinstance(node2, AbstractNode):
+        is_node2 = True
+        if node1._network != node2._network:
+            raise ValueError('Nodes must be in the same network')
 
-    new_tensor = node1.tensor - node2.tensor
+    if is_node2:
+        new_tensor = node1.tensor - node2.tensor
+    else:
+        new_tensor = node1.tensor - node2
+    
     new_node = Node._create_resultant(axes_names=node1.axes_names,
                                       name='sub',
                                       network=node1._network,
                                       tensor=new_tensor,
                                       edges=node1._edges,
                                       node1_list=node1.is_node1())
 
     # Create successor
     net = node1._network
-    args = (node1, node2)
-    successor = Successor(node_ref=(node1.node_ref(),
-                                    node2.node_ref()),
-                          index=(node1._tensor_info['index'],
-                                 node2._tensor_info['index']),
-                          child=new_node)
+    
+    if is_node2:
+        args = (node1, node2)
+        successor = Successor(node_ref=(node1.node_ref(),
+                                        node2.node_ref()),
+                              index=(node1._tensor_info['index'],
+                                     node2._tensor_info['index']),
+                              child=new_node,
+                              hints=is_node2)
+    else:
+        args = (node1,)
+        successor = Successor(node_ref=(node1.node_ref(),),
+                              index=(node1._tensor_info['index'],),
+                              child=new_node,
+                              hints=is_node2)
 
     # Add successor to parent
     if 'sub' in node1._successors:
         node1._successors['sub'].update({args: successor})
     else:
         node1._successors['sub'] = {args: successor}
 
     # Add operation to list of performed operations of TN
     net._seq_ops.append(('sub', args))
 
     # Record in inverse_memory while tracing
     if net._tracing:
         node1._record_in_inverse_memory()
-        node2._record_in_inverse_memory()
+        
+        if is_node2:
+            node2._record_in_inverse_memory()
 
     return new_node
 
 
 def _sub_next(successor: Successor,
               node1: AbstractNode,
-              node2: AbstractNode) -> Node:
+              node2: Union[AbstractNode,
+                           torch.Tensor,
+                           Number]) -> Node:
+    is_node2 = successor.hints
     tensor1 = node1._direct_get_tensor(successor.node_ref[0],
                                        successor.index[0])
-    tensor2 = node1._direct_get_tensor(successor.node_ref[1],
-                                       successor.index[1])
+    if is_node2:
+        tensor2 = node2._direct_get_tensor(successor.node_ref[1],
+                                           successor.index[1])
+    else:
+        tensor2 = node2
+    
     new_tensor = tensor1 - tensor2
     child = successor.child
     child._direct_set_tensor(new_tensor)
 
     # Record in inverse_memory while contracting, if network is traced
     # (to delete memory if possible)
     if node1._network._traced:
-        node1._check_inverse_memory(successor.node_ref)
-        node2._check_inverse_memory(successor.node_ref)
+        node1._check_inverse_memory(successor.node_ref[0])
+        
+        if is_node2:
+            node2._check_inverse_memory(successor.node_ref[1])
 
     return child
 
 
 sub_op = Operation('sub', _check_first_sub, _sub_first, _sub_next)
 
 
-def sub(node1: AbstractNode, node2: AbstractNode) -> Node:
+def sub(node1: AbstractNode,
+        node2: Union[AbstractNode,
+                     torch.Tensor,
+                     Number]) -> Node:
     """
     Element-wise subtraction between two nodes. It can also be performed using
     the operator ``-``.
     
+    It also admits to take as ``node2`` a number or tensor, that will be
+    subtracted from the ``node1`` tensor as ``node1.tensor - node2``. If this
+    is used like this in the :meth:`~tensorkrowch.TensorNetwork.contract` method
+    of a  :class:`~tensorkrowch.TensorNetwork`, this will have to be called
+    explicitly to contract the network, rather than relying on its internal
+    call via the :meth:`~tensorkrowch.TensorNetwork.forward`.
+    
     Nodes ``resultant`` from this operation are called ``"sub"``. The node
     that keeps information about the :class:`Successor` is ``node1``.
 
     Parameters
     ----------
     node1 : Node or ParamNode
         First node, minuend . Its edges will appear in the resultant node.
-    node2 : Node or ParamNode
-        Second node, subtrahend.
+    node2 : Node, ParamNode, torch.Tensor or number
+        Second node, subtrahend. It can also be a number or tensor with
+        appropiate shape.
 
     Returns
     -------
     Node
     
     Examples
     --------
     >>> net = tk.TensorNetwork()
     >>> nodeA = tk.randn((2, 3), network=net)
     >>> nodeB = tk.randn((2, 3), network=net)
     >>> result = nodeA - nodeB
     >>> result.shape
     torch.Size([2, 3])
+    
+    >>> net = tk.TensorNetwork()
+    >>> nodeA = tk.randn((2, 3), network=net)
+    >>> tensorB = torch.randn(2, 3)
+    >>> result = nodeA - tensorB
+    >>> result.shape
+    torch.Size([2, 3])
     """
     return sub_op(node1, node2)
 
 
 sub_node = copy_func(sub)
 sub_node.__doc__ = \
     """
     Element-wise subtraction between two nodes. It can also be performed using
     the operator ``-``.
     
+    It also admits to take as ``node2`` a number or tensor, that will be
+    subtracted from the ``self`` tensor as ``self.tensor - node2``. If this
+    is used like this in the :meth:`~tensorkrowch.TensorNetwork.contract` method
+    of a  :class:`~tensorkrowch.TensorNetwork`, this will have to be called
+    explicitly to contract the network, rather than relying on its internal
+    call via the :meth:`~tensorkrowch.TensorNetwork.forward`.
+    
     Nodes ``resultant`` from this operation are called ``"sub"``. The node
     that keeps information about the :class:`Successor` is ``self``.
 
     Parameters
     ----------
-    node2 : Node or ParamNode
-        Second node, subtrahend.
+    node2 : Node, ParamNode, torch.Tensor or number
+        Second node, subtrahend. It can also be a number or tensor with
+        appropiate shape.
 
     Returns
     -------
     Node
     
     Examples
     --------
     >>> net = tk.TensorNetwork()
     >>> nodeA = tk.randn((2, 3), network=net)
     >>> nodeB = tk.randn((2, 3), network=net)
     >>> result = nodeA.sub(nodeB)
     >>> result.shape
     torch.Size([2, 3])
+    
+    >>> net = tk.TensorNetwork()
+    >>> nodeA = tk.randn((2, 3), network=net)
+    >>> tensorB = torch.randn(2, 3)
+    >>> result = nodeA.sub(tensorB)
+    >>> result.shape
+    torch.Size([2, 3])
     """
 
 AbstractNode.__sub__ = sub_node
 
 
+###############################   renormalize    ##############################
+# MARK: renormalize
+def _check_first_renormalize(
+    node: AbstractNode,
+    p: Union[int, float] = 2,
+    axis: Optional[Union[Ax, Sequence[Ax]]] = None) -> Optional[Successor]:
+    
+    if isinstance(axis, (tuple, list)):
+        axis = tuple(axis)
+    args = (node, p, axis)
+    successors = node._successors.get('renormalize')
+    if not successors:
+        return None
+    return successors.get(args)
+
+
+def _renormalize_first(
+    node: AbstractNode,
+    p: Union[int, float] = 2,
+    axis: Optional[Union[Ax, Sequence[Ax]]] = None) -> Node:
+    
+    axis_num = []
+    if axis is not None:
+        if isinstance(axis, (tuple, list)):
+            for ax in axis:
+                axis_num.append(node.get_axis_num(ax))
+            axis = tuple(axis)
+        else:
+            axis_num.append(node.get_axis_num(axis))
+    
+    norm = node.tensor.norm(p=p, dim=axis_num, keepdim=True)
+    new_tensor = node.tensor / norm
+    new_node = Node._create_resultant(axes_names=node.axes_names,
+                                      name='renormalize',
+                                      network=node._network,
+                                      tensor=new_tensor,
+                                      edges=node._edges,
+                                      node1_list=node.is_node1())
+
+    # Create successor
+    net = node._network
+    args = (node, p, axis)
+    successor = Successor(node_ref=node.node_ref(),
+                          index=node._tensor_info['index'],
+                          child=new_node,
+                          hints=axis_num)
+
+    # Add successor to parent
+    if 'renormalize' in node._successors:
+        node._successors['renormalize'].update({args: successor})
+    else:
+        node._successors['renormalize'] = {args: successor}
+
+    # Add operation to list of performed operations of TN
+    net._seq_ops.append(('renormalize', args))
+
+    # Record in inverse_memory while tracing
+    if net._tracing:
+        node._record_in_inverse_memory()
+
+    return new_node
+
+
+def _renormalize_next(
+    successor: Successor,
+    node: AbstractNode,
+    p: Union[int, float] = 2,
+    axis: Optional[Union[Ax, Sequence[Ax]]] = None) -> Node:
+    
+    axis_num = successor.hints
+    tensor = node._direct_get_tensor(successor.node_ref,
+                                     successor.index)
+    norm = tensor.norm(p=p, dim=axis_num, keepdim=True)
+    new_tensor = tensor / norm
+    
+    child = successor.child
+    child._direct_set_tensor(new_tensor)
+
+    # Record in inverse_memory while contracting, if network is traced
+    # (to delete memory if possible)
+    if node._network._traced:
+        node._check_inverse_memory(successor.node_ref)
+    
+    return child
+
+
+renormalize_op = Operation('renormalize',
+                           _check_first_renormalize,
+                           _renormalize_first,
+                           _renormalize_next)
+
+
+def renormalize(
+    node: AbstractNode,
+    p: Union[int, float] = 2,
+    axis: Optional[Union[Ax, Sequence[Ax]]] = None) -> Node:
+    """
+    Normalizes the node with the specified norm. That is, the tensor of ``node``
+    is divided by its norm.
+    
+    Different norms can be taken, specifying the argument ``p``, and accross
+    different dimensions, or node axes, specifying the argument ``axis``.
+    
+    See also `torch.norm() <https://pytorch.org/docs/stable/generated/torch.norm.html>`_.
+
+    Parameters
+    ----------
+    node : Node or ParamNode
+        Node that is to be renormalized.
+    p : int, float
+        The order of the norm.
+    axis : int, str, Axis or list[int, str or Axis], optional
+        Axis or sequence of axes over which to reduce.
+
+    Returns
+    -------
+    Node
+    
+    Examples
+    --------
+    >>> nodeA = tk.randn((3, 3))
+    >>> renormA = tk.renormalize(nodeA)
+    >>> renormA.norm()
+    tensor(1.)
+    """
+    return renormalize_op(node, p, axis)
+
+
+renormalize_node = copy_func(renormalize)
+renormalize_node.__doc__ = \
+    """
+    Normalizes the node with the specified norm. That is, the tensor of ``node``
+    is divided by its norm.
+    
+    Different norms can be taken, specifying the argument ``p``, and accross
+    different dimensions, or node axes, specifying the argument ``axis``.
+    
+    See also `torch.norm() <https://pytorch.org/docs/stable/generated/torch.norm.html>`_.
+
+    Parameters
+    ----------
+    p : int, float
+        The order of the norm.
+    axis : int, str, Axis or list[int, str or Axis], optional
+        Axis or sequence of axes over which to reduce.
+
+    Returns
+    -------
+    Node
+    
+    Examples
+    --------
+    >>> nodeA = tk.randn((3, 3))
+    >>> renormA = nodeA.renormalize()
+    >>> renormA.norm()
+    tensor(1.)
+    """
+
+AbstractNode.renormalize = renormalize_node
+
+
 ###############################################################################
 #                            NODE-LIKE OPERATIONS                             #
 ###############################################################################
 
 ##################################   SPLIT    #################################
 # MARK: split
 def _check_first_split(node: AbstractNode,
@@ -999,23 +1567,23 @@
         if cum_percentage is not None:
             s_percentages = s.cumsum(-1) / \
                 (s.sum(-1, keepdim=True).expand(s.shape) + 1e-10) # To avoid having all 0's
             cum_percentage_tensor = cum_percentage * torch.ones_like(s)
             cp_rank = torch.lt(
                 s_percentages,
                 cum_percentage_tensor
-                ).view(-1, s.shape[-1]).all(dim=0).sum()
+                ).view(-1, s.shape[-1]).any(dim=0).sum()
             lst_ranks.append(max(1, cp_rank.item() + 1))
             
         if cutoff is not None:
             cutoff_tensor = cutoff * torch.ones_like(s)
             co_rank = torch.ge(
                 s,
                 cutoff_tensor
-                ).view(-1, s.shape[-1]).all(dim=0).sum()
+                ).view(-1, s.shape[-1]).any(dim=0).sum()
             lst_ranks.append(max(1, co_rank.item()))
         
         # Select rank from specified restrictions
         rank = min(lst_ranks)
         
         u = u[..., :rank]
         s = s[..., :rank]
@@ -1198,23 +1766,23 @@
         if cum_percentage is not None:
             s_percentages = s.cumsum(-1) / \
                 (s.sum(-1, keepdim=True).expand(s.shape) + 1e-10) # To avoid having all 0's
             cum_percentage_tensor = cum_percentage * torch.ones_like(s)
             cp_rank = torch.lt(
                 s_percentages,
                 cum_percentage_tensor
-                ).view(-1, s.shape[-1]).all(dim=0).sum()
+                ).view(-1, s.shape[-1]).any(dim=0).sum()
             lst_ranks.append(max(1, cp_rank.item() + 1))
             
         if cutoff is not None:
             cutoff_tensor = cutoff * torch.ones_like(s)
             co_rank = torch.ge(
                 s,
                 cutoff_tensor
-                ).view(-1, s.shape[-1]).all(dim=0).sum()
+                ).view(-1, s.shape[-1]).any(dim=0).sum()
             lst_ranks.append(max(1, co_rank.item()))
         
         # Select rank from specified restrictions
         rank = min(lst_ranks)
         
         u = u[..., :rank]
         s = s[..., :rank]
@@ -1660,14 +2228,18 @@
         rank: Optional[int] = None,
         cum_percentage: Optional[float] = None,
         cutoff: Optional[float] = None) -> Tuple[Node, Node]:
     r"""
     Contracts an edge via :func:`contract` and splits it via :func:`split`
     using ``mode = "svd"``. See :func:`split` for a more complete explanation.
     
+    This only works if the nodes connected through the edge are ``leaf`` nodes.
+    Otherwise, this will perform the contraction between the ``leaf`` nodes
+    that were connected through this edge.
+    
     This operation is the same as :meth:`~Edge.svd`.
 
     Parameters
     ----------
     edge : Edge
         Edge whose nodes are to be contracted and split.
     side : str, optional
@@ -1783,14 +2355,18 @@
 
 svd_edge = copy_func(svd)
 svd_edge.__doc__ = \
     r"""
     Contracts an edge via :meth:`~Edge.contract` and splits it via
     :meth:`~AbstractNode.split` using ``mode = "svd"``. See :func:`split` for
     a more complete explanation.
+    
+    This only works if the nodes connected through the edge are ``leaf`` nodes.
+    Otherwise, this will perform the contraction between the ``leaf`` nodes
+    that were connected through this edge.
 
     Parameters
     ----------
     side : str, optional
         Indicates the side to which the diagonal matrix :math:`S` should be
         contracted. If "left", the first resultant node's tensor will be
         :math:`US`, and the other node's tensor will be :math:`V^{\dagger}`.
@@ -2053,14 +2629,18 @@
          rank: Optional[int] = None,
          cum_percentage: Optional[float] = None,
          cutoff: Optional[float] = None) -> Tuple[Node, Node]:
     r"""
     Contracts an edge via :func:`contract` and splits it via :func:`split`
     using ``mode = "svdr"``. See :func:`split` for a more complete explanation.
     
+    This only works if the nodes connected through the edge are ``leaf`` nodes.
+    Otherwise, this will perform the contraction between the ``leaf`` nodes
+    that were connected through this edge.
+    
     This operation is the same as :meth:`~Edge.svdr`.
 
     Parameters
     ----------
     edge : Edge
         Edge whose nodes are to be contracted and split.
     side : str, optional
@@ -2176,14 +2756,18 @@
 
 svdr_edge = copy_func(svdr)
 svdr_edge.__doc__ = \
     r"""
     Contracts an edge via :meth:`~Edge.contract` and splits it via
     :meth:`~AbstractNode.split` using ``mode = "svdr"``. See :func:`split` for
     a more complete explanation.
+    
+    This only works if the nodes connected through the edge are ``leaf`` nodes.
+    Otherwise, this will perform the contraction between the ``leaf`` nodes
+    that were connected through this edge.
 
     Parameters
     ----------
     side : str, optional
         Indicates the side to which the diagonal matrix :math:`S` should be
         contracted. If "left", the first resultant node's tensor will be
         :math:`US`, and the other node's tensor will be :math:`V^{\dagger}`.
@@ -2442,14 +3026,18 @@
 
 
 def qr(edge: Edge) -> Tuple[Node, Node]:
     r"""
     Contracts an edge via :func:`contract` and splits it via :func:`split`
     using ``mode = "qr"``. See :func:`split` for a more complete explanation.
     
+    This only works if the nodes connected through the edge are ``leaf`` nodes.
+    Otherwise, this will perform the contraction between the ``leaf`` nodes
+    that were connected through this edge.
+    
     This operation is the same as :meth:`~Edge.qr`.
 
     Parameters
     ----------
     edge : Edge
         Edge whose nodes are to be contracted and split.
 
@@ -2543,14 +3131,18 @@
 
 qr_edge = copy_func(qr)
 qr_edge.__doc__ = \
     r"""
     Contracts an edge via :meth:`~Edge.contract` and splits it via
     :meth:`~AbstractNode.split` using ``mode = "qr"``. See :func:`split` for
     a more complete explanation.
+    
+    This only works if the nodes connected through the edge are ``leaf`` nodes.
+    Otherwise, this will perform the contraction between the ``leaf`` nodes
+    that were connected through this edge.
 
     Returns
     -------
     tuple[Node, Node]
     
     Examples
     --------
@@ -2741,14 +3333,18 @@
 
 
 def rq(edge: Edge) -> Tuple[Node, Node]:
     r"""
     Contracts an edge via :func:`contract` and splits it via :func:`split`
     using ``mode = "rq"``. See :func:`split` for a more complete explanation.
     
+    This only works if the nodes connected through the edge are ``leaf`` nodes.
+    Otherwise, this will perform the contraction between the ``leaf`` nodes
+    that were connected through this edge.
+    
     This operation is the same as :meth:`~Edge.rq`.
 
     Parameters
     ----------
     edge : Edge
         Edge whose nodes are to be contracted and split.
 
@@ -2842,14 +3438,18 @@
 
 rq_edge = copy_func(rq)
 rq_edge.__doc__ = \
     r"""
     Contracts an edge via :meth:`~Edge.contract` and splits it via
     :meth:`~AbstractNode.split` using ``mode = "rq"``. See :func:`split` for
     a more complete explanation.
+    
+    This only works if the nodes connected through the edge are ``leaf`` nodes.
+    Otherwise, this will perform the contraction between the ``leaf`` nodes
+    that were connected through this edge.
 
     Returns
     -------
     tuple[Node, Node]
     
     Examples
     --------
@@ -3393,14 +3993,18 @@
     return contract_edges_op(edges, node1, node2)
 
 
 def contract(edge: Edge) -> Node:
     """
     Contracts the nodes that are connected through the edge.
     
+    This only works if the nodes connected through the edge are ``leaf`` nodes.
+    Otherwise, this will perform the contraction between the ``leaf`` nodes
+    that were connected through this edge.
+    
     Nodes ``resultant`` from this operation are called ``"contract_edges"``.
     The node that keeps information about the :class:`Successor` is
     ``edge.node1``.
     
     This operation is the same as :meth:`~Edge.contract`.
 
     Parameters
@@ -3432,14 +4036,18 @@
     return contract_edges_op([edge], edge.node1, edge.node2)
 
 contract_edge = copy_func(contract)
 contract_edge.__doc__ = \
     """
     Contracts the nodes that are connected through the edge.
     
+    This only works if the nodes connected through the edge are ``leaf`` nodes.
+    Otherwise, this will perform the contraction between the ``leaf`` nodes
+    that were connected through this edge.
+    
     Nodes ``resultant`` from this operation are called ``"contract_edges"``.
     The node that keeps information about the :class:`Successor` is
     ``self.node1``.
 
     Returns
     -------
     Node
@@ -4027,14 +4635,21 @@
 
     The stack dimension will be the first one in the ``resultant`` node.
     
     See :class:`ParamStackNode` and :class:`TensorNetwork` to learn how the
     :meth:`~TensorNetwork.auto_stack` mode affects the computation of
     :func:`stack`.
     
+    If this operation is used several times with the same input nodes, but their
+    dimensions can change from one call to another, this will lead to undesired
+    behaviour. The network should be :meth:`~tensorkrwoch.TensorNetwork.reset`.
+    This situation should be avoided in the
+    :meth:`~tensorkrowch.TensorNetwork.contract` method. Otherwise it will fail
+    in subsequent calls to ``contract`` or :meth:`~tensorkrowch.TensorNetwork.forward`
+    
     Nodes ``resultant`` from this operation are called ``"stack"``. If this
     operation returns a ``virtual`` :class:`ParamStackNode`, it will be called
     ``"virtual_result_stack"``. See :class:AbstractNode` to learn about this
     **reserved name**.  The node that keeps information about the
     :class:`Successor` is ``nodes[0]``, the first stacked node.
 
     Parameters
@@ -4565,15 +5180,15 @@
 einsum_op = Operation('einsum',
                       _check_first_einsum,
                       _einsum_first,
                       _einsum_next)
 
 
 def einsum(string: Text, *nodes: Sequence[AbstractNode]) -> Node:
-    """
+    r"""
     Performs einsum contraction based on `opt_einsum
     <https://optimized-einsum.readthedocs.io/en/stable/autosummary/opt_einsum.contract.html>`_.
     This operation facilitates contracting several nodes at once, specifying
     directly the order of appearance of the resultant edges. Without this
     operation, several contractions and permutations would be needed.
 
     Since it adapts a tensor operation for nodes, certain nodes' properties are
@@ -4630,15 +5245,15 @@
     """
     return einsum_op(string, *nodes)
 
 
 ##############################   STACKED EINSUM   #############################
 def stacked_einsum(string: Text,
                    *nodes_lists: List[AbstractNode]) -> List[Node]:
-    """
+    r"""
     Applies the same :func:`einsum` operation (same ``string``) to a sequence
     of groups of nodes (all groups having the same amount of nodes, with the
     same properties, etc.). That is, it stacks these groups of nodes into a
     single collection of ``StackNodes`` that is then contracted via
     :func:`einsum` (using the stack dimensions as **batch**), and
     :func:`unbound <unbind>` afterwards.
```

### Comparing `tensorkrowch-1.1.0/tensorkrowch/utils.py` & `tensorkrowch-1.1.1/tensorkrowch/utils.py`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.1.0/tensorkrowch.egg-info/PKG-INFO` & `tensorkrowch-1.1.1/tensorkrowch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorkrowch
-Version: 1.1.0
+Version: 1.1.1
 Summary: Tensor Networks with PyTorch
 Author-email: José Ramón Pareja Monturiol <joserapa98@gmail.com>
 Maintainer-email: José Ramón Pareja Monturiol <joserapa98@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 José Ramón Pareja Monturiol
```

### Comparing `tensorkrowch-1.1.0/tensorkrowch.egg-info/SOURCES.txt` & `tensorkrowch-1.1.1/tensorkrowch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

