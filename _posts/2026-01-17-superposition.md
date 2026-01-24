---
title: ---
title: Superposition
date: 2026-01-17 10:33:00 -0800
categories: [朝花夕拾, Quantum Mechanics Reimagined]
tags: [quantum mechanics, superposition]
pin: false
math: true
---

Imagine multiple species of ants foraging within the same environment. Each species, indexed by $n$, is associated with a characteristic action

$$
h_n = E_n \, \tau_n,
$$

where $\tau_n$ denotes the species' mean step duration and $E_n$ the mean energy required for the species to complete a single step.

Each ant step $h_n$ arises from a series of biochemical reactions. Each biochemical reaction, in turn, consists of a sequence of electron transitions between discrete energy levels at the atomic level. Each transition is associated the absorption or emission of a photon, a fixed physical action quantifiable by Planck’s constant,

$$
h_0 = 6.62607015 \times 10^{-34} \text{J} \cdot \text{s}.
$$

Therefore, the macroscopic action $h_n$ can be expressed as an integer multiple of this fundamental unit of action,

$$
h_n =  n \, h_0, \quad n \in \mathbb{Z}^+.
$$

The execution of a single Planck's action $h_0$ defines a natural clock tick for the system. This internal clock runs at the fundamental frequency

$$
f_0 = \frac{1}{\tau_0},
$$

where $\tau_0$ is the mean time for the system to execute one unit Planck's action.

An ant action $h_n$ can thus be associated with a pair of frequencies,

$$
f_n^{\pm} = \pm  \frac{h_n}{h_{0}} f_0 = \pm n f_0,
$$

and the corresponding angular frequencies,

$$
\omega_n^{\pm} =  2 \pi f_n^{\pm}.
$$

The opposite signs indicate that the same action may unfold in opposite directions in space.

Let $\lambda_n$ denote the mean step length of $h_n$. The corresponding wavenumber,

$$
k_n =  2 \pi \lambda_n,
$$

measures the spatial frequency of $h_n$.

The spacetime evolution of a multi-species system can then be represented as the superposition of all possible sub-systems,

$$
\psi(x,t) =  \sum_n c_n \psi_n(x,t),
$$

where the wave function

$$
\psi_n(x,t) =  e^{i(\omega_n^{\pm} t \pm k_n x)},
$$

tracks the spacetime evolution of species $n$. The complex coefficient

$$
c_n =  A_n e^{i \theta_n}  
$$

specifies its configuration: $A_n^2$ represents the expected number of actions (o ants) of species $n$ per unit spacetime, while the phase $\theta_n$ encodes their action progression or spatial offset relative to other species. For species absent from the system, $A_n=0$. The coefficient $c_0$ encode the system's bias.

{% include embed/youtube.html id='x63UcRw7sOU' %}

Applying the Born rule to the superposed wave function yields the observable action density,

$$
\rho(x,t) = \frac{1}{i2\pi} \bar{\psi}(x,t) \dot{\psi}(x,t).
$$

Integrating this density over a finite spacetime region produces the expected number of net actions observable within that region,

$$
P(x, t) = \int_{t-\frac{\Delta t}{2}}^{t+\frac{\Delta t}{2}}  \int_{x-\frac{\Delta x}{2}}^{x+\frac{\Delta x}{2}} \rho(x', t') \, \mathrm{d}x' \, \mathrm{d}t'.
$$

This formalism provides a unified description of quantum systems of arbitrary complexity.

{% include embed/youtube.html id='yRkfwKPO6ik' %}
