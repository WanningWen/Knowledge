---
created: 2025-02-19T13:08:11-05:00
tags:
  - Statistics
---
# Definition: ==the study of randomness and uncertainty==
> properties of the population under study are assumed known (e.g., in a numerical population, some specified distribution of the population values may be assumed), and questions regarding a sample taken from the population are posed and answered
- ask and answer questions on the sample without information on population

- ## [[Sample Space]] 
- ## [[Event]]
	- [[Set Theory]]

- Given an experiment and a sample space $\mathcal{S}$, *the **objective of probability** is to assign to each event* $A$ *a number* $P(A)$, called the **probability of the [[Event]]** $A$, *which will give a precise measure of the chance that* $A$ *will occur.* To ensure that probability assignments are consistent with our intuitive understanding of probability, all assignments should satisfy the following axioms (basic properties): ^7f0817
## **Axioms of Probability**
>[!important] The axioms only rule out assignments inconsistent with our intuitive notions of probability, they do not completely determine an assignment of probabilities to events
- **Axiom 1:** For any event $A$,
$$
P(A) \geq 0.
$$
- **Axiom 2:** The probability of the sample space is
$$
P(\mathcal{S}) = 1.
$$
- **Axiom 3:** If $A_1, A_2, A_3, \dots$ is an infinite collection of disjoint events, then
$$
P(A_1 \cup A_2 \cup A_3 \cup \cdots) = \sum_{i=1}^{\infty} P(A_i).
$$
## **Proposition**
$$
P(\varnothing) = 0
$$
$\varnothing$ : null event (the event containing no outcomes whatsoever). 

This implies that  **Axiom 3** is valid for a *finite* collection of disjoint events.
### **Proof**
First, consider the infinite collection:
$$
A_1 = \varnothing, \quad A_2 = \varnothing, \quad A_3 = \varnothing, \dots
$$
Since:
$$
\varnothing \cap \varnothing = \varnothing,
$$
the events in this collection are disjoint, and:
$$
\bigcup A_i = \varnothing.
$$
By **Axiom 3**:
$$
P(\varnothing) = \sum P(\varnothing).
$$

This can occur only if:
$$
P(\varnothing) = 0.
$$

Now suppose that $A_1, A_2, \dots, A_k$ are disjoint events. Append to these the infinite collection:
$$
A_{k+1} = \varnothing, \quad A_{k+2} = \varnothing, \quad A_{k+3} = \varnothing, \dots
$$
Invoking **Axiom 3** again:
$$
P\left( \bigcup_{i=1}^{k} A_i \right) = P\left( \bigcup_{i=1}^{\infty} A_i \right) = \sum_{i=1}^{\infty} P(A_i) = \sum_{i=1}^{k} P(A_i),
$$
as desired.

## [[relative frequency]] of occurence
![[relative frequency]]


## Worksheets:
[probability worksheets](https://www.coconino.edu/resources/files/pdfs/academics/arts-and-sciences/MAT142/Chapter_3_Probability.pdf) 