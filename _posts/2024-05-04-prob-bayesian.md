---
layout: post
title: Probability in Bayesian Perspectives
date: 2024-05-04 10:01:00
description: This article discusses about a fudamental theory of probability in the Bayesian paradigms.
tags: formatting math
categories: sample-posts
related_posts: false
---

### Frequentist vs Bayesian
* Frequentist Probability: Long run frequencies of events.
* Bayesian Probability: Quantifying our uncertainty about something.
  * It can be used to model our uncertainty about events that do not have long term frequencies.
  * E.g. the event that the polar ice cap will melt by 2020.
* The rules of probability are the same for both approaches.

### Sample Space
* Sample space: Set of all possible outcomes of an experiment and is denoted as $\Omega$.
  * $\Omega = \{ 1, 2, 3, 4, 5, 6\}$ is the sample space for the numbers that appear on a dice rolled once.
* Event: A subset of the sample space.
  * If $E = \{ 5 \}$ then $E$ is the event of rolling a 5.
  * If $E = \{J, Q, K\}$ the $E$ represents as the event of getting a face card.

### Union and Intersection
* Union operator, $\cup$: For any events $E$ and $F$ of a sample space $\Omega$, we define the new event $E \cup F$ to consist of all outcomes that are either in $E$ or in $F$ or both $E$ and $F$.
  * If $E = \{1, 5\}$ and $F = \{3\}$ then $E \cup F = \{1,3,5\}$ which might be represented as the event of rolling an odd.
* Intersection, $\cap$: For any two events $E$ and $F$ of a sample space $\Omega$, we define the new event $E \cap F$ to consist of all outcomes that are in both $E$ and $F$.
  * If $E = \{1, 3, 5\}$ and $F = \{3\}$ then $E \cap F = \{3\}$ is the event of rolling a three.
  * If $E = \{J,Q,K\}$ and $F = \{10, K\}$ then $E \cap F = \{K\}$ is the event of getting a King.
  * If $E = \{H\}$ and $F = \{T\}$ then $E \cap F = \emptyset$ would not consist of any outcomes and would thus not occur. If $E \cap F = \emptyset$, then $E$ and $F$ are said to be mutually exclusive ($\emptyset$ is called the empty set).
* Likewise, $\cup_{i=1}^{\infty} E_i$ describes the union of events $E_1, E_2, \cdots$ and corresponds to outcomes that are in $E_i$  for at least one value of $i = 1, 2, \cdots$.
* And $\cap_{i=1}^{\infty}$ describes the intersection of events $E_1, E_2, \cdots$ and corresponds to outcomes that are in all events $E_i, i=1,2,\cdots$.

### Laws of Probability
The probability of event $E$, $\text{Pr}(E)$, is a number satisfying the following three conditions:
1. $0 \leq \text{Pr}(E) \leq 1$.
2. $\text{Pr}(\Omega) = 1$ and $\text{Pr}(\emptyset)=0$.
3. For any sequence of events $E_1, E_2, \cdots$ that are mutually exclusive(i.e., $E_i \cap E_j = \emptyset, i \neq j$), the following holds:

$$ \text{Pr}(\cup_{i=1}^{\infty}E_i)=\sum_{i=1}^{\infty} \text{Pr}(E_i) $$

### Some Properties of Probability Laws
Consider a probability law, and let $E$, $F$, and $G$ be events.
1. If $E \subset F$, then $\text{Pr}(E) \leq \text{Pr}(F)$.
2. $\text{Pr}(E \cup F) = \text{Pr}(E) + \text{Pr}(F) - \text{Pr}(E \cap F).$
3. $\text{Pr}(E \cup F) \leq \text{Pr}(E) + \text{Pr}(F).$
4. $\text{Pr}(E \cup F \cup G) = \text{Pr}(E) + \text{Pr}(E^c \cap F) + \text{Pr}(E^c \cap F^c \cap G).$

### Discrete Random Variables
* Discrete random variable $X$ can take on any value from a finite or countably infinite set $\mathcal{X}$.
* Denote the probability of the event that $X = x$ by $P(X=x)$, or just $P(x)$. Here $P(.)$ is called a probability mass function or pmf. It satifies the properties

\begin{equation}
\label{eq:prop-pmf}
0 \leq P(x) \leq 1, \sum_{x \in \mathcal{X}} P(x) = 1
\end{equation} 

