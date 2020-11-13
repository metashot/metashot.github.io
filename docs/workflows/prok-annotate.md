---
layout: default
title: prok-annotate
nav_order: 4
permalink: /workflows/prok-annotate
parent: Workflows
---

# prok-annotate

![annotate](https://img.shields.io/github/v/release/metashot/prok-annotate?sort=semver&label=Latast%20release&style=for-the-badge)

metashot/prok-annotate is a workflow for functional annotation of prokaryotic
contigs/genomes.

[View it on GitHub](https://github.com/metashot/prok-annotate){: .btn .fs-5}

## Main features

- Input: prokaryotic contig/genomes in FASTA format;
- Protein-coding gene prediction using
  [Prodigal](https://github.com/hyattpd/Prodigal);
- Functional annotation through orthology assignment by
  [eggNOG-mapper](https://github.com/eggnogdb/eggnog-mapper) v2 and the [eggNOG
  v5.0](http://eggnog-mapper.embl.de/) database.


## Quick start

1. Install Docker (or Singulariry) and Nextflow (see [Dependences](/#dependencies));
1. Fetch the eggNOG database:

   ```bash
   docker run --rm -v /path/to/eggnog_data:/eggnog_data metashot/eggnog-mapper:2.0.1-3 \
     python /eggnog_mapper/download_eggnog_data.py -y --data_dir /eggnog_data
   ```
1. Start running the analysis:

   ```bash
   nextflow run metashot/prok-annotate \
     --genomes "data/*.fa" \
     --eggnog_db /path/to/eggnog_data \
     --outdir results
   ```

## Parameters
See the file
[`nextflow.config`](https://github.com/metashot/prok-annotate/blob/master/nextflow.config)
for the complete list of parameters.

## Output
The files and directories listed below will be created in the `results` directory
after the pipeline has finished.

### Main outputs
- `prodigal`: the output of eggNOG-mapper
  [documentation](https://github.com/hyattpd/prodigal/wiki/understanding-the-prodigal-output).
- `eggnog`: the output of Prodigal
  [documentation](https://github.com/eggnogdb/eggnog-mapper/wiki/eggNOG-mapper-v2).

## System requirements
Please refer to [System requirements](/#system-requirements) for the complete
list of system requirements options.
