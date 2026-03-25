---
created: 2025-02-19T17:30:10-05:00
tags:
  - Statistics
---
## **Requirements for Experiments**  
1. The experiment consists of a sequence of $n$ smaller experiments called **trials**, where $n$ is fixed in advance of the experiment.  
2. Each trial can result in one of the same two possible outcomes (**dichotomous trials**), generically denoted as:  
   - **Success (S)**  
   - **Failure (F)**  
3. The trials are **independent**, meaning the outcome of any particular trial does **not** influence the outcome of any other trial.  
4. The **probability of success** $P(S)$ is constant from trial to trial,denoted by:     $$
   p = P(S).
   $$
>[!important] In most binomial experiments, we want to know the total number of S’s, rather than knowledge of exactly which trials yielded S’s

# Denoting PMF of Binomial rv $X$ 
The notation:  
$$X \sim \text{Bin}(n, p)$$ or $b(x; n, p)$
means that the random variable $X$ follows a **binomial distribution** with:  
- $n$: Number of independent trials  
- $p$: Probability of success on each trial
## Formula for PMF of Binomial rv $X$:
The **probability mass function (pmf)** of a binomial random variable is given by:  
$$
b(x; n, p) = 
\begin{cases} 
\displaystyle \binom{n}{x} p^x (1 - p)^{n - x} & x = 0, 1, 2, \dots, n \\[10pt]
0 & \text{otherwise}
\end{cases}
$$
where:  
- $n$: Number of trials  
- $x$: Number of successes $(0 \leq x \leq n)$  
- $p$: Probability of success on a single trial  
- $\binom{n}{x}$: Binomial coefficient, representing the number of ways to choose $x$ successes from $n$ trials  
## Formula for CMF of Binomial rv $X$:
For $X \sim \text{Bin}(n, p)$, the **cumulative distribution function (cdf)** is denoted by:  
$$
B(x; n, p) = P(X \leq x) = \sum_{y=0}^{x} b(y; n, p), \quad x = 0, 1, \dots, n
$$  where:  
- $B(x; n, p)$: CDF of the binomial distribution  
- $b(y; n, p)$: PMF of the binomial distribution  
- $x$: Number of successes up to which the probability is accumulated 

## Mean and Variance of $X$ 
if $n = 1$, the binomial distribution becomes a [[Bernoulli random variable|Bernoulli distribution]], where ![[Bernoulli random variable#^aa2c9a]]
Therefore,
### [[Expected value of a Discrete Random Variable|Expected value]] of  a binomial experiment
$E(X) = np$
