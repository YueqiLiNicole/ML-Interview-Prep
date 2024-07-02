# Probability Review for Machine Learning

## Motivation
- Uncertainty in machine learning arises from:
  - Noisy measurements
  - Variability between samples
  - Finite size of data sets
- Probability theory provides a consistent framework for quantifying and managing uncertainty.

## Sample Space
- **Definition**: The sample space \( \Omega \) is the set of all possible outcomes of an experiment.
- **Observations**: Points in the sample space, also known as sample outcomes or realizations.
- **Events**: Subsets of the sample space.
- **Example**: For a double coin flip, the sample space \( \Omega = \{HH, HT, TH, TT\} \).

## Probability Axioms
1. \( P(E) \geq 0 \) for every event E.
2. \( P(\Omega) = 1 \).
3. For disjoint events \( E_1, E_2, \ldots \):
   \[ P\left(\bigcup_{i=1}^\infty E_i\right) = \sum_{i=1}^\infty P(E_i) \]

## Joint and Conditional Probabilities
- **Joint Probability**: \( P(A, B) \) denotes the probability of both A and B occurring.
- **Conditional Probability**: \( P(A \mid B) \) is the probability of A given that B has occurred.
- Formula: \( P(A, B) = P(A \mid B)P(B) = P(B \mid A)P(A) \)

## Conditional Independence
- Events A and B are conditionally independent given C if:
  \[ P(A, B \mid C) = P(A \mid C)P(B \mid C) \]

## Marginalization and Total Probability
- **Marginalization**:
  \[ P(X) = \sum_Y P(X, Y) = \sum_Y P(X \mid Y)P(Y) \]
- **Total Probability** provides a way to calculate the probability of X via its relationship with Y.

## Bayes' Rule
\[ P(A \mid B) = \frac{P(B \mid A)P(A)}{P(B)} \]

## Random Variables
- **Discrete**: Takes countable values, probability defined by a probability mass function (PMF).
- **Continuous**: Takes uncountable values, probability defined by a probability density function (PDF).

## Distributions
- **Joint Distribution**: For variables X and Y, defines probabilities across combinations of X and Y.
- **Conditional Distribution**: Defines the distribution of X given Y.

## Independence
- Observations are independent and identically distributed (i.i.d.) if sampled from the same distribution and are independent.

## Notation and Probability Distributions
- Common notations and simplifications in machine learning:
  - Random variables in lower case.
  - Use of p for PMFs/PDFs.
  - Often omit ranges of integration for clarity.

## Gaussian Distribution
- **Univariate Gaussian**: Defined by mean (µ) and variance (σ²).
- **Multivariate Gaussian**: Defined by a mean vector and a covariance matrix.

## Inferring Parameters
- **Maximum Likelihood Estimation (MLE)**: Method to estimate parameters of a distribution that make the observed data most probable.

## MLE for Gaussian Distribution
- Describes the process of estimating the mean and variance from data using the likelihood and log-likelihood functions.
