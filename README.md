# Soft-Margin Support Vector Machine from Scratch

A Python implementation of a **Soft-Margin Support Vector Machine (SVM)** from scratch using Lagrange multipliers and quadratic optimization.

## Overview

This project implements a binary Soft-Margin SVM classifier without relying on a pre-built SVM implementation. The model learns a separating hyperplane while allowing some classification errors through the soft-margin formulation.

## Features

- Soft-Margin SVM implementation from scratch
- Lagrange multiplier optimization
- Support vector identification
- Weight vector and bias computation
- Binary classification using a decision function
- Synthetic data generation
- Visualization of the learned decision boundary

## Methodology

The implementation follows the standard Soft-Margin SVM formulation:

1. Generate and normalize synthetic training data.
2. Formulate the SVM optimization problem.
3. Solve for the Lagrange multipliers using quadratic optimization.
4. Identify support vectors from the optimized multipliers.
5. Compute the weight vector and bias.
6. Construct the decision function.
7. Classify samples based on the sign of the decision function.
8. Visualize the resulting decision boundary.

## Mathematical Formulation

The decision function is defined as:

```text
f(x) = w · x + b
