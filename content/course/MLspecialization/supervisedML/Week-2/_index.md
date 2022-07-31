---
# Page title
title: "Week 2: Introduction to Machine Learning"

# Page summary for search engines.
summary: Notes on week 2

# Date page published
date: 2022-07-30

type: book

# Position of this page in the menu. Remove this option to sort alphabetically.
weight: 1
---

# Multivariate Linear Regression 

Terminology: 

- $x_j$ is the list of features, $x_j = \{ x_1, x_2, \dots x_n \}$. 
- $n$ is the number of features.
- $\mathbf x^{(i)}$ is the feature vector of the $i^{th}$ training example. 
- $x_j^{(i)}$ is the $j^{th}$ feature of the $i^{th}$ training example. 

Our model for the data is now: 

$$
f_{w, b}(\mathbf x) = \mathbf w \cdot \mathbf x + b
$$

In the house price regression example, $\mathbf x_1$ may be the size, $x_2$ may be the number of bedrooms, $x_3$ may be the number of floors, etc... each of the coefficients $w_i$ control the response of the price to each of these feaures. 
