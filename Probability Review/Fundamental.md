## Fundamental Concepts

### Sample Space
- **Definition**: The sample space, denoted as $\Omega$, includes all possible outcomes of a probabilistic experiment.
- **Observations**: Individual outcomes within $\Omega$, known as realizations or elements.
- **Events**: Subsets of the sample space which may contain one or more outcomes.

**Example**: In a double coin flip:
  - **Sample Space**: $\Omega = \{HH, HT, TH, TT\}$ where H and T represent heads and tails, respectively.
  - **Event Example**: The event of both flips resulting in the same outcome: $E = \{HH, TT\}$.

### Probability Axioms
The probability of an event $E$ in a sample space $\Omega$ follows these axioms:
1. $P(E) \geq 0$ for every event $E$.
2. $P(\Omega) = 1$.
3. For disjoint events $E_1, E_2, \ldots$, the probability of their union is the sum of their probabilities:
   $$P\left(\bigcup_{i=1}^\infty E_i\right) = \sum_{i=1}^\infty P(E_i)$$

### Joint and Conditional Probabilities
- **Joint Probability**: $P(A, B)$ denotes the probability of both $A$ and $B$ occurring.
- **Conditional Probability**: $P(A \mid B)$ is the probability of $A$ given that $B$ has occurred.
- **Formula**: $P(A, B) = P(A \mid B)P(B) = P(B \mid A)P(A)$.

### Conditional Independence
Events $A$ and $B$ are conditionally independent given $C$ if:
$$P(A, B \mid C) = P(A \mid C)P(B \mid C)$$
