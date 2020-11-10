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
`nextflow.config` file (which is present in each workflow and add the following:

```nextflow
singularity.enabled = true
singularity.autoMounts = true
```

Alternatively, you can provide an extra configuration file by using the command
line option `-c <config_file>`.








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