---
title: The Born Rule
date: 2026-01-16 10:33:00 -0800
categories: [朝花夕拾, Quantum Mechanics Reimagined]
tags: [quantum mechanics, the born rule]
pin: false
math: true
---

The dynamics of an ant-foraging system may be described using two complementary methods: the real-valued action density $\rho(x,t)$ and the complex-valued wave function $\psi(x,t)$. Note that position $x$ and time $t$ are not two independent variables. Instead, their evolution along a given path is constrained by the speed of the underlying agent,

$$
c = \frac{x}{t} = \frac{s \cdot \lambda}{s \cdot \tau} = \frac{\lambda}{\tau}.
$$

A physical trajectory traversed by the agent is therefore parametrized by a single physical quantity $s$, which measures the cumulative action along a given path:

$$
x(s) = s \frac{\lambda}{h}, \quad
t(s) = s \frac{\tau}{h}.
$$

Consider a small spacetime interval $\mathrm{d}s$. The amount of action executed within the interval is given by

$$
\mathrm{d}P = \rho(x,t) \, \mathrm{d}s,
$$

which may be geometrically interpreted as the area under the function $\rho(x,t)$ over the spacetime interval $\mathrm{d}s$.

Over the same spacetime interval, the probability amplitude $\psi(x,t)$ evolves as a rotating vector tracing the unit circle. The area swept by the vector is given geometrically by

$$
\mathrm{d}A = \frac{1}{2} |\psi| |d\psi|,
$$

equal to one half the product of the vector’s magnitude and the arc length it traces.

Normalizing this swept area by $\pi$, the area of a unit circle, converts the value of an area into the amount of action:

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

Here, the imaginary unit $i$ in the denominator rotates the resulting vector by $-90^\circ$ clockwise. This operation transforms the complex product to a signed, real value, allowing it to be interpreted as the expected number of net action.

Comparing the two expressions for $\mathrm{d} P$, the action density and the wave function are thus related by

$$
\rho(x,t) = \frac{1}{i2\pi} \bar{\psi}(x,t) \dot{\psi}(x,t),
$$

Since the product $\bar{\psi} \dot{\psi}$ scales quadratically with the amplitude of $\psi$, the probability of observing an action event must be proportional to the squared magnitude of the associated complex amplitude:

$$
P(x,t) \propto \rho(x,t) \propto \left|\psi(x,t)\right|^2.
$$

This relation is often referred to as the Born rule. It can be extended to systems with multiple ants, described by the wave function

$$
\psi(x,t) = A \, e^{i(wt \pm k x)}, \quad A^2 \in \mathbb{Z^+},
$$

where $A^2$ represents the number of ants in the system. 

The Born rule provides the fundamental link between the abstract wave function and the observable action density.
