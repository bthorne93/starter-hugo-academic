---
title: Variational Autoencoder Model of Galactic Foregrounds
subtitle: A generative model to capture foreground non-Gaussianity
date: 2022-07-20T17:30:28.642Z
summary: We develop a generative model of Galactic dust using a variational
  autoencoder written in Tensorflow, and apply this model to various inverse
  tasks in Bayesian inference, such as data imputation and semantic
  interpolation.
draft: false
featured: false
tags:
  - GAN
  - VAE
categories:
  - Machine Learning
links:
  - url: https://github.com/bthorne93/DustVAEder
    name: Project
    icon_pack: fab
    icon: github
  - url: https://doi.org/10.1093/mnras/stab1011
    name: Paper
    icon_pack: ai
    icon: doi
image:
  filename: featured
  focal_point: Smart
  preview_only: false
---

## Semantic Interpolation 

As a demonstration that our variational autoencoder has learned a compact embedding of the foreground images, we can interpolate between latent embeddings of different images $\mathbf{z}_1 \rightarrow \mathbf{z}_2$. 

An example of semantic interpolation is shown below in Figure 1. The left hand panel is the image encoded to $\mathbf z_1$, and the right hand panel is the image encoded to $\mathbf z_2$. The middle panel shows the smoothly varying interpolated path.

<figure>
<img src="animation-10.gif" style="width:100%">
<figcaption align = "center"><b>Fig.1 - Semantic interpolation between latent embeddings.</b></figcaption>
</figure>