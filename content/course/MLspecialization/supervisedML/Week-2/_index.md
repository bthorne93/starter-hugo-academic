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
- $\bm x^{(i)}$ is the feature vector of the $i^{th}$ training example. 
- $x_j^{(i)}$ is the $j^{th}$ feature of the $i^{th}$ training example. 

Our model for the data is now: 

$$
f_{w, b}(\bm x) = \bm w \cdot \bm x + b
$$

In the house price regression example, $x_1$ may be the size, $x_2$ may be the number of bedrooms, $x_3$ may be the number of floors, etc... each of the coefficients $w_i$ control the response of the price to each of these feaures. 

Our cost function is then: 

$$
J(\bm w, b) = \frac{1}{2m} \sum_{i=1}^m (f_{\bm w, b}(\bm x^{(i)}) - \bm y^{(i)})^2.
$$

Applying the gradient descent algorithm:

$$
\bm{w}^{i + 1} = \bm{w}^i - \alpha \frac{\partial J(\bm w, b)}{\partial \bm w} \\
b^{i + 1} = b^i - \alpha \frac{\partial J(\bm w, b)}{\partial b}
$$

We can write down an analytic expression for these gradient updates by differentiating the cost function: 

$$
\frac{\partial J(\bm w, b)}{\partial \bm w} = \frac{1}{m} \sum_{i=1}^m (f_{\bm w, b}(\bm x^{(i)}) - \bm y^{(i)}) \bm x^{(i)}
$$

As we have written it here, this is **batch gradient descent**. This means we take the average of the gradient over the entire training dataset before making the update. For small datasets this is fine, but as we move to larger datasets it becomes difficult to fit the entire model and dataset into memory. The alternatives are:

- **Stochastic gradient descent**: where we take a single example at a time to update. 
- **Mini-batch gradient descent**: where we perform gradient updates on mini-batches of data. 

# Practical tips for gradient descent 

## Feature scaling

### Max normalization 

In this case we normalize by the largest value per feature: 

$$
\bm x^{(i)} \rightarrow \bm x^{(i)} / {\rm max}(\bm x)
$$

where the maximum is taken over examples in the training set.

### Mean normalization 

In this case we are normalizing to the interval $(-1, 1)$ for each feature. To do this, we calculate:

$$
\bm x^{(i)} \rightarrow \frac{\bm x^{(i)} - \bm \mu }{{\rm max}(\bm x) - {\rm min}(\bm x)}
$$

### Z-score normalization 

First calculate the mean and standard deviation, and then scale the distribution per feature to the normal distribution. 

$$
\bm x^{(i)} \rightarrow \frac{\bm x^{(i)} - \bm \mu }{\bm \sigma}
$$

## Checking gradient descent for convergence

