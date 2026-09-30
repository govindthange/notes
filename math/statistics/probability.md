# 🎲 Probability Cheat Sheet

## I. Basic Probability & Axioms

* Classical Probability Definition: $P(A) = \frac{n(A)}{n(S)}$

* Probability Range: $0 \leq P(A) \leq 1$

* Complementary Event: $P(A') = 1 - P(A)$

* Sure and Impossible Events: $P(S) = 1, P(\emptyset) = 0$

## II. Addition Theorem of Probability

* Addition Rule for Two Events: $P(A \cup B) = P(A) + P(B) - P(A \cap B)$

* Mutually Exclusive Events: $P(A \cup B) = P(A) + P(B)$ (where $P(A \cap B) = 0$)

* Addition Rule for Three Events: $P(A \cup B \cup C) = P(A) + P(B) + P(C) - P(A \cap B) - P(B \cap C) - P(C \cap A) + P(A \cap B \cap C)$

## III. Conditional Probability & Independence

* Conditional Probability: $P(A|B) = \frac{P(A \cap B)}{P(B)}$ (where $P(B) > 0$)

* Multiplication Theorem: $P(A \cap B) = P(A)P(B|A) = P(B)P(A|B)$

* Independent Events Definition: $P(A \cap B) = P(A)P(B)$

* Mutually Independent Events: Events $A, B, C$ are mutually independent if pairwise independent and $P(A \cap B \cap C) = P(A)P(B)P(C)$

## IV. Total Probability & Bayes' Theorem

* Law of Total Probability: $P(A) = \sum_{i=1}^{n} P(A|E_i)P(E_i)$ (where $E_i$ form a partition of sample space $S$)

* Bayes' Theorem: $P(E_i|A) = \frac{P(A|E_i)P(E_i)}{\sum_{j=1}^{n} P(A|E_j)P(E_j)}$

## V. Probability Distributions

* Expectation / Mean of Discrete Random Variable: $E(X) = \sum x_i P(x_i)$

* Variance of Random Variable: $\text{Var}(X) = E(X^2) - [E(X)]^2$

* Binomial Probability Distribution: $P(X = k) = \binom{n}{k} p^k q^{n-k}$ (where $q = 1 - p$)

* Mean of Binomial Distribution: $\mu = np$

* Variance of Binomial Distribution: $\sigma^2 = npq$

## VI. Geometrical Probability & Odds

* Geometrical Probability: $P(A) = \frac{\text{Favorable Measure}}{\text{Total Measure}}$

* Odds in Favor: $\text{Odds in favor} = \frac{P(A)}{P(A')}$

* Odds Against: $\text{Odds against} = \frac{P(A')}{P(A)}$