---
title: The Born Rule
date: 2026-01-16 10:33:00 -0800
categories: [朝花夕拾, Quantum Mechanics Reimagined]
tags: [quantum mechanics, born rule, superposition]
pin: false
math: true
---

The dynamics of an ant-foraging system may be described using two complementary methods: the real-valued action density $\rho(x,t)$ and the complex-valued wave function $\psi(x,t)$. To relate these two descriptions, it is necessary to realize that position $x$ and time $t$ are not independent variables. Instead, their evolution along a given path is constrained by the speed of the underlying agent,

$$
c = \frac{x}{t} = \frac{s \cdot \lambda}{s \cdot \tau} = \frac{\lambda}{\tau}.
$$

An action path is therefore parametrized by $s$, the cumulative action along that path:

$$
x(s) = \frac{s}{h} \lambda, \quad
t(s) = \frac{s}{h} \tau.
$$

Consider a small spacetime interval $\mathrm{d}s$. The amount of action accrued within the interval is given by

$$
\mathrm{d}P = \rho(x,t) \, \mathrm{d}s,
$$

which may be geometrically interpreted as the area under $\rho(x,t)$ over the spacetime interval $\mathrm{d}s$.

Over the same spacetime interval, $\psi(x,t)$ evolves as a rotating vector tracing the unit circle in the complex plane. The area swept by the rotating vector is given geometrically by

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

Here, division by the imaginary unit $i$ rotates the complex product by $90^\circ$ clockwise. This operation transforms it to a real-valued quantity, allowing it to be interpreted as the signed action increment.

Comparing the two expressions for $\mathrm{d} P$, the action density and the wave function are thus related by

$$
\rho(x,t) = \frac{1}{i2\pi} \bar{\psi}(x,t) \dot{\psi}(x,t),
$$

Since the product $\bar{\psi} \dot{\psi}$ scales quadratically with the amplitude of $\psi$, the probability of observing an action event must be proportional to the squared magnitude of the associated complex amplitude:

$$
P(x,t) \propto \rho(x,t) \propto \left|\psi(x,t)\right|^2.
$$

This relation is often referred to as the Born rule. It can be extended to systems with multiple ants, corresponding to the wave function

$$
\psi(x,t) = A \, e^{i(wt \pm k x)}, \quad A^2 \in \mathbb{Z^+},
$$

where $A^2$ represents the number of ants in the system. 

The Born rule provides the fundamental link between the abstract wave function and the observable action density.

## Superposition

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

Applying the Born rule to the superposed wave function yields the observable action density,

$$
\rho(x,t) = \frac{1}{i2\pi} \bar{\psi}(x,t) \dot{\psi}(x,t).
$$

Integrating this density over a finite spacetime region produces the expected number of net actions observable within that region,

$$
P(x, t) = \int_{t-\frac{\Delta t}{2}}^{t+\frac{\Delta t}{2}}  \int_{x-\frac{\Delta x}{2}}^{x+\frac{\Delta x}{2}} \rho(x', t') \, \mathrm{d}x' \, \mathrm{d}t'.
$$

This formalism provides a unified description of quantum systems of arbitrary complexity.

> Quantum Mechanics Reimagined (`ion channel/pump` = `ant` = `any step motor`)
{: .prompt-info }
{% include embed/youtube.html id='7-Ge6N0Um2M' %}
