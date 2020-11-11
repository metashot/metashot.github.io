---
layout: default
title: Docker images
nav_order: 2
permalink: /docker/
---

# Docker images

The MetaShot workflows use the Docker images for reproducibility [[1]](#1)_. The last
number of the Docker image version (e.g. 1 in `2.0.3-1`) represent the MetaShot
release of that image (e.g. the first image release of the software version
`2.0.3`). Note that the `latest` tag is not present. Images are available at the
[MetaShot Docker Hub](https://hub.docker.com/u/metashot/).

<a name="1"></a> [_Ten simple rules for writing Dockerfiles for reproducible data science_]
       (https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1008316)