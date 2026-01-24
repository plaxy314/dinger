---
title: The Born Rule
date: 2026-01-16 10:33:00 -0800
categories: [朝花夕拾, Quantum Mechanics Reimagined]
tags: [quantum mechanics, the born rule]
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

{% include embed/youtube.html id='Ww6dpiJDmIo' %}
