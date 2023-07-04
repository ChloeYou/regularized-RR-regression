## ☕ Regularized Binary Regression Model for Relative Risk

🎯 We develop an algorithm that extends on the [`rbrm`](https://github.com/mclements/brm) package to estimate relative risk.

📖 The original model is based on the [regularized binary regression model](https://arxiv.org/abs/1510.02430) (rbrm) paper by Thomas S. Richardson, James M. Robins, Linbo Wang.

#### 📂 This repository contains the following files

* `rbrm.r`: contains the R function for the algorithm
* `cv.rbrm.r`: contains the R function for performing cross-validation
* `helper.r`: contains some helper functions

#### 💡 Abstract

Binary regression models, such as Poisson and logistic regression, are commonly employed in clinical studies to estimate measures like relative risks (RR) or odds ratios (OR). While RR are preferred for their straightforward interpretation, logistic regression, which models OR, is the most widely used approach. However, it only provides a reliable estimate of RR when the outcome of interest is infrequent. Meanwhile, the Poisson regression can estimate RR directly but can produce fitted probabilities outside the range of zero and one. To address these challenges, Richardson et al. (2017) proposed a novel binary regression model that estimates RR directly via a log odds-product nuisance model. However, this model also has limitations in estimating high-dimensional data (p > N). Therefore, we propose a new estimator and develop an algorithm of the binary regression model that allows variable selection when p > N. Finally, we examine the properties of our estimator in a simulation study.
