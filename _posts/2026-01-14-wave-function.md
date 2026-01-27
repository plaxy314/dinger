---
title: Wave Function
date: 2026-01-14 10:33:00 -0800
categories: [朝花夕拾, Quantum Mechanics Reimagined]
tags: [quantum mechanics, wave function, Schrödinger's equation]
pin: false
math: true
---

The execution of the unit action $h$ along a given path may be represented by a rotating vector that traces the unit circle in the complex plane, using Euler's formula:

$$
\psi(\theta) = e^{i \theta} = \cos\theta + i \sin\theta,
$$

whre $e$ is the base of the natural logarithm and $i$ is the imaginary unit ($i^2=-1$).

As the phase angle $\theta$ increases from $0$ to $+2\pi$, the complex vector $\psi(\theta)$ completes a full counterclockwise revolution. This motion models the execution of the action, denoted $h^+$, along the path in a chosen direction. Conversely, as $\theta$ decreases from $0$ to $-2\pi$, the vector completes a full rotation in reverse, corresponding the execution of the action in the opposite direction, denoted $h^-$.

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

The signed action $S$ accumulated along a path determines the phase of the corresponding action signal. Expressed in units of $h$, this phase takes the form

$$
\psi(S) = e^{i 2\pi \frac{S}{h}}.
$$

> Quantum Mechanics Reimagined (`ant` = `kinesin/step motor` =  `action agent`)
{: .prompt-info }
{% include embed/youtube.html id='WXTKZUhPcDA' %}

The temporal evolution of the system can be expressed as

$$
\psi^{\pm}(t) = e^{\pm i 2\pi \frac{t}{\tau}}.
$$

The $\pm$ superscript indicates that we need a pair of equations to describe the direction of the underlying actions. Because the time $t$ increases monotonically and carries no intrinsic directionality, opposite orientations must be encoded in the sign of the frequency. This is accomplished by introducing a pair of signed frequencies,

$$
\psi^{\pm}(t) = e^{i2\pi f^{\pm} t} = e^{i \omega^{\pm} t},
$$

where $f^{\pm} = \pm \frac{1}{\tau}$ correspond to two opposite directions, and $\omega^{\pm} = 2\pi f$ is the associated angular frequency.

Space, by contrast, is bidirectional. The signs of $x$ (or of a displacement $\Delta x$) naturally represent two opposite directions. The spatial evolution of the system is thus written as

$$
\psi^{\pm}(x) = e^{\pm i 2\pi \frac{x}{\lambda}} = e^{\pm i 2\pi k x},
$$

where the wavenumber $k= \frac{2\pi}{\lambda}$ corresponds to the spatial frequency of the periodic action.

Combining two equations yields the wave function that describes the spacetime evolution of the system:

$$

\begin{align*}

\psi^{\pm}(x,t) &= e^{\pm i 2\pi \cdot z}  \\
&= e^{i2\pi(f^{\pm} t \pm \frac{x}{\lambda})} \\
&= e^{i( \omega^{\pm} t \pm k x)}.
\end{align*}
$$

This complex-valued function satisfies Schrödinger's partial differential equation:

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

{% include embed/youtube.html id='nZhSoC_EbMw' %}
