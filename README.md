# Genomic Drivers of Uveal Melanoma Metastasis

## Overview
Multi-omics machine learning analysis to identify genomic drivers 
of disease progression in Uveal Melanoma (UVM) using TCGA data.

## Data
- RNA-seq gene expression (20,530 genes, 80 patients)
- DNA Methylation 450k array (485,577 CpG probes, 80 patients)
- Clinical outcome labels from TCGA-CDR
- Source: UCSC Xena Browser

## Methods
- Feature selection using variance filtering and t-tests
- Random Forest and SVM classification (5-fold cross validation)
- Combined multi-omics analysis (RNA + Methylation)

## Results
| Model | RNA only | RNA + Methylation |
|-------|----------|-------------------|
| Random Forest AUC | 0.879 | 0.887 |
| SVM AUC | 0.908 | 0.908 |

## Top Genomic Drivers Identified
- **TIMP3** — tumor suppressor, matrix degradation
- **ENPP2** — immune evasion via autotaxin pathway
- **KDM5B** — epigenetic reprogramming
- **TANK** — NF-κB inflammatory signaling (methylation)
- **WHAMM** — actin cytoskeleton, cell migration (methylation)

## Tools
Python, pandas, scikit-learn, scipy, matplotlib, seaborn
