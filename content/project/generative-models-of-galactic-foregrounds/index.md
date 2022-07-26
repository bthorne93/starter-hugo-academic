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

# Summary 

Emission from the interstellar medium can be a significant contaminant of measurements of the intensity and polarization of thecosmic microwave background (CMB). For planning CMB observations, and for optimizing foreground-cleaning algorithms,a description of the statistical properties of such emission can be helpful. Here, we examine a machine learning approach toinferring the statistical properties of dust from observational data. In particular, we apply a type of neural network called avariational autoencoder (VAE) to maps of the intensity of emission from interstellar dust as inferred fromPlancksky maps anddemonstrate its ability to (i) simulate new samples with similar summary statistics as the training set, (ii) provide fits to emission maps withheld from the training set, and (iii) produce constrained realizations. We find VAEs are easier to train than anotherpopular architecture: that of generative adversarial networks, and are better suited for use in Bayesian inference.

## Training

Our fundamental goal here is to take a set of observations of interstellar dust, $\{ x_1, x_2, \dots, x_N \} \in \mathbb{R}^n$, and infer from them an underlying distribution, $p(x)$, from which they may have been drawn.

Kullback-Leibler divergence: 

$$
\mathbb D_{\rm KL}(q_\phi || p_\theta) = \mathbb{E}_{q_\phi(\mathbf z | \mathbf x)} \left[\log \left[\frac{\log q_\phi(\mathbf z | \mathbf x)}{\log p_\theta(\mathbf z|\mathbf x)} \right] \right] 
$$

## Semantic Interpolation 

As a demonstration that our variational autoencoder has learned a compact embedding of the foreground images, we can interpolate between latent embeddings of different images $\mathbf{z}_1 \rightarrow \mathbf{z}_2$. 

An example of semantic interpolation is shown below in Figure 1. The left hand panel is the image encoded to $\mathbf z_1$, and the right hand panel is the image encoded to $\mathbf z_2$. The middle panel shows the smoothly varying interpolated path.

<figure>
<img src="animation-10.gif" style="width:100%">
<figcaption align = "center"><b>Fig.1 - Semantic interpolation between latent embeddings.</b></figcaption>
</figure>