# Bulk RNA-seq Differential Expression Workflow

A reproducible R workflow for **bulk RNA-seq differential expression and pathway analysis**, demonstrated with an example count dataset.

## Overview

The workflow covers the core steps commonly used in transcriptomic analysis:

- sample-level quality assessment
- PCA and correlation analysis
- differential expression with edgeR
- volcano-plot and heatmap visualization
- GO and KEGG enrichment
- gene-set enrichment analysis (GSEA)

## Project Structure

```text
airway-DEG-analysis/
├── Step00-R packages.R
├── Step01-airwayCounts.R
├── Step02-sampleDistribution.R
├── Step03-PCA_Cor.R
├── Step04-edgeR_DEG.R
├── Step05-DEG_volcano.R
├── Step05-DGE_heatmap.R
├── Step06-GO_KEGG_enrich.R
├── Step06-GSEA_analysis.R
├── data/
├── result/
└── Diff_analysis/
```

## Example Experimental Design

The example metadata contains three conditions with biological replicates:

```text
A = control
B = treatment 1
C = treatment 2
```

The workflow can be adapted to other experimental designs by replacing the count matrix and sample metadata.

## Main Methods

### Exploratory analysis
- count-distribution inspection
- PCA
- sample-sample correlation

### Differential expression
- edgeR-based modeling
- fold-change and statistical-significance filtering
- volcano plots
- DEG heatmaps

### Functional interpretation
- Gene Ontology enrichment
- KEGG pathway enrichment
- GSEA

## Intended Use

This repository serves as a compact, reusable reference for bulk transcriptomic analysis. For real studies, filtering thresholds, design matrices, covariates, contrasts, and enrichment databases should be selected according to the experimental design.

## Related Areas

Transcriptomics · differential expression · pathway analysis · cancer biology · translational bioinformatics
