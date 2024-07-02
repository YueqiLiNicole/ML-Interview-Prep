In probability theory and statistics, **Expectations** (or Expected Values) and **Variance** are two fundamental concepts used to describe the distributions of random variables. These measures give us insights into the central tendency and variability of data.

## Expectations (Expected Value)
The expected value of a random variable gives a measure of the central or typical value we expect to see when we observe the random variable many times. The expected value is essentially a weighted average of all possible values the random variable can take, weighted by their probabilities.

### Calculation
- **For Discrete Random Variables**: If $X$ is a discrete random variable with possible values $x_1, x_2, \dots$ and probability mass function $P(X = x_i)$, then the expectation is given by:
  $$E(X) = \sum_{i} x_i P(X = x_i)$$
  
- **For Continuous Random Variables**: If $X$ is a continuous random variable with probability density function $f(x)$, then the expectation is:
  $$E(X) = \int_{-\infty}^\infty x f(x) \, dx$$
  
- **Properties**:
  - **Linearity**: $E(aX + bY) = aE(X) + bE(Y)$ for any two random variables $X$ and $Y$ and constants $a$ and $b$.
  - Expectations do not necessarily give information about the spread or dispersion of the values.

## Variance
Variance measures how spread out the values of a random variable are around the mean. Essentially, it provides a quantification of the spread of a distribution.

### Calculation
- **Definition**: The variance of a random variable $X$ is the expected value of the squared deviation of $X$ from its mean $E(X)$:

  $$\text{Var}(X) = E\left[(X - E(X))^2\right]$$
  
- **Formula**: This can also be expressed using the linearity of expectation:
$$\text{Var}(X) = E(X^2) - [E(X)]^2$$
  where $E(X^2)$ is the expected value of $X$ squared.

### Properties
- **Non-negativity**: Variance is always non-negative, $\text{Var}(X) \geq 0$.
- **Scale**: $\text{Var}(aX + b) = a^2 \text{Var}(X)$ for any real number $a$ and $b$.
- **Additivity for Independent Variables**: If $X$ and $Y$ are independent, $\text{Var}(X + Y) = \text{Var}(X) + \text{Var}(Y)$.

Together, expectations and variance provide a foundational framework for understanding the behavior of random variables in probability and statistics, informing everything from economics to engineering.
