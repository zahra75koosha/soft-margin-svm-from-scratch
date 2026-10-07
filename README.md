# Soft-Margin Support Vector Machine from Scratch

A Python implementation of a **Soft-Margin Support Vector Machine (SVM)** from scratch using Lagrange multipliers and quadratic optimization.

## Overview

This project implements a binary Support Vector Machine classifier without relying on a pre-built SVM classifier. The model learns a separating hyperplane for linearly separable and overlapping data while allowing classification errors through the soft-margin parameter.

## Features

- Soft-margin SVM implementation
- Lagrange multiplier optimization
- Identification of support vectors
- Computation of the weight vector and bias
- Binary classification using the sign of the decision function
- Synthetic data generation for model evaluation
- Visualization of the learned decision boundary

## Methodology

The implementation follows the standard soft-margin SVM formulation:

1. Generate and normalize synthetic training data.
2. Formulate the SVM optimization problem.
3. Solve for the Lagrange multipliers.
4. Identify support vectors from non-zero multipliers.
5. Compute the weight vector and bias.
6. Project data points onto the learned hyperplane.
7. Classify samples using the sign of the decision function.

## Main Components

### Lagrange Multipliers

The optimization problem is solved to obtain the Lagrange multipliers associated with the training samples.

### Support Vectors

Samples with non-zero Lagrange multipliers are identified as support vectors. These points determine the position of the decision boundary.

### Decision Function

The model computes:

```text
f(x) = w · x + b
