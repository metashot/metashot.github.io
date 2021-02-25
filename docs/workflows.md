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
metashot/kraken2 is a workflow for the taxonomic classification of reads and the
abundance estimation of species in metagenomic samples.

[Documentation](https://github.com/metashot/kraken2){: .btn}

### mag-illumina
metashot/mag-illumina is a workflow for the assembly and binning of Illumina
sequences from metagenomic samples.

[Documentation](https://github.com/metashot/mag-illumina){: .btn}


## Prokaryotes

### prok-assembly
Assemble prokaryotic isolate genomes from Illumina reads.

[Documentation](https://github.com/metashot/prok-assembly){: .btn}

### prok-quality
metashot/prok-quality is a pipeline for assessing the quality of prokaryotic
genomes including the prediction of rRNA and tRNA genes.

[Documentation](https://github.com/metashot/prok-quality){: .btn}

### prok-classify
metashot/prok-classify is a workflow for assigning objective taxonomic
classifications to bacterial and archaeal genomes using
[GTDB-Tk](https://github.com/Ecogenomics/GTDBTk) and the Genome Database
Taxonomy GTDB.

[Documentation](https://github.com/metashot/prok-classify){: .btn}

### prok-annotate
metashot/prok-annotate is a workflow for functional annotation of prokaryotic
contigs/genomes.

[Documentation](https://github.com/metashot/prok-annotate){: .btn}

### prok-snp
metashot/prok-snp is a workflow for the identification SNVs (of closely related
organisms) and phylogenetic tree inference from prokaryotic isolates.

[Documentation](https://github.com/metashot/prok-snp){: .btn}

### prok-pan
metashot/prok-pan is a workflow for the pan genome analysis of closely related
prokariotic genomes.

[Documentation](https://github.com/metashot/prok-pan){: .btn}

## Other

### busco
metashot/busco is a pipeline for assessing the quality of prokaryotic and
eukaryotic genomes.

[Documentation](https://github.com/metashot/busco){: .btn}
