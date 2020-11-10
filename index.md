---
layout: default
title: Home
nav_order: 1
permalink: /
---

MetaShot is a curated set of [Docker](https://www.docker.com/) images and
[Nextflow](nextflow.io) pipelines for metagenomics and bacterial genomics
{:.fs-6 .fw-300 }

[Get started now](#getting-started){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [View it on GitHub](https://github.com/pmarsceill/just-the-docs){: .btn .fs-5 .mb-4 .mb-md-0 }

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
taxonomic classification of reads and the abundance estimation of species in
metagenomic samples. It relies on two main software,
[Kraken2](https://ccb.jhu.edu/software/kraken2/) for the taxonomic
classification of short sequences, and
[Bracken](https://ccb.jhu.edu/software/bracken/), which uses the predicted
taxonomy to estimate the number of reads originating from each species in a
metagenomic sample.

1. Download and extract/unzip a Kraken2/Bracken database available at [this
   page](https://benlangmead.github.io/aws-indexes/k2);
1. Start running the analysis on the compressed paired-end sequences in FASTQ
   format:
   
  ```bash
  nextflow run metashot/kraken2:1.0.1 \
    --reads '*_R{1,2}.fastq.gz' \
    --kraken2_db k2db \
    --read_len 100 \
    --outdir results
  ```








- ![barrnap](https://img.shields.io/docker/v/metashot/barrnap?sort=semver&label=barrnap&style=flat-square)

🚀 🐼

yes

You can use the [editor on GitHub](https://github.com/pmarsceill/test-jtd/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/pmarsceill/test-jtd/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.