## Advanced Topics

### Marginalization and Total Probability
- **Marginalization**: Allows the computation of the probability of an event $X$ irrespective of the outcomes of another variable $Y$:
  $$P(X) = \sum_Y P(X, Y) = \sum_Y P(X \mid Y)P(Y)$$
- **Total Probability**: Breaks down the probability of $X$ into a sum of probabilities weighted by the probabilities of $Y$.

### Bayes' Rule
A fundamental theorem in probability given by:
$$P(A \mid B) = \frac{P(B \mid A)P(A)}{P(B)}$$
It allows the updating of our belief about $A$ after observing $B$.

### Random Variables
- **Discrete Random Variables**: Take countable values, defined by a probability mass function (PMF).
- **Continuous Random Variables**: Take uncountable values, defined by a probability density function (PDF).

### Distributions
- **Joint Distribution**: Defines the probability distribution for combinations of two or more random variables.
- **Conditional Distribution**: Describes the distribution of a random variable conditioned upon another.

### Independence and IID
- **Independence**: Observations are independent if the occurrence of one does not affect the probability of occurrence of another.
- **Identically Distributed**: Observations are identically distributed if they all come from the same probability distribution.

## Applications in Machine Learning
These probability foundations enable the rigorous application of machine learning techniques, from basic classification to advanced predictive modeling. Understanding these concepts is crucial for designing algorithms that can effectively learn from data and make predictions.

