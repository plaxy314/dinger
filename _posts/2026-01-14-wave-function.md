---
title: Wave Function
date: 2026-01-14 10:33:00 -0800
categories: [朝花夕拾, Quantum Mechanics Reimagined]
tags: [quantum mechanics, wave function, Schrödinger's equation]
pin: false
math: true
---

The execution of the unit action $h$ along a particular path may be represented by a rotating vector that traces the unit circle in the complex plane, using Euler's formula:

$$
\psi(\theta) = e^{i \theta} = \cos\theta + i \sin\theta,
$$

whre $e$ is the base of the natural logarithm and $i$ is the imaginary unit ($i^2=-1$).

As the phase angle $\theta$ increases from $0$ to $+2\pi$, the complex vector $\psi(\theta)$ completes a full counterclockwise revolution. This motion models the execution of the action, denoted $h^+$, along a given path in a chosen direction. Conversely, as $\theta$ decreases from $0$ to $-2\pi$, the vector completes a full rotation in reverse, corresponding the execution of the action in the opposite direction, denoted $h^-$.

In this representation, any periodic physical process can be modeled by a continuously rotating vector using the following identity:

$$  
z = \frac{\theta}{2\pi} = \frac{S}{h} = \frac{t}{\tau} = \frac{x}{\lambda},
$$

where

- $z$ a dimensionless variable representing the number of completed action cycles;
- $\theta$ is the phase in radians, with $2\pi$ corresponding to a full cycle;
- $S$ is the signed action accumulated along a physical trajectory, measured in units of $h$;
- $t$ is the elapsed time measured in units of the action period $\tau$;
- $x$ is the length of an action path measured in units of the step length $\lambda$.

Note that no physical quantity—such as the action $S$, time $t$, or position $x$—can be measured with infinite precision. For example, the measured length of an action path depends on the unit of measurement: as the spatial resolution increases, a physical path reveals additional micro-structure, yielding a scale-dependent value. To remove this ambiguity, physical quantities should be expressed in their natural units. For example, the length of a single action step is defined as

$$
x = 1 \lambda.
$$

Expressing the phase $\theta$ in terms of $S$ and $h$ yields a mathematical description of how an action propagates along a specific path

$$
\psi(S) = e^{i 2\pi \frac{S}{h}},
$$

where $S$ is a signed quantity counting the cumulative action along the path.

The temporal evolution of the system can be expressed as

$$
\psi^{\pm}(t) = e^{\pm i 2\pi \frac{t}{\tau}}.
$$

Here, the $\pm$ sign represents two possible directions as an action propagates along the path. Since time $t$ always increases monotonically, the unfolding of two opposite actions may be encoded as a pair of signed frequencies,

$$
\psi^{\pm}(t) = e^{i2\pi f^{\pm} t} = e^{i \omega^{\pm} t},
\label{eq:time-dependent-wave-function}

$$

where $f^{\pm} = \pm \frac{1}{\tau}$ represent a pair of opposite actions and $\omega^{\pm} = 2\pi f$ represents the corresponding angular frequency.

Space, by contrast, is bidirectional. The value of $x$ specifies a relative position along a path, while the sign of $x$ (or of a displacement $\Delta x$) indicates the direction. The spatial evolution of the system is then written as

$$
\psi^{\pm}(x) = e^{\pm i 2\pi \frac{x}{\lambda}} = e^{\pm i 2\pi k x}, 
\label{eq:space-dependent-wave-function}
$$

where the wavenumber $k= \frac{2\pi}{\lambda}$ represents the spatial density of the periodic action.

Combining ths two equations yields the wave function:

$$
\psi^{\pm}(x,t) = e^{\pm i 2\pi \cdot z} = e^{i2\pi(f^{\pm} t \pm \frac{x}{\lambda})} = e^{i( \omega^{\pm} t \pm k x)}.
$$

This function satisfies Schrödinger's partial differential equation:

$$
i\hbar \frac{\partial}{\partial t}\,\psi(x,t)
=
\hat{H}\,\psi(x,t),
$$

where $\hbar = \frac{h}{2\pi}$ denotes the reduced action constant. The Hamiltonian operator

$$
\hat{H}
=
-\frac{\hbar^2}{2m}\frac{\partial^2}{\partial x^2}
+ V(x)
$$

represents the energy that drives the spacetime evolution of the system.
