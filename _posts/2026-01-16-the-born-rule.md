---
title: The Born Rule
date: 2026-01-16 10:33:00 -0800
categories: [朝花夕拾, Quantum Mechanics Reimagined]
tags: [quantum mechanics, born rule, superposition]
pin: false
math: true
---

The evolution of a quantum system may be described using two complementary methods: the real-valued action density $\rho(x,t)$ and the complex-valued wave function $\psi(x,t)$. To relate these descriptions, it is important to recognize that position $x$ and time $t$ are not independent variables. They are constrained by the speed of the action agent,

$$
c = \frac{x}{t} = \frac{s \cdot \lambda}{s \cdot \tau} = \frac{\lambda}{\tau},
$$

where $s$ denotes the number of steps along the path. 

Given a stable environmet, the speed $c$ is constant. $x$ and $t$ are thus parameterized by a single spacetime variable $s$:

$$
x(s) = s \lambda, \quad
t(s) = s \tau.
$$

By definition, the amount of action executed by an action agent within a small spacetime interval $\mathrm{d}s$ is given by

$$
\mathrm{d}P = \rho(x,t) \, \mathrm{d}s.
$$

Over the same spacetime interval, $\psi(x,t)$ traces the unit circle in the complex plane. The area swept by the rotating vector is given by

$$
\mathrm{d}A = \frac{1}{2} |\psi| |d\psi|,
$$

equal to one half the product of the vector’s magnitude and the arc length it traces.

Normalizing this swept area by $\pi$, the area of a unit circle, converts the area into the corresponding action increment:

$$
\mathrm{d} P = \frac{1}{2\pi} |\psi| |d\psi|.
$$

Let $\bar{\psi}$ denote the complex conjugate of $\psi$, and $\dot{\psi}$ denote the directional derivative of $\psi$ along an action path, defined as:

$$
\dot{\psi}
\;\equiv\;
\frac{\mathrm{d}\psi}{\mathrm{d}s}
\;=\;
\partial_t \psi\,\frac{\mathrm{d}t}{\mathrm{d}s}
\;+\;
\partial_x \psi\,\frac{\mathrm{d}x}{\mathrm{d}s}
\;\equiv\;
\partial_{\mu}\psi \mathrm{d}x^{\mu}.
$$

With this notation, the action increment may be written as

$$
\mathrm{d} P = \frac{1}{i2\pi} \bar{\psi} \dot{\psi} \, \mathrm{d}s.
$$

Here, the factor $\frac{1}{i}$ corresponds to a $-\frac{\pi}{2}$ rotation in the complex plane. This rotation converts the complex product into a real-valued quantity that can be interpreted as a signed action increment.

Comparing the two expressions for $\mathrm{d} P$, the action density and the wave function are thus related by

$$
\rho(x,t) = \frac{1}{i2\pi} \bar{\psi}(x,t) \dot{\psi}(x,t).
$$

Because the product $\bar{\psi} \dot{\psi}$ scales quadratically with the amplitude of $\psi$, the probability of observing an action event must be proportional to the squared magnitude of the associated complex amplitude:

$$
P(x,t) \propto \rho(x,t) \propto \left|\psi(x,t)\right|^2.
$$

This relation is often referred to as the Born rule and can be extended to systems containing any number of ants:

$$
\psi(x,t) = A \, e^{i(wt \pm k x)}, \quad A^2 \in \mathbb{Z^+},
$$

where $A^2$ represents the number of ants in the system. 

## Superposition

Imagine multiple species of ants foraging within the same environment. Each species, indexed by $n$, is associated with a characteristic action

$$
h_n = E_n \, \tau_n,
$$

where $\tau_n$ denotes the species' mean step duration and $E_n$ the mean energy required for ants of species $n$ to carry out one step.

Each ant step $h_n$ arises from a sequence of biochemical reactions within the ant’s body. These reactions themselves consist of a finite number of atomic-scale actions, such as electron transitions between discrete energy levels. Whenever an electron transitions between two energy levels, a photon is absorbed or emitted, a process associated with a fundamental unit of action, given by Planck’s constant:

$$
h_0 = 6.62607015 \times 10^{-34} \text{J} \cdot \text{s}.
$$

Since the macroscopic action of a single ant step is built from many such discrete microscopic events, it can be expressed as an integer multiple of this fundamental unit:

$$
h_n =  n \, h_0, \quad n \in \mathbb{Z}^+.
$$

The execution of a unit action $h_0$ defines the fundamental frequency for a physical system,

$$
f_0 = \frac{1}{\tau_0},
$$

where $\tau_0$ represents the mean time for the system to complete one Planck's action.

The frequency of an ant action $h_n$ can then be expressed as an integer multiple of that fundamental frequency,

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

The evolution of a multi-species system can be represented by the superposition of all possible sub-systems,

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

Applying the Born rule to the superposed wave function yields the observable action density,

$$
\rho(x,t) = \frac{1}{i2\pi} \bar{\psi}(x,t) \dot{\psi}(x,t).
$$

Integrating the action density over a finite spacetime region produces the expected number of observable (net) actions within that region,

$$
P(x, t) = \int_{t-\frac{\Delta t}{2}}^{t+\frac{\Delta t}{2}}  \int_{x-\frac{\Delta x}{2}}^{x+\frac{\Delta x}{2}} \rho(x', t') \, \mathrm{d}x' \, \mathrm{d}t'.
$$

This provides a unified framework for modeling systems of arbitrary complexity.

> Quantum Mechanics Reimagined (`ant` = `ion channel/pump` =  `action agent`)
{: .prompt-info }
{% include embed/youtube.html id='7-Ge6N0Um2M' %}
