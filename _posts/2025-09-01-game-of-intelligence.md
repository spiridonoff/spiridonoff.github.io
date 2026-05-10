---
layout: default
title: "Game of Intelligence"
categories: [Research, Mathematics, AI]
permalink: /articles/game-of-intelligence
---

[← Back to Articles](/articles/)

# Game of Intelligence
**Artin Spiridonoff**  
*August 2025*

---

## 1. Introduction
The goal of this article is to pursue an accurate definition of intelligence and attempt to solve it as a mathematical problem.

### Current AI models don't think like humans
It starts with noticing the stark differences between how humans think and how current Artificial Intelligence (AI) models work. They face significant limitations: they are expensive to train, require massive amounts of data, and often struggle with reasoning or hallucinations.

### What is intelligence?
If current AI has shortcomings, what is true intelligence? In my previous writing, I suggested that intelligence can be defined as predicting the unknown given historical samples and current contextual information (the Bayesian Brain Hypothesis). This prediction extends beyond directly observed phenomena to abstract concepts like gravity or laws of motion.

To move beyond a vague definition, I propose that an algorithmic solution for intelligence should ideally have the following properties:
*   It doesn't require global knowledge (implemented in a decentralized manner).
*   It doesn't perform back-propagation.
*   It allows for an adaptive architecture without requiring supervision for every application.
*   **It can handle missing values.**

---

## 2. Game of Intelligence
I propose to define intelligence through a series of progressive mathematical "games," starting simple and increasing in complexity.

#### Game 1: Simple coin toss
Suppose you have a coin, potentially unfair. Before every flip, the player guesses heads or tails. If they are right, they get a score $s=1$, else $s=0$. The goal is to maximize average score per flip $\bar{s}$.
*   *Result:* If $P(\text{heads}) \geq 0.5$, always guessing heads yields $\bar{s}^* = P(\text{heads})$.

#### Game 2: The Player's Perspective
Instead of a single outcome, the player picks a **distribution of outcomes** $q$. The score is the perceived probability of the actual outcome $q(\text{outcome})$.
The average score for fixed $q$ (perceived) and $p$ (actual) is:
$$ \bar{s} = 1 - p(h) + q(h)\big( 2p(h) - 1 \big) $$

#### Game 3: New Scoring (Cross-Entropy)
Total score is now cross-entropy: $H(q,p) = \mathbb{E}_{q(x)}[\ln p(x)]$. This incentivizes the player to pick a distribution that explains outcomes over time, not just in a single round.

#### Game 4: Multiple Coins (Random Vectors)
Represent coins as a random vector $X$. The score is $H(q(X),p(X))$. To estimate the joint probability $p(X)$, we can use the Bayes chain rule:
$$ p(X) = p(X_1)p(X_2 | X_1) \cdots p(X_n | X_{n-1}, \ldots, X_1) $$

#### Game 5: Revealed in Order
In each round, RVs are revealed sequentially as clues (e.g., $X_1, X_2, \ldots$). The goal is to estimate $p(X_i \mid x_{i-1}, \ldots, x_1)$.

#### Game 6: Beyond Fixed Order (The Great Divergence)
Suppose the order of reveals is **not fixed**. There are $n!$ possible orders. Training a different auto-regressive model for each order is unfeasible. We need a solution that handles **missing information** regardless of the reveal sequence—much like how humans make educated guesses with partial data.

#### Game 7: Hidden Variables
What if some variables are never revealed? The player may create an **auxiliary RV** (like "Gravity") to help predict the information that *is* revealed.

#### Game 8, 9, & 10: Complexity and Agency
*   **Game 8:** Observing distributions instead of single outcomes.
*   **Game 9:** Moving beyond Bernoulli to continuous distributions (relevant for vision).
*   **Game 10:** **Agency.** The player picks which variable to reveal next to maximize information gain or survival.

---

## References
*   Hinton, G. (2022). *The Forward-Forward Algorithm*.
*   Spiridonoff, A. (2025). *Toward a Definition of General Intelligence*.
*   Salvatori et al. (2023). *Predictive Coding Survey*.