---
layout: default
title: Docker images
nav_order: 2
permalink: /docker/
---

# Docker images

The MetaShot workflows use the Docker images for reproducibility[^1]. The
last number of the Docker image version (e.g. 1 in `2.0.3-1`) represent the
MetaShot release of that image (e.g. the first image release of the software
version `2.0.3`). Note that the `latest` tag is not present.

[View it on GitHub](https://github.com/metashot/docker){: .btn .fs-5 .mr-2 }
[View it on Docker Hub](https://hub.docker.com/u/metashot/){: .btn .fs-5 .btn-blue }

{% capture my_include %}{% include https://raw.githubusercontent.com/metashot/prok-annotate/master/README.md %}{% endcapture %}
{{ my_include | markdownify }}

---

[^1]: Nüst D, Sochat V, Marwick B, Eglen SJ, Head T, et al. (2020) *Ten simple
      rules for writing Dockerfiles for reproducible data science*. PLOS
      Computational Biology 16(11): e1008316.
      [Link](https://doi.org/10.1371/journal.pcbi.1008316).