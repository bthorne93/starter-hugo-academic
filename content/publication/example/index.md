---
title: The Python Sky Model 3 software
authors:
  - Andrea Zonca
  - admin
  - Nicoletta Krachmalnicoff
  - Julian Borrill
author_notes: []
publication_short: In *JOSS*
abstract: >-
  The Python Sky Model (PySM) is a Python package used by Cosmic Microwave
  Background (CMB) experiments to simulate maps, in HEALPix pixelization, of the
  various diffuse astrophysical components of Galactic emission relevant at CMB
  frequencies (i.e. dust, synchrotron, free-free and Anomalous Microwave
  Emission), as well as the CMB itself. These maps may be integrated over a
  given instrument bandpass and smoothed with a given instrument beam. 

  PySM 2, released in 2016, has become the de-facto standard for simulating Galactic emission, for example it is used by CMB-S4, Simons Observatory, LiteBird, PICO, CLASS, POLARBEAR and other CMB experiments, as shown by the 80+ citations of the PySM 2 publication. As the resolution of upcoming experiments increases, the PySM 2 software has started to show some limitations, the solution to these issues was to reimplement PySM from scratch focusing on these features: reimplement all the models with the numba Just-In-Time compiler for Python to reduce memory overhead and optimize performance; use MPI through mpi4py to coordinate execution of PySM 3 across multiple nodes and rely on libsharp, for distributed spherical harmonic transforms; employ the data utilities infrastructure provided by astropy to download the input templates and cache them when requested. 

  At this stage we strive to maintain full compatibility with PySM 2, therefore we implement the exact same astrophysical emission models with the same naming scheme. In the extensive test suite we compare the output of each PySM 3 model with the results obtained by PySM 2.
tags: []
projects: []
slides: ""
url_pdf: ""
publication_types:
  - "2"
image:
  caption: ""
  focal_point: ""
  preview_only: false
summary: Performance improvements of PySM version 3
url_dataset: ""
url_project: ""
url_source: ""
url_video: ""
publication: Journal of Open Source Software
featured: true
date: 2022-07-20T18:20:14.306Z
url_slides: ""
publishDate: 2017-01-01T00:00:00Z
url_poster: ""
url_code: ""
doi: https://doi.org/10.21105/joss.03783
---
