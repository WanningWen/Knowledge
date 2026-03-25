---
created: 2025-03-03T20:28:54-05:00
tags:
  - Statistics
---
# 📌 Chapter 5 - 

## 🚀 1. Jointly Distributed Random Variables
- If two or more random variables are defined on the **same sample space**, they are **jointly distributed**.
- The **joint probability mass function (PMF)** for discrete random variables \( X \) and \( Y \):
  $$
  P(X = x, Y = y) = f(x, y)
  $$
- The **joint probability density function (PDF)** for continuous random variables:
  $$
  f(x, y) \geq 0, \quad \int \int f(x, y) \, dx \, dy = 1
  $$

## 🚀 2. Marginal Distributions
- The **marginal PMF/PDF** is found by summing or integrating over the other variable:
  - **Discrete Case**:
    $$
    f_X(x) = \sum_{y} f(x, y), \quad f_Y(y) = \sum_{x} f(x, y)
    $$
  - **Continuous Case**:
    $$
    f_X(x) = \int_{-\infty}^{\infty} f(x, y) \, dy, \quad f_Y(y) = \int_{-\infty}^{\infty} f(x, y) \, dx
    $$

## 🚀 3. Conditional Distributions
- The **conditional probability** of \( Y \) given \( X = x \):
  $$
  P(Y = y \mid X = x) = \frac{P(X = x, Y = y)}{P(X = x)}
  $$
- The **conditional density function**:
  $$
  f_{Y|X}(y|x) = \frac{f(x, y)}{f_X(x)}
  $$

## 🚀 4. Independence of Random Variables
- **Two random variables** \( X \) and \( Y \) are **independent** if:
  $$
  P(X = x, Y = y) = P(X = x) P(Y = y)
  $$
  - **For continuous random variables**:
    $$
    f(x, y) = f_X(x) f_Y(y)
    $$
- If \( X \) and \( Y \) are **independent**, then:
  $$
  E[XY] = E[X]E[Y]
  $$

## 🚀 5. Expected Values, Variance, and Covariance
### **(a) Expected Value of a Function of Two Variables**
- If \( g(X, Y) \) is a function of \( X \) and \( Y \), then:
  - **Discrete Case**:
    $$
    E[g(X, Y)] = \sum_{x} \sum_{y} g(x, y) f(x, y)
    $$
  - **Continuous Case**:
    $$
    E[g(X, Y)] = \int \int g(x, y) f(x, y) \, dx \, dy
    $$

### **(b) Variance and Covariance**
- **Variance of \( X \)**:
  $$
  Var(X) = E[X^2] - (E[X])^2
  $$
- **Covariance of \( X \) and \( Y \)**:
  $$
  Cov(X, Y) = E[XY] - E[X]E[Y]
  $$
- **Properties**:
  - If \( Cov(X, Y) > 0 \), then \( X \) and \( Y \) are **positively correlated**.
  - If \( Cov(X, Y) < 0 \), then \( X \) and \( Y \) are **negatively correlated**.
  - If \( Cov(X, Y) = 0 \), then \( X \) and \( Y \) are **uncorrelated** (but not necessarily independent).

## 🚀 6. Correlation Coefficient
- The **correlation coefficient** measures the **strength of the linear relationship** between \( X \) and \( Y \):
  $$
  \rho_{X,Y} = \frac{Cov(X, Y)}{\sigma_X \sigma_Y}
  $$
  - \( \rho = 1 \) indicates a **perfect positive linear relationship**.
  - \( \rho = -1 \) indicates a **perfect negative linear relationship**.
  - \( \rho = 0 \) indicates **no linear relationship**.

## 🚀 7. Joint Moment-Generating Function (MGF)
- The **joint MGF** of \( X \) and \( Y \) is:
  $$
  M_{X,Y}(t_1, t_2) = E[e^{t_1 X + t_2 Y}]
  $$
- **Properties**:
  - If \( X \) and \( Y \) are **independent**, then:
    $$
    M_{X,Y}(t_1, t_2) = M_X(t_1) M_Y(t_2)
    $$

## 🚀 8. Conditional Expectation
- The **expected value of \( Y \) given \( X \)**:
  $$
  E[Y \mid X] = \sum_y y P(Y = y \mid X = x)
  $$
  $$
  E[Y \mid X] = \int y f_{Y|X}(y|x) \, dy
  $$
- **Law of Total Expectation**:
  $$
  E[Y] = E[E[Y \mid X]]
  $$

---

# 📌 Summary of Key Formulas
| Concept                                   | Formula                                                      |      |                                |
| ----------------------------------------- | ------------------------------------------------------------ | ---- | ------------------------------ |
| **Joint PMF (Discrete)**                  | \( P(X = x, Y = y) = f(x, y) \)                              |      |                                |
| **Joint PDF (Continuous)**                | \( \int \int f(x, y) \, dx \, dy = 1 \)                      |      |                                |
| **Marginal PMF (Discrete)**               | \( f_X(x) = \sum_y f(x, y) \)                                |      |                                |
| **Marginal PDF (Continuous)**             | \( f_X(x) = \int f(x, y) \, dy \)                            |      |                                |
| **Conditional PMF**                       | \( P(Y = y \mid X = x) = \frac{P(X = x, Y = y)}{P(X = x)} \) |      |                                |
| **Conditional PDF**                       | \( f_{Y                                                      | X}(y | x) = \frac{f(x, y)}{f_X(x)} \) |
| **Independence**                          | \( P(X = x, Y = y) = P(X = x) P(Y = y) \)                    |      |                                |
| **Expectation of Function \( g(X, Y) \)** | \( E[g(X, Y)] = \sum_x \sum_y g(x, y) f(x, y) \)             |      |                                |
| **Variance**                              | \( Var(X) = E[X^2] - (E[X])^2 \)                             |      |                                |
| **Covariance**                            | \( Cov(X, Y) = E[XY] - E[X]E[Y] \)                           |      |                                |
| **Correlation Coefficient**               | \( \rho = \frac{Cov(X, Y)}{\sigma_X \sigma_Y} \)             |      |                                |
| **Joint MGF**                             | \( M_{X,Y}(t_1, t_2) = E[e^{t_1 X + t_2 Y}] \)               |      |                                |
| **Conditional Expectation**               | \( E[Y \mid X] = \int y f_{Y                                 | X}(y | x) \, dy \)                    |
| **Law of Total Expectation**              | \( E[Y] = E[E[Y \mid X]] \)                                  |      |                                |

---

Let me know if you need additional details or specific examples! 🚀