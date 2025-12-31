---
title: Self-Organizing Intelligence
date: 2025-12-30 10:33:00 -0800
categories: [Neural Network Redefined]
tags: [neural network, quantum mechanics, emergent behavior, artificial intelligence]
pin: true
math: true
---

Recent advances in deep learning have produced intelligent systems capable of
recognizing complex patterns, generating coherent text, and performing tasks
once considered the exclusive domain of human cognition[^deep-learning].
Despite their impressive performance, these systems differ fundamentally from
biological intelligence in their reliance on large training datasets, lack of
grounding in the physical world, and absence of intrinsic goals or agency[^ai-foundational-issues].

By contrast, biological systems are self-organizing and intelligence emerges
spontaneously without central planning or explicit training. A striking
example can be seen through the collective behavior of ants. 

{% include embed/youtube.html id='3-98z00A4S8' %}

In this classical piano-movers puzzle [^puzzle-1], the arena is divided into
three chambers connected by two narrow openings. A T-shaped load, designed to
resemble food, is placed in the leftmost chamber. Through coordinated
pushing, pulling, and rotational maneuvers, the ants overcome the spatial
constraints and deliver the load to the chamber near the nest on the right.

{% include embed/youtube.html id='V9aB8963rwM' %}

The second puzzle [^puzzle-2] introduces a new kind of challenge. The arena is
again divided into three sections, but the middle one now contains a gap too
wide for any individual ant to cross. Remarkably, the ants discover a creative
solution: they link their bodies together to form a living bridge, allowing
the continuous transport of food across the gap. 

{% include embed/youtube.html id='zDHp-jV8p4g' %}

Even when a curved path is already laid out for them [^puzzle-2], the ants do
not settle. They continue to explore, seeking the optimal solution that
minimizes the total effort—measured by the number of steps all ants—to carry
the food from the source to the nest.

These ants exhibit a clear form of intelligence. They collectively develop
situational awareness and problem-solving capabilities. In the experiment,
individual ants may be replaced without disrupting the system's overall
performance, indicating that the intelligence does not reside in the brain
of any single ant, but rather emerges from their continuous interactions with
one another and with the environment.

The piano-movers puzzle [^puzzle-1] resembles a minimal neural network: three chambers
correspond to three neurons. Each chambers exists in one of two states:
active when it contains a load and inactive when it is empty. A chamber
becomes active through the coordinated actions of many ants, analogous to
how the synchronized activations of ion channels generate action potentials
in a neuron. The narrow openings connecting chambers function like synapses,
regulating signal (load) transmission from one chambers to the next. The
leftmost chamber serves as input layer, while the rightmost as output layer.

Now imagine scaling the puzzle up: First, divide the arena into roughly
100 billion microscopic cells, each connecting to 1,000–10,000 neighboring
cells. Then, replace the ants in each cell with millions of membrane proteins,
including ion channels and pumps, and neurotransmitter transporters and
receptors. These molecular machines are in constant motion, continuously
interacting with their environment and transporting an enormous number of
ions, neurotransmitters, and signaling molecules in and out of cells.
This forms a vast signal transduction network, the functional equivalent of
the human brain.

The geometric puzzle therefore serves as a good physical model for
understanding the workings of the brain. Our aim is to uncover the principles
that govern the system’s dynamics and the mathematics underlying neural
signal processing.

For a quick overview, see the introductory video *Neural Network Redefined*.

{% include embed/youtube.html id='zg7aA3TsuUs' %}

[^deep-learning]: LeCun, Y., Bengio, Y., & Hinton, G. (2015). *Deep learning*. Nature, 521(7553), 436–444. [doi.org/10.1038/nature14539](https://doi.org/10.1038/nature14539)

[^ai-foundational-issues]: Mumuni, A., & Mumuni, F. (2025). *Large language models for artificial general intelligence (AGI): A survey of foundational principles and approaches*. [arXiv:2501.03151](https://doi.org/10.48550/arXiv.2501.03151)

[^puzzle-1]: Dreyer, T., Haluts, A., Korman, A., Gov, N., Fonio, E., & Feinerman, O. (2025). *Comparing cooperative geometric puzzle solving in ants versus humans*. PNAS, 122(1), e2414274121. [doi.org/10.1073/pnas.2414274121](https://doi.org/10.1073/pnas.2414274121)

[^puzzle-2]: Reid, C. R., Lutz, M. J., Powell, S., Kao, A. B., Couzin, I. D.,& Garnier, S. (2015). *Army ants dynamically adjust living bridges in response to a cost–benefit trade‑off*. PNAS, 112(49), 15113–15118. [doi.org/10.1073/pnas.1512241112](https://doi.org/10.1073/pnas.1512241112)
