---
layout: default
title: "Toward a Definition of General Intelligence"
categories: [AI, Philosophy, Research]
permalink: /articles/toward-general-intelligence
---

[← Back to Articles](/articles/)


# Toward a Definition of General Intelligence
**Artin Spiridonoff**  
*May 2025* |
View this article on [Medium](https://medium.com/@artin.spiridonoff/toward-a-definition-of-general-intelligence-2f8237a75141)

## Abstract
This article explores the concept of general intelligence and proposes a preliminary mathematical framework to define and model it. We contrast biological intelligence with current artificial intelligence systems and argue for a rethinking of how we define and pursue artificial general intelligence.

---

## 1. Introduction
Intelligence remains one of humanity's greatest mysteries. While we often claim superiority in intelligence over other species, we lack a clear definition - let alone a full understanding - of how it works.
The recent rise of generative artificial intelligence (AI), particularly tools like ChatGPT, has brought renewed attention to this topic. Despite impressive advances, these systems are still far from achieving true general intelligence.
In this paper, I outline limitations of current AI paradigms, then propose a mathematical lens through which we might define and study general intelligence more rigorously.

---

## 2. Current AI and Its Limitations
While recent AI systems show remarkable capabilities, they face several key challenges:
Scale: Model sizes are growing rapidly. GPT-4, for example, comprises eight models, each with 220 billion parameters.
Data Requirements: These large models demand vast training datasets, which may soon become insufficient.
Cost: Training state-of-the-art models is increasingly expensive - GPT-4 reportedly cost \$63 million.
Energy Consumption: AI training is power-intensive. Tech companies are investing in nuclear energy to meet future demands.

These trends raise concerns about the sustainability of current approaches. The human brain, by contrast, is highly efficient: it contains approximately 86 billion neurons and learns effectively from far fewer examples, with dramatically lower energy use. It operates on roughly 20 watts of power - less than a light bulb - yet it supports lifelong learning, abstraction, memory, and multi-modal reasoning. By contrast, modern AI models require megawatt-scale GPU clusters to perform inference and learning tasks that humans accomplish with ease.
If we aim to build general intelligence, we may need a fundamental shift in how we approach learning systems.

---

## 3. Defining Intelligence
### 3.1 Intelligence as Survival-Oriented Processing
At its core, biological intelligence is a system that receives sensory input, processes it, and takes actions to increase its chances of survival. Survival here includes behaviors such as avoiding danger, acquiring resources, reproducing, and protecting offspring.
Many such behaviors are not the result of conscious reasoning. Reflexes like fight-or-flight likely originated from evolved decision-making mechanisms. Over time, natural selection retained only those responses aligned with survival, regardless of how they were generated.
### 3.2 Intelligence as Predictive Understanding
We can define intelligence more generally as the ability to model the environment and make effective decisions. This entails prediction - estimating outcomes of actions - and decision-making - choosing actions that maximize a goal, such as survival.
This predictive ability aligns with the Bayesian brain hypothesis, which posits that the brain continuously updates probabilistic models of the world, using sensory input to minimize prediction errors. From this perspective, intelligence can be seen as the optimization of belief updates under uncertainty.
Consider a simplified formulation:
Problem 1: Given prior experiences with complete observed pairs $((x_i, y_i) \sim (X, Y))$, predict $(Y)$ for a new instance $(x \sim X)$.
This resembles standard supervised learning. However, it differs from real-world intelligence in key ways:
The target $(Y)$ is not fixed; it depends on context.
Observations may be incomplete; not all variables are observed at once.

A more general framing is:
Problem 2: Given prior experiences with incomplete observations $(\{x_i \sim X_i\})$, predict $(X_j)$ for any $(j)$, conditioned on the other $(\{x_i \mid i \neq j\})$.
This formulation more closely mirrors biological cognition. Humans observe the world through imperfect, partial sensory channels, yet we make coherent inferences.
### 3.3 Abstract Reasoning and Latent Variables
Humans can infer unobserved concepts to better model the world. For example, from patterns in motion, Newton inferred gravity - a variable not directly sensed. Such abstractions improve prediction and understanding.
Newton contemplates the falling apple - not just as an observation, but as a clue to an unseen force. This image symbolizes the essence of general intelligence: the human ability to infer hidden variables and form abstract models of the world.This capacity for abstraction corresponds to what psychologists call System 2 cognition - slow, deliberate, and symbolic reasoning - distinct from the fast, pattern-based System 1 processes. While most current AI excels at System 1-style tasks (pattern recognition, statistical inference), general intelligence likely requires integrating both.
Crucially, any prediction about unobservable variables depends on assumed relationships with observed ones. Thus, intelligence involves hypothesizing structure where it cannot be directly confirmed.
### 3.4 Agency and Active Learning
A key aspect of human intelligence is agency: the capacity to act. We do not passively observe; we intervene, explore, and manipulate our environments to learn and survive.
This aligns with theories of active inference in neuroscience, where agents not only predict sensory input but act to reduce expected uncertainty. That is, action and perception are tightly coupled in minimizing prediction error - a concept increasingly influential in robotics and AI.
### 3.5 Transfer and Meta-Learning
A defining feature of general intelligence is the ability to generalize across domains. Humans routinely transfer knowledge from one context to another, a process known as transfer learning. Moreover, we engage in meta-learning - learning how to learn - by identifying patterns in how tasks relate. Modern AI systems often lack this flexibility, as they must be retrained for new tasks and environments from scratch. Bridging this gap is key to developing systems that exhibit true generality.

---

## 4. Conclusion
General intelligence may be best characterized as the ability to form abstract representations from incomplete data, make flexible predictions, and take effective actions in pursuit of complex goals such as survival or understanding. Current AI systems, while powerful, lack many of these traits.
This article offers a mathematical perspective to ground future research and invites further exploration of agency, abstraction, and efficient learning as cornerstones of intelligence.
This article was reviewed and polished by an artificial - not so general - intelligence model.

---

## 5. References
- https://www.nature.com/articles/d41586-024-03990-2
- https://www.nei.org/news/2024/tech-companies-and-their-love-of-nuclear