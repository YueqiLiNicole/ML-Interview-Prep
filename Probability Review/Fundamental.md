# Basic Concepts

## Sample Space
- **Definition**: The sample space, denoted as $\Omega$, includes all possible outcomes of a probabilistic experiment.
- **Observations**: Individual outcomes within $\Omega$, known as realizations or elements.
- **Events**: Subsets of the sample space which may contain one or more outcomes.

**Example**: In a double coin flip:
  - **Sample Space**: $\Omega = \{HH, HT, TH, TT\}$ where H and T represent heads and tails, respectively.
  - **Event Example**: The event of both flips resulting in the same outcome: $E = \{HH, TT\}$.

## Random Variable
- **Definition:** A random variable is a function that assigns a real number to each outcome in a sample space of a random process. This mapping from the abstract outcome of a process (like flipping a coin or rolling a dice) to a numerical value allows for more straightforward mathematical treatment.
- **Types of Random Variables**

1. **Discrete Random Variables**:
   - These random variables take on a countable number of distinct values. 
   - Examples include rolling a die (values 1 through 6) or the number of cars passing a checkpoint in an hour (0, 1, 2, 3, ...).

2. **Continuous Random Variables**:
   - These can take on any value within a given range or interval and are typically associated with measurements.
   - Examples include the exact time a train arrives at a station or the amount of rain in a day.
- **Example**
Suppose $X$ is a random variable representing the result of rolling a six-sided die. The possible values of $X$ are 1, 2, 3, 4, 5, and 6, each with a probability of $\frac{1}{6}$.

- $X$ is a discrete random variable.
- The probability distribution of $X$  is uniform since each outcome is equally likely.
- The expected value $E(X)$ would be $\frac{1 + 2 + 3 + 4 + 5 + 6}{6} = 3.5$.

Random variables provide a formal mechanism to study and analyze outcomes quantitatively in the context of probability and statistics.

## Probability Axioms
The probability of an event $E$ in a sample space $\Omega$ follows these axioms:
1. $P(E) \geq 0$ for every event $E$.
2. $P(\Omega) = 1$.
3. For disjoint events $E_1, E_2, \ldots$, the probability of their union is the sum of their probabilities:
   $$P\left(\bigcup_{i=1}^\infty E_i\right) = \sum_{i=1}^\infty P(E_i)$$

## Joint and Conditional Probabilities
- **Joint Probability**: $P(A, B)$ denotes the probability of both $A$ and $B$ occurring.
- **Conditional Probability**: $P(A \mid B)$ is the probability of $A$ given that $B$ has occurred.
- **Formula**: $P(A, B) = P(A \mid B)P(B) = P(B \mid A)P(A)$.

## Conditional Independence
Events $A$ and $B$ are conditionally independent given $C$ if:
$$P(A, B \mid C) = P(A \mid C)P(B \mid C)$$

## Chain Rule

- **Definition:** provides a way to break down the probability of a sequence of interdependent events. It is a direct extension of the basic rule of probability that states the probability of the intersection of two events is the product of the probability of one event and the conditional probability of the other event, given the first.

- **Mathematical Expression**
For a set of $n $random variables $X_1, X_2, \dots, X_n$, the joint probability of these variables can be expressed as:

$$P(X_1, X_2, \ldots, X_n) = P(X_1) \times P(X_2 | X_1) \times P(X_3 | X_1, X_2) \times \ldots \times P(X_n | X_1, X_2, \ldots, X_{n-1})$$

This formula shows how to decompose the probability of a complex event involving multiple variables into simpler, conditional probabilities.

## Bayes' Rule

- **Definition:** Bayes' Rule is a fundamental theorem in probability theory that describes how to update the probability of a hypothesis based on new evidence. It is extensively used in statistics, machine learning, and data analysis to update beliefs or predictions in light of new data.

### Mathematical Expression
Bayes' Rule can be stated as:

$$P(A | B) = \frac{P(B | A) \times P(A)}{P(B)}$$

where:
- $P(A | B)$ is the conditional probability of $A$ given $B$ (posterior probability).
- $P(B | A)$ is the conditional probability of $B$ given $ A$ (likelihood).
- $P(A)$ is the probability of $A$ (prior probability).
- $P(B)$ is the probability of $B$ (marginal probability).

### Calculation of Marginal Probability $P(B)$
The denominator $P(B$ can be challenging to calculate directly in many cases, especially when $B$ depends on several factors. It is often computed using the Law of Total Probability:

$$P(B) = \sum_{i} P(B | A_i) P(A_i)$$

where $A_i$ are the different mutually exclusive cases that cover all possibilities for $A$.

### Applications and Examples

- **Chain Rule**: This rule is essential in scenarios where the probability of a sequence of events is required, such as in speech recognition, genetic sequence analysis, and other sequential analysis tasks.
- **Bayes' Rule**: It is pivotal in Bayesian statistics, where it is used to update the probability estimate for a hypothesis as more evidence or data becomes available. It's fundamental in machine learning models like Naive Bayes classifiers, Bayesian networks, and in various forms of hypothesis testing and decision-making processes in medicine, finance, and law.

These rules not only underpin many statistical methods and models but also provide a framework for reasoning about uncertainty in a coherent and systematic way.
