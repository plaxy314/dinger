---
title: Self-Organizing Intelligence
date: 2025-12-30 10:33:00 -0800
categories: [朝花夕拾, Introduction]
tags: [neural network, quantum mechanics, emergent behavior, artificial intelligence]
pin: true
math: true
---

Recent advances in deep learning have produced intelligent systems capable of
recognizing complex patterns, generating coherent text, and performing tasks
once considered the exclusive domain of human cognition[^deep-learning].
Despite their impressive performance, these systems differ fundamentally from
biological intelligence in their reliance on large training datasets, lack of
grounding in the physical world, and absence of intrinsic goals or agency.

By contrast, biological systems are self-organizing, with intelligence emerging
spontaneously without central planning or explicit training. A striking example
is the collective behavior of ants. 

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

Even when a curved path is already laid out for them, the ants do not settle. They continue to explore, seeking the most efficient route that minimizes the total effort of foraging—measured by the number of steps taken by all ants.

These ants exhibit a clear form of intelligence. They collectively develop situational awareness and problem-solving capabilities. In the experiment, individual ants may be replaced without disrupting the system's overall performance, indicating that the intelligence does **not** reside in the brain of any single ant, but rather emerges from their continuous interactions with one another and with the environment.

The piano-movers puzzle implements a minimal neural network, where three chambers correspond to three neurons and the narrow openings between chambers function as synapses, allowing action signals (i.e., the transport of a load) to propagate from one chamber to the next. Each chamber exists in one of two states: active when it contains a load, and inactive when it is empty. A chamber becomes active through the coordinated actions of many ants, much like how an action potential is triggered in a biological neuron through the synchronized activities of ion channels. In this neural network, the chamber open to the food serves as the input layer, while the chamber near the nest serves as the output layer.

Now imagine scaling this network up. First, divide the arena into roughly 100 billion microscopic cells, each connected to 1,000–10,000 neighboring cells. Then, replace the ants within each cell with millions of molecular machines—ion channels and pumps, neurotransmitter transporters and receptors, and other membrane proteins. These molecular machines are in constant motion, continuously interacting with their environment and transporting vast numbers of ions, neurotransmitters, and signaling molecules across cell membranes. Together, they form a vast signal-transduction network, comparable in the scale to the human brain.

Our goal is to uncover the principles governing the dynamics of such systems and to understand their collective behavior through the lens of signal processing. Before turning to the technical discussion, readers may find it helpful to watch this introductory video, which provides a high-level overview of the ideas to be developed here.

> Neural Network Redefined (`ant` = `ion channel/pump` =  `action agent`)
{: .prompt-info }
{% include embed/youtube.html id='q2VHfX8PyoU' %}

[^deep-learning]: LeCun, Y., Bengio, Y., & Hinton, G. (2015). *Deep learning*. Nature, 521(7553), 436–444. [doi.org/10.1038/nature14539](https://doi.org/10.1038/nature14539)

[^puzzle-1]: Dreyer, T., Haluts, A., Korman, A., Gov, N., Fonio, E., & Feinerman, O. (2025). *Comparing cooperative geometric puzzle solving in ants versus humans*. PNAS, 122(1), e2414274121. [doi.org/10.1073/pnas.2414274121](https://doi.org/10.1073/pnas.2414274121)

[^puzzle-2]: Reid, C. R., Lutz, M. J., Powell, S., Kao, A. B., Couzin, I. D.,& Garnier, S. (2015). *Army ants dynamically adjust living bridges in response to a cost–benefit trade‑off*. PNAS, 112(49), 15113–15118. [doi.org/10.1073/pnas.1512241112](https://doi.org/10.1073/pnas.1512241112)
