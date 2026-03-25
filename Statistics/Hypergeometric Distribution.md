---
created: 2025-02-19T17:54:02-05:00
tags:
  - Statistics
---
> [!info] the exact probability model for the number of S’s in the sample

> [!important] when the independent assumption isn't met
- The hypergeometric distribution is good for describing **a finite population** where the population falls into **separate categories.**
	1. finite population
	2. categories (know exactly how many are in each category)
	3. members are independent (if one chemist is chosen then the likilyhood of another being chosen changes)
![[CleanShot 2025-02-20 at 14.58.45@2x.png]]
(r choose y)
num ways you can choose group of n out of capital N
#### EX: X = the # of chemists on the committee of size five What is the probability that we select a committee that has 2 chemists?
 ![[CleanShot 2025-02-20 at 15.01.59@2x.png]]![[CleanShot 2025-02-20 at 15.03.28@2x.png]]
## Conditions of the **hypergeometric distribution**:  
1. The population or set to be sampled consists of a **finite population** of $N$ individuals, objects, or elements
2. Each individual can be characterized as either a **success (S)** or a **failure (F)**, with $M$ successes in the population.  
3. A sample of $n$ individuals is selected **without replacement** such that each subset of size $n$ is equally likely to be chosen.  

---

The random variable of interest is:  
$$
X = \text{the number of successes (S) in the sample}.
$$  

The probability distribution of $X$ depends on the parameters $n$, $M$, and $N$, and is given by:  
$$
P(X = x) = h(x; n, M, N).
$$  
# Formula:
If $X$ is the number of successes (S) in a completely random sample of size $n$ drawn from a population consisting of $M$ successes and $(N - M)$ failures (F)

**hypergeometric distribution**, is given by:  
$$
P(X = x) = h(x; n, M, N) = \frac{\displaystyle \binom{M}{x} \binom{N - M}{n - x}}{\displaystyle \binom{N}{n}}
$$ for $x$ satisfying:  
$$
\max(0, \, n - N + M) \leq x \leq \min(n, M).
$$
## **Mean and Variance of the Hypergeometric Random Variable**  
For a hypergeometric random variable $X$ with pmf $h(x; n, M, N)$:  
- **Mean (Expected Value):**  
  $$
  E(X) = n \cdot \frac{M}{N}
  $$  - **Variance:**  
  $$
  V(X) = \left( \frac{N - n}{N - 1} \right) \cdot n \cdot \frac{M}{N} \cdot \left( 1 - \frac{M}{N} \right)
  $$  

# References:
- [[Probability and Statistics for Engineering and the Sciences, Ninth Edition Jay L. Devore.pdf]]
- [[3.5.2. Hypergeometric Probability Distribution]] youtube video