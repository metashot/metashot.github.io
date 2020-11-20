---
layout: default
title: Workflows
nav_order: 3
permalink: /workflows/
---

# Workflows
{: .no_toc }

MetaShot provides a curated, easy-to-use collection of [Nextflow](nextflow.io)
pipelines for metagenomics and bacterial genomics. We recommend to specify a
pipeline version when running the workflow on your data with the `-r` parameter,
e.g. `-r 1.0.0`.

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>


## Metagenomics

### kraken2

![kraken2](https://img.shields.io/github/v/release/metashot/kraken2?sort=semver&label=Latast%20release)

metashot/kraken2 is a workflow for the taxonomic classification of reads and the
abundance estimation of species in metagenomic samples.

[View it on GitHub](https://github.com/metashot/kraken2){: .btn}

### mag-illumina

![mag_illumina](https://img.shields.io/github/v/release/metashot/mag-illumina?sort=semver&label=Latast%20release)

metashot/mag-illumina is a workflow for the assembly and binning of Illumina
sequences from metagenomic samples.

[View it on GitHub](https://github.com/metashot/mag-illumina){: .btn}


## Prokaryotes

### prok-quality

![prok_quality](https://img.shields.io/github/v/release/metashot/prok-quality?sort=semver&label=Latast%20release)

metashot/prok-quality is a pipeline for assessing the quality of prokaryotic
genomes including the prediction of rRNA and tRNA genes.

[View it on GitHub](https://github.com/metashot/prok-quality){: .btn}

### prok-classify

![prok_classify](https://img.shields.io/github/v/release/metashot/prok-classify?sort=semver&label=Latast%20release)

metashot/prok-classify is a workflow for assigning objective taxonomic
classifications to bacterial and archaeal genomes using
[GTDB-Tk](https://github.com/Ecogenomics/GTDBTk) and the Genome Database
Taxonomy GTDB.

[View it on GitHub](https://github.com/metashot/prok-classify){: .btn}

### prok-annotate

![prok-annotate](https://img.shields.io/github/v/release/metashot/prok-annotate?sort=semver&label=Latast%20release)

metashot/prok-annotate is a workflow for functional annotation of prokaryotic
contigs/genomes.

[View it on GitHub](https://github.com/metashot/prok-annotate){: .btn}

### prok-snp

![prok-snp](https://img.shields.io/github/v/release/metashot/prok-snp?sort=semver&label=Latast%20release)

metashot/prok-snp is a workflow for the identification SNVs (of closely related
organisms) and phylogenetic tree inference from prokaryotic isolates.

[View it on GitHub](https://github.com/metashot/prok-snp){: .btn}
