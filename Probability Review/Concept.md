## Probability Background

### Prior vs. Conditional Probability
- **Prior Probabilities**: Probability of an interpretation prior to seeing any evidence.
- **Conditional (Posterior) Probability**: Probability of an interpretation after taking evidence into account.

### Sample Space and Basic Outcomes
- **Sample Space Ω**: Each element is a possible basic outcome or "possible world" (e.g., the 6 possible rolls of a die).

### Probability Distribution
- A probability distribution assigns a probability to each basic outcome such that Σ P(ω) = 1.0 for every outcome ω in Ω.
- **Events**: An event A is any subset of Ω. The probability of event A is calculated as P(A) = Σ P(ω) for ω in A.
  - E.g., P(die roll <4) = P(1) + P(2) + P(3) = 1/6 + 1/6 + 1/6 = 1/2

### Bayes' Rule and Random Variables
- **Bayes' Rule**: P(A|B) = (P(B|A) * P(A)) / P(B)
- **Conditional Independence**:
  - Two events are independent if P(A) = P(A|B), or equivalently, P(A,B) = P(A) * P(B) if P(B) > 0.
  - Two events are conditionally independent if: P(B,C|A) = P(B|A) * P(C|A) or equivalently, P(B|A,C) = P(B|A) and P(C|A,B) = P(C|A).

