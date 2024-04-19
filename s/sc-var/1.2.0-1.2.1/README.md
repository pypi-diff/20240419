# Comparing `tmp/sc_var-1.2.0.tar.gz` & `tmp/sc_var-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc_var-1.2.0.tar", max compression
+gzip compressed data, was "sc_var-1.2.1.tar", max compression
```

## Comparing `sc_var-1.2.0.tar` & `sc_var-1.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2024-01-03 08:29:55.804216 sc_var-1.2.0/LICENSE
--rw-r--r--   0        0        0      687 2024-01-09 08:50:22.201450 sc_var-1.2.0/README.md
--rw-r--r--   0        0        0      522 2024-01-09 08:50:48.606918 sc_var-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     6148 2024-01-04 07:23:38.014518 sc_var-1.2.0/sc_var/.DS_Store
--rw-r--r--   0        0        0       20 2024-01-09 08:42:43.329977 sc_var-1.2.0/sc_var/__init__.py
--rw-r--r--   0        0        0    22519 2024-01-09 08:45:07.736022 sc_var-1.2.0/sc_var/method.py
--rw-r--r--   0        0        0     1347 1970-01-01 00:00:00.000000 sc_var-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-01-03 08:29:55.804216 sc_var-1.2.1/LICENSE
+-rw-r--r--   0        0        0      726 2024-04-19 05:28:46.744761 sc_var-1.2.1/README.md
+-rw-r--r--   0        0        0      522 2024-04-19 05:35:47.637192 sc_var-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-01-04 07:23:38.014518 sc_var-1.2.1/sc_var/.DS_Store
+-rw-r--r--   0        0        0       20 2024-01-09 08:42:43.329977 sc_var-1.2.1/sc_var/__init__.py
+-rw-r--r--   0        0        0    28379 2024-04-19 05:21:46.169546 sc_var-1.2.1/sc_var/method.py
+-rw-r--r--   0        0        0     1386 1970-01-01 00:00:00.000000 sc_var-1.2.1/PKG-INFO
```

### Comparing `sc_var-1.2.0/LICENSE` & `sc_var-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sc_var-1.2.0/pyproject.toml` & `sc_var-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sc_var"
-version = "1.2.0"
+version = "1.2.1"
 description = "An approch for interpreting disease-associated human variants using single-cell epigenomics"
 authors = ["Gefei Z <gefeizhao@163.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 scanpy = "^1.9.6"
```

### Comparing `sc_var-1.2.0/sc_var/.DS_Store` & `sc_var-1.2.1/sc_var/.DS_Store`

 * *Files identical despite different names*

### Comparing `sc_var-1.2.0/sc_var/method.py` & `sc_var-1.2.1/sc_var/method.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # package load
 import os
 import sys
+import csv
 import numpy as np
 import pandas as pd
 import scanpy as sc
 import anndata
 import matplotlib.pyplot as plt
 import seaborn as sns
 import scipy
@@ -21,15 +22,76 @@
 
 
 
 
 #########################################################################################
 #####                                ANNOTATION                                    ######
 #########################################################################################
+   
+def read_gwas(gwas_file):
+    '''
+    Read GWAS data from txt file
+    GWAS file  should like 
+    chr pos rsids pval
+    if GWAS data from finn database
+    USE load_snp_list function
+    ''' 
+    snp_list=pd.read_csv(gwas_file,sep='\t')
+    snp_list['chr']=snp_list['chr'].astype(str)
+    snp_list['rsids'] = snp_list['rsids'].astype(str)
+    snp_list['pos'] = snp_list['pos'].astype(int)
+    snp_list.sort_values(['chr', 'pos'], inplace=True)
+    snp_list.reset_index(drop=True, inplace=True)
+    return snp_list
+    
+def load_snp_list(gwas_file):
+
+    '''
+    Load GWAS data from finn database
+    '''
+    
+    snp_list = pd.read_csv(gwas_file, 
+                            sep='\t',
+                            dtype={'#chrom':str,'pos':int,'rsids':str,'pval':float})
+    snp_list['chr']='chr'+ snp_list['#chrom']
+    snp_list=snp_list.drop(columns=['#chrom'])
+    #for rsids column split the data "," to two rows
+    snp_list=snp_list.assign(rsids=snp_list['rsids'].str.split(',')).explode('rsids')
+    snp_list[['rsids']]=snp_list['rsids'].str.split(',',expand=True)
+    #drop row with null rsid
+    snp_list=snp_list.dropna(subset=['rsids'],axis=0)
+    snp_list=snp_list.dropna(subset=['pval'],axis=0)
+    snp_list.sort_values(['chr', 'pos'], inplace=True)
+    snp_list.reset_index(drop=True, inplace=True)
+    #save snp_list as txt file named by phenotype
+    order=['chr','pos','rsids','pval']
+    snp_list=snp_list[order]
+    snp_list.to_csv(gwas_file,sep='\t',index=False)
+    
+    return snp_list    
+
+
+def load_peak_data(peak_file):
+
+    '''
+    Load peak to gene file from cicero
+    if only have co-accessibility link file from cicero
+    Use get_p2g_conn function to get peak to gene file
+    '''
+
+    peak_list = pd.read_csv(peak_file,sep='\t')
+    peak_list['chr'] = peak_list['chr'].astype(str)
+    peak_list['start'] = peak_list['start'] .astype(int)
+    peak_list['end'] = peak_list['end'].astype(int)
+    peak_list.sort_values(['chr', 'start', 'end'], ignore_index=True, inplace=True)
+    peak_list.reset_index(drop=True, inplace=True)
 
+    return peak_list
+    
+    
 def get_p2g_conn(cicero_conn,fdata):
     
     
     '''
     A function help to get the peak-gene conn from cicero_conn and cds fdata
 
     cicero_conn: output file from cicero conns 
@@ -77,60 +139,34 @@
     p2g['start']=p2g['Peak'].str.split('-').str[1]
     p2g['end']=p2g['Peak'].str.split('-').str[2]
     p2g=p2g[['gene','chr','start','end']]
     #get work path and save the result
     work_path=os.getcwd()
     p2g.to_csv(work_path+'/p2g_conn.txt',sep='\t',index=False)
     
-    return p2g
+    return p2g    
     
-    
-
-def annotate(overlap_matrix,gene_cor,dmagma_file,disease_name):
-    '''
-    Annotate GWAS SNPs with co_accessibility peaks with gene information
 
 
-    overlap_matrix: output from dis_peak function
-    gene_cor: output from gene_corr function
-    dmagma_file: output from dmagma function
-    disease_name: disease name interested from GWAS
+def multi_omics_p2g(p2g_file):
     '''
-    
-    gene_list=overlap_matrix.groupby('gene')['rsids'].apply(list).reset_index(name='snps')
-    gene_list=pd.merge(gene_list,gene_cor,on='gene',how='left')
-    gene_id=mg.querymany(gene_list['gene'], scopes='symbol', fields='entrezgene', species='human', as_dataframe=True)['entrezgene']
-    gene_id=gene_id.to_frame().reset_index()
-    gene_id.dropna(inplace=True)
-    gene_id=gene_id.rename(columns={'query':'gene'})
-    convert=pd.merge(gene_list,gene_id,on='gene',how='left')
-    convert.drop(columns=['gene'],inplace=True)
-    convert['snps']=convert['snps'].astype(str)
-    convert['snps']=convert['snps'].str.replace("nan","")
-    convert['snps']=convert['snps'].str.replace(',',' ')
-    convert['snps']=convert['snps'].str.replace('[','')
-    convert['snps']=convert['snps'].str.replace(']','')
-    convert['snps']=convert['snps'].str.replace("'","")
-    convert.dropna(inplace=True)
-    convert.dropna(subset=['g_cor'],inplace=True)
-    convert.rename(columns={'entrezgene':'GENE'},inplace=True)
+    Read multi omics peak to gene link file
+    which is output from signac LinkPeaks() function
+    '''
+    p2g=pd.read_csv(p2g_file,sep=',')
+    p2g=p2g[['gene','peak']]
+    p2g['chr']=p2g['peak'].str.split('-').str[0].astype(str)
+    p2g['start']=p2g['peak'].str.split('-').str[1].astype(int)
+    p2g['end']=p2g['peak'].str.split('-').str[2].astype(int)
+    p2g=p2g.drop('peak',axis=1)
+    p2g.sort_values(['chr', 'start', 'end'], ignore_index=True, inplace=True)
+    p2g.reset_index(drop=True, inplace=True)
+    return p2g  
 
-    cmagma=pd.merge(dmagma_file,convert,on='GENE',how='outer')
-    cmagma['POS']=cmagma['POS'].fillna(cmagma['g_cor'])
-    cmagma['SNPs']=cmagma['SNPs'].astype(str)
-    cmagma['snps']=cmagma['snps'].astype(str)
-    cmagma['SNPs'] = cmagma.apply(lambda x: str(x['SNPs']) + ' ' + str(x['snps']), axis=1)
-    cmagma['SNPs']=cmagma['SNPs'].str.replace('nan',' ')
-    cmagma=cmagma[['GENE','POS','SNPs']]
 
-    cmagma_annot=open(disease_name+'cmagma.genes.annot','w')
-    cmagma_annot.write(convert.to_string(index=False,header=False))
-    cmagma_annot.close()
-    
-    return cmagma
 
 
 
 
 
 def dmagma(magma_file):
 
@@ -151,14 +187,15 @@
     dmagma[['GENE','POS','SNPs']]=dmagma['content'].str.split(n=2,expand=True)
     dmagma.drop(columns=['content'],inplace=True)
     dmagma['SNPs']=dmagma['SNPs'].str.replace('\t',' ')
     dmagma['SNPs']=dmagma['SNPs'].str.split()
     dmagma['SNPs']=dmagma['SNPs'].apply(lambda x: list(set(x)))
     dmagma['SNPs']=dmagma['SNPs'].astype(str)
     dmagma['SNPs']=dmagma['SNPs'].str.replace('\[|\]|\'','')
+    dmagma['SNPs'] = dmagma['SNPs'].str.replace('[', '').str.replace(']', '').str.replace("'", '')
     dmagma['SNPs']=dmagma['SNPs'].str.replace(',',' ')
     return dmagma
 
 
 def snp_peak(peak_list, snp_list):
 
     '''
@@ -291,19 +328,83 @@
     output.close()
     
     return merge_annotate
 
 
 
 
+
+def annotate(overlap_matrix,gene_cor,dmagma_file,disease_name):
+    '''
+    Annotate GWAS SNPs with co_accessibility peaks with gene information
+
+
+    overlap_matrix: output from dis_peak function
+    gene_cor: output from gene_corr function
+    dmagma_file: output from dmagma function
+    disease_name: disease name interested from GWAS
+    '''
+    
+    gene_list=overlap_matrix.groupby('gene')['rsids'].apply(list).reset_index(name='snps')
+    gene_list=pd.merge(gene_list,gene_cor,on='gene',how='left')
+    gene_id=mg.querymany(gene_list['gene'], scopes='symbol', fields='entrezgene', species='human', as_dataframe=True)['entrezgene']
+    gene_id=gene_id.to_frame().reset_index()
+    gene_id.dropna(inplace=True)
+    gene_id=gene_id.rename(columns={'query':'gene'})
+    convert=pd.merge(gene_list,gene_id,on='gene',how='left')
+    convert.drop(columns=['gene'],inplace=True)
+    convert['snps']=convert['snps'].astype(str)
+    convert['snps']=convert['snps'].str.replace("nan","")
+    convert['snps']=convert['snps'].str.replace(',',' ')
+    convert['snps']=convert['snps'].str.replace('[','')
+    convert['snps']=convert['snps'].str.replace(']','')
+    convert['snps']=convert['snps'].str.replace("'","")
+    convert.dropna(inplace=True)
+    convert.dropna(subset=['g_cor'],inplace=True)
+    convert.rename(columns={'entrezgene':'GENE'},inplace=True)
+
+    cmagma=pd.merge(dmagma_file,convert,on='GENE',how='outer')
+    cmagma['POS']=cmagma['POS'].fillna(cmagma['g_cor'])
+    cmagma['SNPs']=cmagma['SNPs'].astype(str)
+    cmagma['snps']=cmagma['snps'].astype(str)
+    cmagma['SNPs'] = cmagma.apply(lambda x: str(x['SNPs']) + ' ' + str(x['snps']), axis=1)
+    cmagma['SNPs']=cmagma['SNPs'].str.replace('nan',' ')
+    cmagma=cmagma[['GENE','POS','SNPs']]
+    cmagma.to_csv(disease_name+'cmagma.genes.annot',index=False,header=False,sep='\t',quoting=csv.QUOTE_NONE)
+    return cmagma
+
+
+
+def save_dict_gs(gs_path: str, dict_gs: dict) -> None:
+    """
+    Save dict_gs to gs file (.gs file).
+    df_gs: Dict = {
+        "TRAIT": [],
+        "GENESET": [],}
+    """
+    df_gs: Dict = {
+        "TRAIT": [],
+        "GENESET": [],
+    }
+    for trait in dict_gs:
+        df_gs["TRAIT"].append(trait)
+        if isinstance(dict_gs[trait], tuple):
+            df_gs["GENESET"].append(
+                ",".join([str(g) + ":" + str(w) for g, w in zip(*dict_gs[trait])])
+            )
+        else:
+            df_gs["GENESET"].append(",".join(dict_gs[trait]))
+    pd.DataFrame(df_gs).to_csv(gs_path, sep="\t", index=False)
+    
+
 def save_gs(gene_file,disease_name,gs_path):
 
     '''
     OPTIONAL
-    Save gene analysis results as .gs file
+    Directly save cmagma gene analysis results into .gs file
 
     gene_file: gene analysis results from cmagma  rename to txt file
     disease_name: disease name interested from GWAS
     gs_path: output path for .gs file
 
     '''
     gene_file=pd.read_csv(gene_file,sep=r'\s+')
@@ -323,15 +424,15 @@
         "TRAIT": [],
         "GENESET": [],
     }
     for trait in dict_gs:
         df_gs["TRAIT"].append(trait)
         if isinstance(dict_gs[trait], tuple):
             df_gs["GENESET"].append(
-                ",".join([g + ":" + str(w) for g, w in zip(*dict_gs[trait])])
+                ",".join([str(g) + ":" + str(w) for g, w in zip(*dict_gs[trait])])
             )
         else:
             df_gs["GENESET"].append(",".join(dict_gs[trait]))
     pd.DataFrame(df_gs).to_csv(gs_path, sep="\t", index=False)
 
 
 
@@ -341,74 +442,116 @@
 #########################################################################################
 #####                                SCORING                                       ######
 #########################################################################################
 
 def get_peak_weights(overlap_matrix):
 
     '''
-    OPTIONAL
     For each peak, determine the lowest p-value of all SNPs that overlap with it.
     '''
 
     peak_weights = overlap_matrix.groupby(['chr', 'start', 'end']).agg({'pval': 'min'})
+    #if min p is 0, replace it with 1e-10
+    peak_weights['pval']=peak_weights['pval'].replace(0,1e-10)
     overlap_matrix['zscore']= np.abs(scipy.stats.norm.ppf(overlap_matrix['pval']/ 2))
     #keep zcore corresponding to min p
     peak_weights=pd.merge(peak_weights,overlap_matrix[['chr','start','end','zscore']],on=['chr','start','end'],how='left')
     peak_weights.reset_index(inplace=True)
     peak_weights.rename({'zscore': 'weight'}, axis=1, inplace=True)
-    peak_weights['GENE']='chr'+peak_weights['chr'].astype(str)+'-'+peak_weights['start'].astype(str)+'-'+peak_weights['end'].astype(str)
+    peak_weights['GENE']=peak_weights['chr'].astype(str)+'-'+peak_weights['start'].astype(str)+'-'+peak_weights['end'].astype(str)
 
     peak_weights.sort_values(['weight'],ascending=False,inplace=True)
     peak_weights.drop_duplicates(subset=['GENE'],keep='first',inplace=True)
     peak_weights=peak_weights[['GENE','weight']]
     return peak_weights
 
+def load_genes(gene_file):
+    gene_file=pd.read_csv(gene_file,sep=r'\s+')
+    gene_id=mg.querymany(gene_file['GENE'], scopes='entrezgene', fields='symbol', species='human', as_dataframe=True)['symbol']
+    gene_id=pd.DataFrame(gene_id)
+    gene_id=gene_id.reset_index('query')
+    gene_id=gene_id.rename(columns={'query':'GENE'})
+    gene_id['GENE']=gene_id['GENE'].astype('str')
+    gene_file['GENE']=gene_file['GENE'].astype('str')
+    gene_file=pd.merge(gene_file,gene_id,on='GENE',how='left')
+    return gene_file
 
+def drop_dup(gene_file):
+    gene_file=gene_file.sort_values(by='P')
+    gene_file=gene_file.drop_duplicates(subset='symbol',keep='first')
+    return gene_file
 
 
-
-
-def scads(adata,overlap_matrix,disease_name):
+def scads_atac(adata,overlap_matrix,cmagma_result,disease_name):
 
     '''
     adata: AnnData object
+    
+    overlap_matrix: output from snp_peak function
     For each peak, determine the lowest p-value of all SNPs that overlap with it.
     peak_weights can also get from get_peak_weights function 
+    
+    cmagma_result: output from cmagma pipline gene analysis results
+    see /magma \ --bfile /g1000_eur \--pval {gwas} use='rsids,pval' N=n\
+    --gene-annot {output from annotate fuction *.cmagma.genes.annot} \--out outfile
+    
     disease_name: disease name interested from GWAS
 
     '''
-
-    peak_weights = overlap_matrix.groupby(['chr', 'start', 'end']).agg({'pval': 'min'})
-    overlap_matrix['zscore']= np.abs(scipy.stats.norm.ppf(overlap_matrix['pval']/ 2))
-    #keep zcore corresponding to min p
-    peak_weights=pd.merge(peak_weights,overlap_matrix[['chr','start','end','zscore']],on=['chr','start','end'],how='left')
-    peak_weights.reset_index(inplace=True)
-    peak_weights.rename({'zscore': 'weight'}, axis=1, inplace=True)
-    peak_weights['GENE']='chr'+peak_weights['chr'].astype(str)+'-'+peak_weights['start'].astype(str)+'-'+peak_weights['end'].astype(str)
-
-    peak_weights.sort_values(['weight'],ascending=False,inplace=True)
-    peak_weights.drop_duplicates(subset=['GENE'],keep='first',inplace=True)
-    peak_weights=peak_weights[['GENE','weight']]
-
-    dict_gs = {disease_name: (peak_weights['GENE'].tolist(), peak_weights['weight'].tolist())}
+    cmagma_gene=load_genes(cmagma_result)
+    cmagma_gene=drop_dup(cmagma_gene)
+    cmagma_gene_sig=cmagma_gene[cmagma_gene['P']<0.05]
+    overlap_matrix=overlap_matrix[overlap_matrix['gene'].isin(cmagma_gene_sig['symbol'])]
+    
+    peak_weights = get_peak_weights(overlap_matrix)
+    peak_weights=peak_weights.rename(columns={'weight':disease_name})
+    dict_gs = {disease_name: (peak_weights['GENE'].tolist(), peak_weights[disease_name].tolist())}
     dict_df_score = dict()
+    scdrs.preprocess(adata,  n_mean_bin=20, n_var_bin=20, copy=False)
     for trait in dict_gs:
         gene_list, gene_weights = dict_gs[trait]
         dict_df_score[trait] = scdrs.score_cell(data=adata,
         gene_list=gene_list,
         gene_weight=gene_weights,
         ctrl_match_key="mean_var",
         n_ctrl=1000,
         weight_opt="vs",
         return_ctrl_raw_score=False,
         return_ctrl_norm_score=True,
         verbose=False,
     )
     return dict_df_score
 
+def scads_rna(adata,gs_file):
+
+    '''
+    adata: AnnData object
+
+    gs_file: output from cmagma pipline gene analysis results
+    or any gene set you interested in .gs format 
+    use save_gs function to save gene set file as .gs format
+    
+    disease_name: disease name interested from GWAS
+
+    '''
+    dict_df_score = dict()
+    scdrs.preprocess(adata,  n_mean_bin=20, n_var_bin=20, copy=False)
+    for trait in gs_file:
+        gene_list, gene_weights = gs_file[trait]
+        dict_df_score[trait] = scdrs.score_cell(data=adata,
+        gene_list=gene_list,
+        gene_weight=gene_weights,
+        ctrl_match_key="mean_var",
+        n_ctrl=1000,
+        weight_opt="vs",
+        return_ctrl_raw_score=False,
+        return_ctrl_norm_score=True,
+        verbose=False,
+    )
+    return dict_df_score
 
         
 #########################################################################################
 #####                          Statistical Analysis                                ######
 #########################################################################################
 
 
@@ -436,19 +579,20 @@
             "assoc_mcp",
             "assoc_mcz"]
         for fdr_threshold in fdr_thresholds:
             res_cols.append(f"n_fdr_{fdr_threshold}")
 
         df_res = pd.DataFrame(index=group_list, columns=res_cols)
         df_res.index.name = "group"
-
+        pvals = df_reg["pval"].values
+        pvals[pvals == 0] = 1e-10 
         df_fdr = pd.DataFrame(
             {"fdr": multipletests(df_reg["pval"].values, method="fdr_bh")[1]},
-            index=df_reg.index,
-        )
+            index=df_reg.index,)
+
 
         for group in group_list:
             group_cell_list = list(df_reg.index[df_reg[group_col] == group])
             # Basic info
             df_res.loc[group, ["n_cell", "n_ctrl"]] = [len(group_cell_list), n_ctrl]
 
             # Number of FDR < fdr_threshold cells in each group
@@ -465,169 +609,203 @@
                 df_reg.loc[group_cell_list, control_list], 0.95, axis=0
             )
             mc_p = ((v_ctrl_score_q95 >= score_q95).sum() + 1) / (
                 v_ctrl_score_q95.shape[0] + 1
             )
             mc_z = (score_q95 - v_ctrl_score_q95.mean()) / v_ctrl_score_q95.std()
             df_res.loc[group, ["assoc_mcp", "assoc_mcz"]] = [mc_p, mc_z]
+            
+        dict_df_res[group_col] = df_res      
 
     return dict_df_res
 
 
 
 #########################################################################################
 #####                                Visualization                                 ######
 #########################################################################################
 
+from statsmodels.stats.multitest import multipletests
+import matplotlib.transforms as mtrans
+import matplotlib.patches as patches
+import seaborn as sns
+import matplotlib.pyplot as plt
+
+
+#change the prop of cell color into mean disease score 
+from statsmodels.stats.multitest import multipletests
+import matplotlib.transforms as mtrans
+import matplotlib.patches as patches
+
+def plot_group_stats(dict_df_stats=None):
+
+    
+    trait_list = list(dict_df_stats.keys())
+    # compile df_fdr_prop, df_assoc_fdr, df_hetero_fdr from dict_df_stats
+    df_fdr_prop = pd.concat(
+        [
+            -np.log10(dict_df_stats[trait]["assoc_mcp"])+1 
+            
+            for trait in trait_list
+        ],
+        axis=1,
+    ).T
+
+
+    df_assoc_fdr = pd.concat(
+        [dict_df_stats[trait]["assoc_mcp"] for trait in trait_list], axis=1
+    ).T
+
+    df_assoc_fdr = pd.DataFrame(
+        multipletests(df_assoc_fdr.values.flatten(), method="fdr_bh")[1].reshape(
+            df_assoc_fdr.shape
+        ),
+        index=df_assoc_fdr.index,
+        columns=df_assoc_fdr.columns,
+    )
+
+
+    df_hetero_fdr = pd.concat(
+        [dict_df_stats[trait]["assoc_mcp"] for trait in trait_list], axis=1
+    ).T
+    df_hetero_fdr = pd.DataFrame(
+        multipletests(df_hetero_fdr.values.flatten(), method="fdr_bh")[1].reshape(
+            df_hetero_fdr.shape
+        ),
+            index=df_hetero_fdr.index,
+            columns=df_hetero_fdr.columns,
+        )
+    
+
+    df_fdr_prop.index = trait_list
+
+    df_assoc_fdr.index = trait_list
+  
+    df_hetero_fdr.index = trait_list
+    
+
+    df_hetero_fdr = df_hetero_fdr.map(lambda x: "" if x < 0.05 else "")
+    df_hetero_fdr[df_assoc_fdr > 0.1] = ""
+
+    fig, ax = plot_heatmap(
+        df_fdr_prop,
+        squaresize=40,
+        heatmap_annot=df_hetero_fdr,
+        heatmap_annot_kws={"color": "blue", "size": 8},
+        heatmap_cbar_kws=dict(
+            use_gridspec=False, location="top", fraction=0.01, pad=0.3, drawedges=True),
+        heatmap_vmin=0,
+        heatmap_vmax=4,
+        colormap_n_bin=8,
+    )
+
+    small_squares(
+        ax,
+        pos=[(y, x) for x, y in zip(*np.where(df_assoc_fdr < 0.05))],
+        size=0.6,
+        linewidth=0.5,
+    )
+
+    cb = ax.collections[0].colorbar
+    cb.ax.tick_params(labelsize=4)
+    #cb.set_ticks([-4.0, 0, 4.0])
+    #cb.ax.set_xticklabels(["-4", "0", "4"], size=7)
+    #cb.ax.set_title("Prop. of sig. cells (FDR < 0.1)", fontsize=8)
+    cb.ax.set_title("-log10 P", fontsize=8)
+    cb.outline.set_edgecolor("black")
+    cb.outline.set_linewidth(1)
+
+    plt.tight_layout()
+    
+    
+    
+def discrete_cmap(N, base_cmap=None, start_white=True):
+    base = plt.colormaps.get_cmap(base_cmap)
+    color_list = base(np.linspace(0, 1, N))
+    if start_white:
+        color_list[0, :] = 1.0
+    cmap_name = base.name + str(N)
+    return base.from_list(cmap_name, color_list, N)
+
 
 
 def plot_heatmap(
     df,
     dpi=150,
-    squaresize=20,
+    squaresize=10,
     heatmap_annot=None,
-    heatmap_annot_kws={"color": "black", "size": 4},
+    heatmap_annot_kws={"color": "black", "size": 10},
     heatmap_linewidths=0.5,
     heatmap_linecolor="gray",
     heatmap_xticklabels=True,
     heatmap_yticklabels=True,
     heatmap_cbar=True,
-    heatmap_cbar_kws=dict(use_gridspec=False, location="top", fraction=0.03, pad=0.01),
-    heatmap_vmin=0.0,
-    heatmap_vmax=1.0,
+    heatmap_cbar_kws=dict(use_gridspec=False, location="top", fraction=0.05, pad=0.1),
+    heatmap_vmin=0,
+    heatmap_vmax=4.0,
     xticklabels_rotation=90,
-    colormap_n_bin=10,
+    colormap_n_bin=8,
 ):
-    figwidth = df.shape[1] * squaresize / float(dpi)
-    figheight = df.shape[0] * squaresize / float(dpi)
+    #figwidth = df.shape[1] * (squaresize) / float(dpi)
+    #figheight = df.shape[0] * squaresize / float(dpi)
+    figwidth = 6
+    figheight = 6
     fig, ax = plt.subplots(1, figsize=(figwidth, figheight), dpi=dpi)
     fig.subplots_adjust(left=0, right=1, bottom=0, top=1)
     ax.set_facecolor("silver")
+    ax.invert_yaxis()
+    #ax.yaxis.set_label_position("right")
+    #ax.yaxis.tick_right()
     sns.heatmap(
         df,
         annot=heatmap_annot,
         annot_kws=heatmap_annot_kws,
         fmt="",
-        cmap=discrete_cmap(colormap_n_bin, "RdPu"),
+        cmap=discrete_cmap(colormap_n_bin, "RdYlBu_r"),
         linewidths=heatmap_linewidths,
         linecolor=heatmap_linecolor,
         square=True,
         ax=ax,
         xticklabels=heatmap_xticklabels,
         yticklabels=heatmap_yticklabels,
         cbar=heatmap_cbar,
         cbar_kws=heatmap_cbar_kws,
         vmin=heatmap_vmin,
         vmax=heatmap_vmax,
     )
 
     plt.yticks(fontsize=8)
+
+    for tick_label in ax.axes.get_yticklabels():
+        tick_label.set_color("black")
     ax.set_xticklabels(
         ax.get_xticklabels(),
         rotation=xticklabels_rotation,
         va="top",
         ha="right",
         fontsize=8,
     )
     ax.tick_params(left=False, bottom=False, pad=-2)
     trans = mtrans.Affine2D().translate(5, 0)
     for t in ax.get_xticklabels():
         t.set_transform(t.get_transform() + trans)
     return fig, ax
-
-
-def discrete_cmap(N, base_cmap=None, start_white=True):
-    base = plt.cm.get_cmap(base_cmap)
-    color_list = base(np.linspace(0, 1, N))
-    if start_white:
-        color_list[0, :] = 1.0
-    cmap_name = base.name + str(N)
-    return base.from_list(cmap_name, color_list, N)
-
+    
 def small_squares(ax, pos, size=1, linewidth=0.8):
+    """
+    Draw many small squares on ax, given the positions of
+    these squares.
 
+    """
     for xy in pos:
         x, y = xy
         margin = (1 - size) / 2
         rect = patches.Rectangle(
             (x + margin, y + margin),
             size,
             size,
             linewidth=linewidth,
-            ls='--',
             edgecolor="black",
             facecolor="none",
-            zorder=40,
+            zorder=15,
         )
-        ax.add_patch(rect)
-
-
-
-
-def plot_stat(dict_df_stats=None):
-
-    
-    trait_list = list(dict_df_stats.keys())
-    # compile df_fdr_prop, df_assoc_fdr, df_hetero_fdr from dict_df_stats
-    df_fdr_prop = pd.concat(
-        [
-            dict_df_stats[trait]["n_fdr_0.1"] / dict_df_stats[trait]["n_cell"]
-            for trait in trait_list
-        ],
-        axis=1,
-    ).T
-    df_assoc_fdr = pd.concat(
-        [dict_df_stats[trait]["assoc_mcp"] for trait in trait_list], axis=1
-    ).T
-    df_assoc_fdr = pd.DataFrame(
-        multipletests(df_assoc_fdr.values.flatten(), method="fdr_bh")[1].reshape(
-            df_assoc_fdr.shape
-        ),
-        index=df_assoc_fdr.index,
-        columns=df_assoc_fdr.columns,
-    )
-    df_hetero_fdr = pd.concat(
-        [dict_df_stats[trait]["assoc_mcz"] for trait in trait_list], axis=1
-    ).T
-    df_hetero_fdr = pd.DataFrame(
-        multipletests(df_hetero_fdr.values.flatten(), method="fdr_bh")[1].reshape(
-            df_hetero_fdr.shape
-        ),
-            index=df_hetero_fdr.index,
-            columns=df_hetero_fdr.columns,
-        )
-    df_fdr_prop.index = trait_list
-    df_assoc_fdr.index = trait_list
-    df_hetero_fdr.index = trait_list
-    
-
-    df_hetero_fdr = df_hetero_fdr.applymap(lambda x: "" if x < 0.05 else "")
-    df_hetero_fdr[df_assoc_fdr > 0.05] = ""
-
-    fig, ax = plot_heatmap(
-        df_fdr_prop,
-        squaresize=40,
-        heatmap_annot=df_hetero_fdr,
-        heatmap_annot_kws={"color": "blue", "size": 8},
-        heatmap_cbar_kws=dict(
-            use_gridspec=False, location="top", fraction=0.03, pad=0.1, drawedges=True
-        ),
-        heatmap_vmin=0,
-        heatmap_vmax=0.2,
-        colormap_n_bin=3,
-    )
-
-    small_squares(
-        ax,
-        pos=[(y, x) for x, y in zip(*np.where(df_assoc_fdr < 0.05))],
-        size=0.6,
-        linewidth=0.5,
-    )
-
-    cb = ax.collections[0].colorbar
-    cb.ax.tick_params(labelsize=8)
-
-    cb.ax.set_title("Prop. of sig. cells", fontsize=8)
-    cb.outline.set_edgecolor("black")
-    cb.outline.set_linewidth(1)
-
-    plt.tight_layout()
+        ax.add_patch(rect)
```

### Comparing `sc_var-1.2.0/PKG-INFO` & `sc_var-1.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sc_var
-Version: 1.2.0
+Version: 1.2.1
 Summary: An approch for interpreting disease-associated human variants using single-cell epigenomics
 Author: Gefei Z
 Author-email: gefeizhao@163.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -12,46 +12,47 @@
 Requires-Dist: mygene (>=3.2.2,<4.0.0)
 Requires-Dist: scanpy (>=1.9.6,<2.0.0)
 Requires-Dist: scdrs (>=1.0.2,<2.0.0)
 Requires-Dist: scipy (>=1.11.4,<2.0.0)
 Requires-Dist: seaborn (>=0.13.1,<0.14.0)
 Description-Content-Type: text/markdown
 
-
 # SC-VAR
 
-An approach to interpreting disease-associated human variants using single-cell epigenomics
+Here we report a human variants interpretation software for single cell data, named SC-VAR. 
 
 
 # What can sc-var do?
 
-Identify risk genes, gene sets, and cells related to different stages and diseases. 
+This tool can interpret disease-related risks with whole genome wide (including both coding and non-coding regions) variants from GWAS studies and single-cell data on three layers: risk genes, gene sets, and cell types.
+
 
-Infer cell types involved in complex traits and diseases using single-cell epigenomes AND does not rely on any other annotations and other Omics data. 
 
 
 # How to install?
 
 pip install sc-var
 
 check https://pypi.org/project/sc-var/
 
 
 ## About
 
 
-![sc_var](https://github.com/gefeiZ/sc_var/assets/116159260/9a37b915-641d-48d6-aa73-97c6f3684b41)
 
+\includegraphics[]{../Desktop/flow.png}
 
 
 
 ## Usage
 
-Check Usage.ipynb for details
+Check https://github.com/gefeiZ/sc_var/  for details
+
+
 
 Data request: 
 
-Single cell ATAC-seq data &
-Peak co-accessibility Data &
+Single cell data &
+Peak co-accessibility Data or Peak to gene linkage Data (which could obtained from single cell data using cicero or signac) &
 GWAS data
```

