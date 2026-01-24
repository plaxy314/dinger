---
title: Action and Observables
date: 2026-01-10 10:33:00 -0800
categories: [朝花夕拾, Quantum Mechanics Reimagined]
tags: [quantum mechanics, action, time, energy, length, momentum]
pin: false
math: true
---

## Natural Units of Time and Length
To model the dynamics of ant-foraging systems such as 
[2](/posts/self-organizing-intelligence/#fn:puzzle-1) and
[3](/posts/self-organizing-intelligence/#fn:puzzle-2),
we focus on the fundamental unit of motion: the ant step. Each ant step is characterized by two parameters: its duration and its step length.

Let $\tau$ denote the mean duration of a single ant step, and $\lambda$ the mean step length. For a given system—defined as a particular species of ants foraging in a stable thermal environment—both $\tau$ and $\lambda$ may be treated as constants. They are intrinsic properties of the species and the environment, and therefore serve as natural units of time and length for describing the system’s motion.

The step frequency

$$
f = \frac{1}{\tau}
$$

represents the expected number of actions performed per unit time by an ant. The step length $\lambda$ represents the step dispacement along its path. Together, these quantities define a characteristic speed for this step motion,

$$
c = \frac{\lambda}{\tau} = \lambda f.
$$

In a homogeneous environment, the speed $c$ is expected to be the same along all ant paths, up to stochastic fluctuations.

## Action, Energy, and Momentum
Let $h$ denote the action of a single ant step. This unit action is physically defined as

$$
h \equiv \overline{E} \tau \equiv \overline{p} \lambda,
$$

where $\overline{E}$ denotes the mean energy required to execute the action, and $\overline{p}$ denotes the mean momentum associated with the step motion.

Under this definition, the unit energy and momentum associated with an ant step can be expressed in terms of the fundamental units $h$, $\tau$, and $\lambda$:

$$
 \overline{E} = \frac{h}{\tau} = h f, \quad  \overline{p} = \frac{h}{ \lambda}.
$$

These relations emphasize that energy and momentum are not independent primitives, but observables derived from the temporal and spatial realization of a physical action.

## Scalar vs Vector Observables

To distinguish the direction of motion, we denote by $h^+$ the action of an ant crossing a fixed reference point in a chosen direction, and by $h^-$ the action crossing the same point in the opposite direction.

A system containing a pair of opposing actions doubles its energy expenditure:

$$
\begin{aligned}
 \overline{E}_{\pm} &= \overline{E}_{+} + \overline{E}_{-} \\
  &= \frac{h^+}{\tau^+} + \frac{h^-}{ \tau^-} \\
  &= 2\frac{h}{\tau} \gt 0,
\end{aligned}
$$

but produces no net change in its center of mass,

$$
\begin{aligned}
 \vec{p}_{\pm} &= \vec{p}_{+} + \vec{p}_{-} \\
 &= (\hat{\mathbf{v}}_{+} + \hat{\mathbf{v}}_{-}) \frac{h}{\lambda} \\
 &= (\hat{\mathbf{v}}_{+} - \hat{\mathbf{v}}_{+}) \frac{h}{\lambda} = 0,
\end{aligned}
$$

where 
$$
\hat{\mathbf{v}}_{+} \; \text{and} \; \hat{\mathbf{v}}_{-} = - \hat{\mathbf{v}}_{+}
$$
are unit vectors pointing in opposite directions.

This distinction highlights a fundamental difference between scalar and vector observables: Quantities such as time and energy are scalars: their quantities increase monotonically as the system evolves. The cumulative action executed by the system therefore serves as a natural clock for measuring its evolution.

By contrast, vector quantities such as momentum and displacement depend sensitively on the directional organization of individual motions. Coordinated actions reinforce one another, while uncorrelated or oppositely directed actions may partially or completely cancel. The directional nature of vector quantities enables the emergence of coherent, large-scale spatiotemporal patterns, even when the underlying microscopic motions remain largely stochastic.

{% include embed/youtube.html id='kAvtsl4KVYo' %}
