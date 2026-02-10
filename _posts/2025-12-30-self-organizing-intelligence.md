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
biological systems in their reliance on large training datasets, lack of
grounding in the physical world, and absence of intrinsic goals or agency.

Biological systems, by contrast, are self-organizing, with intelligence emerging
spontaneously without central planning or explicit training. A striking example can be seen through the behavior of ant colonies.

{% include embed/youtube.html id='3-98z00A4S8' %}

The video above presents a classical "piano-movers" puzzle[^puzzle-1]. The arena is divided into three chambers connected by two narrow openings. A T-shaped load, designed to resemble food, is initially placed in the leftmost chamber. Through coordinated pushing, pulling, and rotational maneuvers, the ants negotiate the spatial constraints and deliver the load to the chamber adjacent to the nest on the right.

The puzzle below [^puzzle-2] introduces a more challenging configuration. The arena is again divided into three sections, but the central section is a gap too wide for any individual ant to cross. Remarkably, the ants discover a creative
solution: they link their bodies together to form a living bridge, allowing
the continuous transport of food across the gap. 

{% include embed/youtube.html id='V9aB8963rwM' %}

Even when a curved path is provided by default, the ants are unsatisfied with this suboptimal solution. They continue to explore, favoring routes that reduce the system’s overall foraging cost.

{% include embed/youtube.html id='zDHp-jV8p4g' %}

These ant-foraging systems exhibit a clear form of intelligence, characterized by collective situational awareness and problem-solving capabilities. In the experiment, individual ants can be replaced without disrupting the system's overall performance, indicating that the intelligence does NOT reside in the brain of any single ant, but rather emerges from their continuous interactions with one another and with the environment.

A close parallel can be drawn between the "piano-movers" puzzle[^puzzle-1] and a biological neural network. The three chambers represent three neurons, and the narrow openings between chambers correspond to synapses that regulate the transmission of action signals. Each chamber exists in one of two possible states: active when it contains a load and inactive when it is empty. A chamber becomes activated through the coordinated actions of many ants, analogous to how synchronized ion-channel activity triggers an action potential in a biological neuron.

In this network, the leftmost chamber, open to the food, serves as the input layer, while the rightmost chamber near the nest serves as the output layer. The network transforms an input signal into an output signal by timeshifting and attenuating it as the signal passes through the intermediate layer. Now imagine scaling this network up:

The arena is divided into roughly 100 billion microscopic chambers by ultra-thin membranes, with each chamber connected to 1,000–10,000 neighbors. Embedded in the membrane of each chamber are millions of ion channels and pumps, neurotransmitter transporters and receptors, and other membrane proteins. These molecular machines are in constant motion, busy transporting ions, neurotransmitters, and signaling molecules across a complex network of membranes—much like ants foraging tirelessly for food in a complex environment.

Individually, these molecular interactions may appear random, but together they form a vast signal-transduction network that gives rise to large-scale coherent behaviors. Our goal is to understand the physical laws that govern the dynamics of such systems. These laws underlie the mathematical foundation of neural computation. Before diving into the formalism, it is helpful to develop a high-level, intuitive understanding of how these systems operate in practice. The following video illustrates how simple, ordinary objects can self-organize to perform complex computations.

> Neural Network Redefined (`ant` = `ion channel/pump` =  `action agent`)
{: .prompt-info }
{% include embed/youtube.html id='q2VHfX8PyoU' %}

[^deep-learning]: LeCun, Y., Bengio, Y., & Hinton, G. (2015). *Deep learning*. Nature, 521(7553), 436–444. [doi.org/10.1038/nature14539](https://doi.org/10.1038/nature14539)

[^puzzle-1]: Dreyer, T., Haluts, A., Korman, A., Gov, N., Fonio, E., & Feinerman, O. (2025). *Comparing cooperative geometric puzzle solving in ants versus humans*. PNAS, 122(1), e2414274121. [doi.org/10.1073/pnas.2414274121](https://doi.org/10.1073/pnas.2414274121)

[^puzzle-2]: Reid, C. R., Lutz, M. J., Powell, S., Kao, A. B., Couzin, I. D.,& Garnier, S. (2015). *Army ants dynamically adjust living bridges in response to a cost–benefit trade‑off*. PNAS, 112(49), 15113–15118. [doi.org/10.1073/pnas.1512241112](https://doi.org/10.1073/pnas.1512241112)
