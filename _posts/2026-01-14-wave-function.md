---
title: Wave Function
date: 2026-01-14 10:33:00 -0800
categories: [朝花夕拾, Quantum Mechanics Reimagined]
tags: [quantum mechanics, wave function, Schrödinger's equation]
pin: false
math: true
---

The execution of a periodic action $h$ can be modeled by a point rotating around the unit circle in the complex plane, represented by the complex function:

$$
\psi(\theta) = e^{i \theta} = \cos\theta + i \sin\theta,
$$

where $e$ is the base of the natural logarithm and $i$ is the imaginary unit ($i^2=-1$).

As the phase angle $\theta$ increases from $0$ to $+2\pi$, the complex vector $\psi(\theta)$ completes a full counterclockwise revolution. This motion represents the execution of the action $h^+$. Conversely, as $\theta$ decreases from $0$ to $-2\pi$, the vector completes a full rotation in reverse, corresponding the execution of the counter-action $h^-$.

Any periodic physical process can therefore be mapped to motion in the complex plane using the identity,

$$  
z = \frac{\theta}{2\pi} = \frac{S}{h} = \frac{t}{\tau} = \frac{x}{\lambda},
$$

where

- $z$ a dimensionless variable representing the number of completed action cycles;
- $\theta$ is the phase in radians, with $2\pi$ corresponding to a full cycle;
- $S$ is the signed action accumulated along a physical trajectory, measured in units of $h$;
- $t$ is the elapsed time measured in units of the action period $\tau$;
- $x$ is the length of an action path measured in units of the step length $\lambda$.

The physical quantity $S$ represents the action accumulated along an action path. Expressing the phase $\theta$ in terms of $S$ and $h$ yields

$$
\psi(S) = e^{i 2\pi \frac{S}{h}}.
$$

This equation plays an essential role in Feynman's path integral formulation of quantum mechanics.

> Quantum Mechanics Reimagined (`ant` = `kinesin/step motor` =  `action agent`)
{: .prompt-info }
{% include embed/youtube.html id='WXTKZUhPcDA' %}

The temporal evolution of the system can be expressed as

$$
\psi(t) = e^{\pm i 2\pi \frac{t}{\tau}},
$$

where the $\pm$ sign in the exponent indicates that we need a pair of equations to describe the evolution of two opposite actions. Because the time $t$ increases monotonically in one direction, two opposite actions can be modeled using a pair of signed frequencies,

$$
\psi(t) = e^{i2\pi f_{\pm} t} = e^{i \omega_{\pm} t},
$$

where $f_{\pm} = \pm \frac{1}{\tau}$ correspond to two opposite directions, and $\omega_{\pm} = 2\pi f_{\pm}$ are the associated angular frequencies.

Space, by contrast, is bidirectional. The signs of $x$ (or of a displacement $\Delta x$) naturally represent two opposite directions. The spatial evolution of the system is thus written as

$$
\psi(x) = e^{\pm i 2\pi \frac{x}{\lambda}} = e^{\pm i 2\pi k x},
$$

where the wavenumber $k= \frac{2\pi}{\lambda}$ corresponds to the spatial frequency of the periodic action.

Combining two equations yields the wave function that describes the evolution of the system over spacetime:

$$

\begin{align*}

\psi(x,t) &= e^{i 2\pi (\frac{t}{\tau} \pm \frac{x}{\lambda})}  \\
 &= e^{i2\pi(f t \pm \frac{x}{\lambda})} \\
 &= e^{i( \omega t \pm k x)}.
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

{% include embed/youtube.html id='I7c5DNziNeU' %}
