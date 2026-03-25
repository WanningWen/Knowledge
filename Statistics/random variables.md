---
created: 2025-02-19T16:15:14-05:00
tags:
  - Statistics
---
# Definition #definition
For a given sample space $S$ of some experiment, a **random variable (RV)** is any rule that associates a number with each outcome in $S$.  

In mathematical terms, a random variable is a **function**:  
$$
X: S \to \mathbb{R},
$$
where the **domain** is the sample space $S$, and the **range** is the set of real numbers $\mathbb{R}$.
### graphical representation:
![[CleanShot 2025-02-19 at 16.22.31@2x.png]]


# Denotation: uppercase letters (ex: $X$ and $Y$)
Random variables are customarily denoted by uppercase letters, such as $X$ and $Y$, near the end of the alphabet.  

**lowercase letters to represent specific values of the corresponding random variable**.  
$$X(\omega) = x$$
means that $x$ is the value associated with the outcome $\omega$ by the random variable $X$.

### [[Bernoulli random variable]]


#### possible values of random variables ex 3.4:
Consider an experiment in which 9-volt batteries are tested until one with an acceptable voltage $(S)$ is obtained.  

The sample space is:  
$$
\mathcal{S} = \{ S, FS, FFS, \dots \}.
$$

Define a random variable $X$ as:  
$$
X = \text{the number of batteries tested before the experiment terminates.}
$$

Then:  
$$
X(S) = 1, \quad X(FS) = 2, \quad X(FFS) = 3, \dots, \quad X(FFFFFFS) = 7, \quad \text{and so on.}
$$
Any positive integer is a possible value of $X$, so the set of possible values is **infinite**.

## [[Discrete Random Variables]]

## [[continuous random variables]]
