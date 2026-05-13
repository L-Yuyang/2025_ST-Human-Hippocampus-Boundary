## Overview
This repository provides the computational pipeline for our study on the human CA1–Subiculum interface. We integrated Stereo-seq and snRNA-seq to establish a molecularly anchored parcellation framework using marker genes such as FN1 and ETV1.


## Files
### Fig1_bayesDEG.ipynb
Main notebook for spatial transcriptomic analysis in Figure 1 and associated Supplementary Figures, including:
Implementation of the Bayesian-based differential expression analysis.
Identification of the initial molecular framework for the CA1–Subiculum interface.

### Fig2_sn.ipynb
Main notebook for single-nucleus RNA-seq (snRNA-seq) analysis in Figure 2 and associated Supplementary Figures, including:
Integration of public snRNA-seq datasets from clinically unremarkable donors.
Cross-modality validation of boundary markers (e.g., FN1, ETV1).

### Fig3.ipynb
Notebook for generating results in Figure 3 and associated Supplementary Figures, focusing on:
Multi-sample spatial parcellation and boundary consistency evaluation.
Expression gradient analysis across the molecularly defined CA1–Sub interface.

### Fig4.ipynb
Notebook for Figure 4 and associated Supplementary Figures, containing analysis of Alzheimer's Disease (AD) vs. Control samples:
Comparative analysis of subfield-specific transcriptomic alterations.
Region-resolved investigations of pathological molecular signatures.

### Fig5.ipynb
Notebook for Figure 5, covering:
Functional enrichment analysis (GO/KEGG) for region-specific markers.
Advanced bioenergetic and metabolic pathway scoring (AUCell-based) within the identified domains.

### Con1.1.bin100.CA1_Sub.rds
Processed R object containing spatial transcriptomic data for a representative Control sample (bin100 resolution). This file includes the specific CA1 and Subiculum regions extracted based on MPPED1 expression.

### AD1.1.bin100.CA1_Sub.rds
Processed R object containing spatial transcriptomic data for a representative Alzheimer's Disease sample (bin100 resolution). This file includes the specific CA1 and Subiculum regions extracted based on MPPED1 expression.

## Data availability
The following .rds files are available via a Quark cloud link:
Con3.1.bin100.CA1_Sub.rds
AD6.1.bin100.CA1_Sub.rds
https://pan.quark.cn/s/ce11e7643be1

While the representative samples above are provided for quick testing, the complete raw datasets for this study must be obtained from the following official repositories:
Spatial Transcriptomics (Stereo-seq) Data: Deposited in the CNGB Nucleotide Sequence Archive (CNSA) under accession code CNP0005077 (https://db.cngb.org/search/project/CNP0005077/).

Single-nucleus RNA-seq (snRNA-seq) Data: Sourced from the Gene Expression Omnibus (GEO) under platform accession GSE186538 (https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE186538).

Users intended to fully reproduce the entire study from scratch should download the raw matrices or FASTQ files from these sources.
