---
layout: default
title: Workflows
nav_order: 3
permalink: /workflows/
has_children: true
---

# Workflows

MetaShot provides a curated, easy-to-use collection of [Nextflow](nextflow.io)
pipelines for metagenomics and bacterial genomics. We recommend to specify a
pipeline version when running the workflow on your data with the `-r` parameter,
e.g. `-r 1.0.0`.

## Metangenomics

| Workflow        | Description                                                                       | 
|:----------------|:----------------------------------------------------------------------------------|
| kraken2         | Taxonomic classification of reads and abundance estimation of species             |
| mag-illumina    | Metagenomic Assembled Genomes from Illumina sequences                             |

## Prokaryotic genomes

| Workflow        | Description                                                                       |
|:----------------|:----------------------------------------------------------------------------------|
| prok-quality    | Assessing the quality of prokaryotic genomes, filtering and dereplication         |
| prok-classify   | Assign objective taxonomic classifications to prokaryotic genomes                 |
| prok-annotate   | Functional annotation fo prokaryotic contigs/genomes through orthology assignment |
| prok-snp        | SNVs identification and phylogenetic tree inference from prokaryotic isolates     |


[kraken2_release]: https://img.shields.io/github/v/release/metashot/kraken2?sort=semver "kraken2 release"
[mag_illumina_release]: https://img.shields.io/github/v/release/metashot/mag-illumina?sort=semver "mag-illumina release"
[prok_quality_release]: https://img.shields.io/github/v/release/metashot/prok-quality?sort=semver "prok-quality release"
[prok_classify_release]: https://img.shields.io/github/v/release/metashot/prok-classify?sort=semver "prok-classify release"
[prok_annotate_release]: https://img.shields.io/github/v/release/metashot/prok-annotate?sort=semver "prok-annotate release"
[prok_snp_release]: https://img.shields.io/github/v/release/metashot/prok-snp?sort=semver "prok-snp release"
