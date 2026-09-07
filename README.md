## Overview
This repository provides the computational pipeline for our study on the human CA1–Subiculum interface. We integrated Stereo-seq and snRNA-seq to establish a molecularly anchored parcellation framework using marker genes such as FN1 and ETV1.


## Files
### ComputingEnvironment_PackageVersions.docx
Software environment and package version information used in the scRNA-seq analysis workflow.

### Fig1_bayesDEG.ipynb

Notebook for Figure 1 and FigS1, covering the initial spatial transcriptomic parcellation of the human hippocampal CA1–Subiculum interface. Analyses include sample overview, CA1-region extraction using the CA1-enriched marker MPPED1, BayesSpace-based unsupervised clustering within the putative CA1 territory, and identification of transcriptionally distinct domains corresponding to CA1 and Subiculum. FigS1 extends this analysis to AD samples.

### Fig2_sn.ipynb

Notebook for Figure 2 and FigS2, focusing on cross-modal validation of Subiculum marker genes using public human hippocampal snRNA-seq data. Analyses include CA1/Sub cell extraction, UMAP visualization of cell types and neuronal subtypes, screening of reported region-specific markers, identification of FN1 as a Sub-enriched marker, and projection of FN1-based Sub/CA1 parcellation onto spatial transcriptomic data. FigS2 includes additional validation of non-signature or subtype-associated genes such as COL5A2, NTNG1, and SEMA3E.

### Fig3.ipynb

Notebook for Figure 3 and FigS3-4, focusing on validation and cross-platform benchmarking of CA1–Sub molecular markers. Analyses include differential expression between molecularly defined Sub and CA1 regions, evaluation of Sub-enriched markers including ETV1, PCSK1, CAMK2G, and FN1, RNAscope-based validation of FN1 and ETV1, comparison with public 10X Genomics spatial transcriptomic data, and expression-gradient analysis across the CA1–Sub interface. FigS3 provides multi-sample spatial visualization and quantification, while FigS4 supports cross-species validation using mouse in situ hybridization and spatial transcriptomic datasets.

### Fig4.ipynb

Notebook for Figure 4 and FigS5, containing region-resolved analysis of Alzheimer’s Disease-associated transcriptional alterations using bin100 spatial transcriptomic data. Analyses include identification of AD-associated DEGs in Sub and CA1, comparison of upregulated and downregulated gene programs, GO enrichment analysis, intersection of Sub-specific markers with AD-related DEGs, hdWGCNA co-expression module construction, module eigengene analysis, spatial visualization of disease-associated modules, and hub-gene/network analysis highlighting Sub-associated bioenergetic remodeling. FigS5 provides supporting volcano plots, marker/module spatial maps, and additional module-score analyses.

### Fig5.ipynb

Notebook for Figure 5 and FigS6, covering single-cell spatial transcriptomic analysis of cell type-specific AD-associated changes in Sub and CA1. Analyses include integration of bin100 regional annotations with cellbin-level spatial transcriptomic data, Spatial-ID-based cell type annotation, comparison with public snRNA-seq references, cell-type density analysis, cell-type-specific DEG and enrichment analysis, Jaccard overlap between DEGs and hdWGCNA modules, M8 bioenergetic module scoring in EX_Sub and IN_PVALB neurons, spatial visualization of cell-type-specific module activity, and hub-gene expression analysis including NDUFA4. FigS6 summarizes technical quality control, cell segmentation validation, marker-based cell type annotation, and chip-level sequencing quality metrics.


### Con3.1.bin100.CA1_Sub.rds
Processed R object containing spatial transcriptomic data for a representative Control sample (bin100 resolution). This file includes the specific CA1 and Subiculum regions extracted based on MPPED1 expression.

### AD6.1.bin100.CA1_Sub.rds
Processed R object containing spatial transcriptomic data for a representative Alzheimer's Disease sample (bin100 resolution). This file includes the specific CA1 and Subiculum regions extracted based on MPPED1 expression.

## Data availability
The following .rds files are available via a Quark cloud link:

Con3.1.bin100.CA1_Sub.rds

AD6.1.bin100.CA1_Sub.rds

https://pan.quark.cn/s/ce11e7643be1

While the representative samples above are provided for quick testing, the complete raw datasets for this study must be obtained from the following official repositories:
Spatial Transcriptomics (Stereo-seq) Data: Deposited in the CNGB Nucleotide Sequence Archive (CNSA) under accession number CNP0005077 (https://db.cngb.org/search/project/CNP0005077/).

Single-nucleus RNA-seq (snRNA-seq) Data: Sourced from the Gene Expression Omnibus (GEO) under platform accession GSE186538 (https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE186538).

Users intended to fully reproduce the entire study from scratch should download the raw matrices or FASTQ files from these sources.
