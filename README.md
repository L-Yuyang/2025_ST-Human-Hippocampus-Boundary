## Overview
This repository provides the computational pipeline for our study on the human CA1–Subiculum interface. We integrated Stereo-seq and snRNA-seq to establish a molecularly anchored parcellation framework using marker genes such as FN1 and ETV1.


## Files
### ComputingEnvironment_PackageVersions.docx
Software environment and package version information used in the scRNA-seq analysis workflow.

### Fig1.ipynb

Analysis for Figure 1, including MPPED1-based CA1 region extraction and BayesSpace-based identification of molecularly distinct CA1/Sub domains in control human hippocampus.

### FigS1.ipynb

Supporting analysis for FigS1, showing MPPED1 expression and BayesSpace-based CA1/Sub parcellation in AD human hippocampal samples.

### Fig2.ipynb

Analysis for Figure 2, including public human hippocampal snRNA-seq processing, CA1/Sub cell visualization, marker screening, and FN1-based validation of Sub identity.

### FigS2.ipynb

Supporting analysis for FigS2, including additional snRNA-seq marker evaluation and spatial validation of CA1/Sub annotations in AD samples.

### Fig3.ipynb

Analysis for Figure 3, including Sub-vs-CA1 marker identification, spatial validation of FN1/ETV1-related patterns, RNAscope validation, 10X spatial data comparison, and CA1–Sub gradient analysis.

### FigS3.ipynb

Supporting analysis for FigS3, showing spatial visualization and quantification of ETV1, PCSK1, CAMK2G, FN1, and ETV1 across samples and validation datasets.

### FigS4.ipynb

Supporting analysis for FigS4, showing mouse brain validation of Sub-enriched Fn1 and Etv1 expression using public spatial transcriptomic datasets.

### Fig4.ipynb

Analysis for Figure 4, including region-resolved AD-vs-control DEG analysis, GO enrichment, Sub-specific marker changes, hdWGCNA module analysis, and M8/NDUFA4-related network characterization.

### FigS5.ipynb

Supporting analysis for FigS5, including AD-associated DEG volcano plots, spatial expression of selected genes, additional module scores, and spatial visualization of M2/M5 modules.

### Fig5.ipynb

Analysis for Figure 5, including cellbin-level cell type annotation, cell-type-specific DEG analysis, M8 module scoring in EX_Sub and IN_PVALB neurons, and NDUFA4 expression analysis.

### FigS6.ipynb

Supporting analysis for FigS6, including cell segmentation validation, cell type marker validation, and chip-level quality-control metrics for spatial transcriptomic data.


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
