---
layout: default
title: Workflows
nav_order: 3
permalink: /workflows/
---

# Workflows

MetaShot provides a curated, easy-to-use collection of [Nextflow](nextflow.io)
pipelines for metagenomics and bacterial genomics. We recommend to specify a
pipeline version when running the workflow on your data with the `-r` parameter,
e.g. `-r 1.0.0`.


| Workflow              | Description                                                                                   | Release                                                                                                        |
|:----------------------|:----------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------|
| kraken2               | Taxonomic classification of reads and abundance estimation of species in metagenomic samples  | ![kraken2][kraken2_release]                               |
| mag-illumina          | Metagenomic Assembled Genomes from Illumina sequences                                         | ![mag-illumina](https://img.shields.io/github/v/release/metashot/mag-illumina?sort=semver)                     |
| kraken2               | Taxonomic classification of reads and abundance estimation of species in metagenomic samples  | ![kraken2](https://img.shields.io/github/v/release/metashot/kraken2?sort=semver)                               |
| mag-illumina          | Metagenomic Assembled Genomes from Illumina sequences                                         | ![mag-illumina](https://img.shields.io/github/v/release/metashot/mag-illumina?sort=semver)                     |





[kraken2_release]: https://img.shields.io/github/v/release/metashot/kraken2?sort=semver&link=https://github.com/metashot/kraken2 "kraken2 release"