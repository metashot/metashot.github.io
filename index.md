---
layout: default
title: Home
nav_order: 1
permalink: /
---

MetaShot is a curated set of [Docker](https://www.docker.com/) images and
[Nextflow](nextflow.io) pipelines for metagenomics and bacterial genomics
{:.fs-6 .fw-300 }

[Get started now](#getting-started){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [View it on GitHub](https://github.com/metashot){: .btn .fs-5 .mb-4 .mb-md-0 }

---

## Getting started

### Dependencies

MetaShot requires [Docker](https://www.docker.com/) (or
[Singularity](https://singularity.lbl.gov/)) and [Nextflow](nextflow.io). If you
want to use Singularity instead of Docker, comment the Docker lines in the
`nextflow.config` file (this file is present in each workflow) and add the
following:

```groovy
singularity.enabled = true
singularity.autoMounts = true
```

Alternatively, you can provide an extra configuration file by using the command
line option `-c <config_file>`
([documentation](https://www.nextflow.io/docs/latest/config.html#configuration-file)).

### Quick start: run the Kraken2/Braken workflow on the local machine
This example shows how to run
[metashot/kraken2](https://github.com/metashot/kraken2), a pipeline for the
taxonomic classification of reads and abundance estimation of species in
metagenomic samples. It relies on two related software,
[Kraken2](https://ccb.jhu.edu/software/kraken2/) and
[Bracken](https://ccb.jhu.edu/software/bracken/).

1. Download and extract/unzip a Kraken2/Bracken database available at [this
   page](https://benlangmead.github.io/aws-indexes/k2);
1. Start running the analysis on the compressed paired-end sequences in FASTQ
   format:
   
   ```bash
   nextflow run metashot/kraken2 -r 1.0.1 \
     --reads '*_R{1,2}.fastq.gz' \
     --kraken2_db k2db \
     --read_len 100 \
     --outdir results
   ```
1. The pipeline will create in the `results` folder the following directories:

   ```bash
   bracken  bracken_combined  kraken2  raw_reads_stats
   ```

## System requirements
Each step in the pipeline has a default set of requirements for number of CPUs,
memory and time. For some of the steps in the pipeline, if the job exits with an
error it will automatically resubmit with higher requests (see the file
`process.config`). You can customize the compute resources that the pipeline
requests by either:
- setting the global parameters `--max_cpus`, `--max_memory` and
  `--max_time` in the command line, or
- creating a [custom config
  file](https://www.nextflow.io/docs/latest/config.html#configuration-file)
  (`-c` or `-C` parameters), or
- modifying the `process.config` file.

## Reproducibility
We recommend to specify a pipeline version when running the workflow on your
data with the `-r` parameter, e.g.:

```bash
  nextflow run metashot/kraken2 -r 1.0.0 ...
```

The workflows use the docker images available at [MetaShot Docker Hub
repositories](https://hub.docker.com/u/metashot/) for reproducibility. You can
check the version of the software used in each workflow by opening the file
`process.config`. For example `container = metashot/kraken2:2.0.9-beta-6` means
that the version of kraken2 is the `2.0.9-beta` (the last number, 6, is the
metashot release of this image).

## Credits
MetaShot is maintained by Davide Albanese and Claudio Donati at the [FEM's Unit
of Computational
Biology](https://www.fmach.it/eng/CRI/general-info/organisation/Chief-scientific-office/Computational-biology).
