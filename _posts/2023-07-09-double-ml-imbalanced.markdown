---
title: "Double-debiased machine learning with unbalanced treatment assignment"
layout: post
date: 2023-08-02 22:48
image: /assets/images/markdown.jpg
headerImage: false
tag:
- causal-ml
- undersampling
- ate
category: blog
author: danieleballinari
description: Adjusting for unbalanced treatment assignment in double-debiased machine learning
---

## Introduction
In the realm of highly unbalanced classification problems, training machine learning models to predict the minority class can be a daunting task. Interestingly, this issue also extends to causal inference. The popular double-debiased machine learning approach for estimating causal effects is sensitive to unbalanced treatment assignment. In this blog post, I will explore how to address this concern and adjust for unbalanced treatment assignment when employing the double-debiased machine learning approach.

I'll start with a concise review of the double-debiased estimator, highlighting its core principles. Then, I'll delve into different methods for adjusting unbalanced treatment assignment, with a focus on a new approach based on undersampling. Remarkably, this method preserves the favorable asymptotic properties of the double-debiased approach.

To illustrate the impact of unbalanced treatment assignment, I'll present the findings of a small simulation study. This study will underscore the sensitivity of the double-debiased estimator and showcase how the proposed adjustment can mitigate bias effectively.

Furthermore, I'll extend the simulation to evaluate the performance of these adjustment in a decision-making scenarios where we try to find an optimal policy to assign treatments.

The code for this blog post is available on [GitHub](https://github.com/dballinari/simulation-unbalanced-treatment).
