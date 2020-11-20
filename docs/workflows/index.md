---
layout: default
title: Workflows
nav_order: 3
permalink: /workflows/
has_children: true
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
1. TOC
{:toc}
</details>


## kraken2 ![kraken2](https://img.shields.io/github/v/release/metashot/kraken2?sort=semver&label=Latast%20release)

metashot/kraken2 is a workflow for the taxonomic classification of reads and the
abundance estimation of species in metagenomic samples.

[View it on GitHub](https://github.com/metashot/kraken2){: .btn}


## prok-quality ![prok_quality](https://img.shields.io/github/v/release/metashot/prok-quality?sort=semver&label=Latast%20release)

metashot/prok-quality is a pipeline for assessing the quality of prokaryotic
genomes including the prediction of rRNA and tRNA genes (MISAG and the MIMAG
standards[^1])

[View it on GitHub](https://github.com/metashot/prok-quality){: .btn}

---

[^1]: Bowers R., Kyrpides N., Stepanauskas R. et al. *Minimum information about
      a single amplified genome (MISAG) and a metagenome-assembled genome
      (MIMAG) of bacteria and archaea*. Nat. Biotechnol. 35, 725–731 (2017).
      [Link[(https://doi.org/10.1038/nbt.3893).