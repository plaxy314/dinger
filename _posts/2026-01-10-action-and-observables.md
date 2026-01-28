---
title: Action and Observables
date: 2026-01-10 10:33:00 -0800
categories: [朝花夕拾, Quantum Mechanics Reimagined]
tags: [quantum mechanics, spacetime, natural units, action, uncertainty principle, action density, observables]
pin: false
math: true
---

## Natural Units of Time and Length
To describe the dynamics of ant-foraging systems such as 
[2]({{'/posts/self-organizing-intelligence/#fn:puzzle-1' | relative_url}}) and
[3]({{'/posts/self-organizing-intelligence/#fn:puzzle-2' | relative_url}}),
we focus on the fundamental unit of motion: the ant step. Each ant step is characterized by two parameters: its duration and its step length.

Let $\tau$ denote the mean duration of a single ant step, and $\lambda$ the mean step length. For a given system—defined as a particular species of ants foraging in a stable thermal environment—both $\tau$ and $\lambda$ may be treated as constants. They are intrinsic properties of the species and the environment, and therefore serve as natural units of time and length for describing the system’s motion.

The step frequency

$$
f = \frac{1}{\tau}
$$

represents the expected number of actions executed per unit time by a single ant (action agent). The step length $\lambda$ represents the unit dispacement along its path. Together, they define a characteristic speed,

$$
c = \frac{\lambda}{\tau} = \lambda f.
$$

In a stable environment, the speed $c$ is expected to be the same along all ant paths, up to some stochastic fluctuations.

## Action, Energy, and Momentum
Let $h$ denote the action of an ant step. The unit action is defined by

$$
h \equiv \overline{E} \tau \equiv \overline{p} \lambda,
$$

where $\overline{E}$ denotes the mean energy required to execute the action, and $\overline{p}$ denotes the mean momentum associated with each step motion.

Under this definition, the unit energy and momentum may be expressed in terms of the fundamental units $h$, $\tau$, and $\lambda$:

$$
 \overline{E} = \frac{h}{\tau} = h f, \quad  \overline{p} = \frac{h}{ \lambda}.
$$

These relations emphasize that energy and momentum are not independent primitives, but observables derived from the temporal and spatial realization of physical action.

To distinguish the direction of motion, we denote by $h^+$ the action of an ant crossing a fixed reference point in a chosen direction, and by $h^-$ the action crossing the same point in the opposite direction.

A system consisting of two opposing actions doubles its energy expenditure:

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

This distinction highlights a fundamental difference between scalar and vector quantities: observables such as time and energy are scalars: their quantities increase monotonically as the system evolves. The cumulative action executed by a system defines a natural clock for measuring its evolution.

By contrast, vector quantities such as momentum and displacement depend sensitively on the directional organization of individual actions. Coordinated actions reinforce one another, while uncorrelated or oppositely directed actions may partially or completely cancel. The directional nature of vector quantities enables the emergence of coherent, large-scale spatiotemporal patterns, even when the underlying microscopic actions remain largely stochastic.

## Uncertainty Principle

To measure quantities such as time, distance, energy, and momentum in an ant-foraging system, one must observe at least one complete action—that is, an ant crossing a reference point from start to finish. This establishes the limits of what can be meaningfully measured. The minimal resolutions in these quantities are therefore bounded by their corresponding units:

$$
\begin{aligned}
\Delta t \geq \tau, \quad \Delta x &\geq \lambda, \\
\Delta E \geq \overline{E}, \quad \Delta p &\geq \overline{p}.
\end{aligned}
$$

Attempts to probe or describe the system below these limits introduce uncertainty, as no single event can be resolved completely. Time and energy, as well as length and momentum, are not independent observables, and the uncertainty principle is often expressed as:

$$
 \Delta{E} \Delta{t} \geq \overline{E}\tau = h, \quad  \\
 \Delta p \Delta x \geq \overline{p} \lambda =  h,
$$

where $h$ denotes the action of a single ant step.

These relations do not arise from imperfect instruments or experimental error, but from the discrete nature of atomic actions. An ant-foraging system cannot be resolved with infinite precision; instead, it must advance one step at a time. As a result, no physical quantity can be meaningfully defined or measured at scales finer than that of a single action.

## Action Density

We define $\rho(x,t)$ as a signed action density, representing the net rate of action events observable at the point $(x,t)$. The expected number of net actions observable within the unit spacetime region

$$
\left[x-\frac{\lambda}{2},x+\frac{\lambda}{2} \right] \times \left[t-\frac{\tau}{2},t+\frac{\tau}{2} \right]
$$

is given by

$$
P(x, t) = \int_{t-\frac{\tau}{2}}^{t+\frac{\tau}{2}}  \int_{x-\frac{\lambda}{2}}^{x+\frac{\lambda }{2}} \rho(x', t') \, \mathrm{d}x' \, \mathrm{d}t'.
$$

Here, $P(x,t) = +1$ if a forward action $h^+$ is observed, $-1$ if a backward action $h^-$ is observed, and $0$ if no action is observed. The sign of $P(x,t)$ encodes the direction of the action, while its magnitude represents the local probability of observing a single action event within the unit spacetime. Note that two entities—such as ants or other action agents—cannot occupy the same location simultaneously. This exclusion principle ensures that the local probablity never exceeds one.

This definition of $\rho(x,t)$ extends naturally to two- and three-dimensional space, where $x$ represents a position vector. For notational simplicity, we continue to use a single symbol $x$ throughout, with the understanding that it may denote $(x,y)$ in 2D or $(x,y,z)$ in 3D.

For a fixed time $\mathbf{t}$, the spatial integral

$$
P(x, \mathbf{t}) = \int_{x-\frac{\lambda}{2}}^{x+\frac{\lambda }{2}} \rho(x', \mathbf{t}) \, \mathrm{d}x'
$$

represents a snapshot of the system at that instant. Each spatial region of extent $\lambda$ contains a value $P(x,\mathbf{t}) \in [-1,+1]$, where the sign captures the direction of an action occurring at that location and the magnitude represents the progression of the action, with $0$ at initiation and $1$ at completion.

For a fixed reference point $\mathbf{x}$, the temporal integral

$$
P(\mathbf{x}, t) = \int_{t-\frac{\tau}{2}}^{t+\frac{\tau}{2}}  \rho(\mathbf{x}, t') \, \mathrm{d}t'
$$

yields a discrete action signal passing through $\mathbf{x}$. Each unit pulse corresponds to an action event.

Because the actions are signed, integrating the action density $\rho(x,t)$ over a large spacetime region ($\Delta t \gg \tau$ and $\Delta x \gg \lambda$) computes the net effect of all actions within that region:

$$
P(x, t) = \int_{t-\frac{\Delta t}{2}}^{t+\frac{\Delta t}{2}}  \int_{x-\frac{\Delta x}{2}}^{x+\frac{\Delta x}{2}} \rho(x', t') \, \mathrm{d}x' \, \mathrm{d}t'.
$$

To illustrate it, consider two actions observable at different resolutions:

- $h_i$: an individual ant moves across a fixed reference point;

- $h_c$: a group of ants transport a load across the same point.

Each action is characterized by a pair of spatiotemporal parameters. For the individual action $h_i$, these are the mean step duration $\tau_i$ and the step length $\lambda_i$. For the collective action $h_c$, they are the mean transport duration $\tau_c$ and the spatial extent of the load $\lambda_c$. These parameters satisfy the relation: $\tau_c \gg \tau_i$ and $\lambda_c \gg \lambda_i$

At fine resolution ($\Delta t \sim \tau_i$ and $\Delta x \sim \lambda_i$), the system is resolved into discrete step motions of individual ants. At coarser resolution ($\Delta t \sim \tau_c$ and $\Delta x \sim \lambda_c$), uncorrelated individual motions average out, while coordinated actions stand out, giving rise to smooth, collective transport of a large load. 

The microscopic dynamics of the system are captured by the density of the individual action $h_i$, denoted $\rho_i(x,t)$, while the macroscopic dynamics are described by the density of the collective action $h_c$, denoted $\rho_c(x,t)$. These two descriptions are related through spatiotemporal coarse-graining:

$$
\rho_c(x,t) = \frac{1}{\lambda_c \tau_c } \int_{t-\frac{\tau_c}{2}}^{t+\frac{\tau_c}{2}} \int_{x-\frac{\lambda_c}{2}}^{x+\frac{\lambda_c}{2}}  \rho_i(x',t') \, \mathrm{d}x' \, \mathrm{d}t'.
$$

The normalization factor $(\lambda_c \tau_c)^{-1}$ ensures that $\rho(x,t)$ retains the interpretation of a probabilistic action density. This coarse-graining procedure suppresses uncorrelated individual motions while preserving coherent, large-scale patterns that emerge at the system level.

## Observable Signals

The propagation of an action event along a given path produces distinct energy and momentum signatures. These physical signals can be derived from the corresponding action density:

$$
E(x,t) = \frac{h}{\tau} P(x,t),
$$

$$
\vec{p}(x,t) = \frac{h}{\lambda} \hat{\mathbf{v}}_x P(x,t),
$$

where $h$ denotes the unit action, $\tau$ its duration, and $\lambda$ its step length. The unit vector $\hat{\mathbf{v}}_x$ specifies the direction of unit displacement at position $x$.

If the moving entity—whether an ant or a transported load—carries a finite amount of elementary charges $n^{\pm e}$, the action signal manifests as an electric current:

$$
I(x,t) = n^{\pm e} \, P(x,t).
$$

More generally, any physical signal observable along an action path can be derived from the action density:

$$
\mathcal{O}(x,t) = \hat{o} \, P(x,t),
$$

where $\hat{o}$ denotes the unit observable associated with the action $h$. Examples include:
- the amount of heat generated per step,
- the number of oxygen molecules consumed,
- the number of carbon dioxide molecules produced,
- or any other quantifiable effect resulting from the execution of a single action.

Because $\rho(x,t)$ measures as the expected number of net actions observable over the unit spacetime, rather than as the density of action agents, an action path may be interpreted either as the trajectory of a single ant or as the collective path formed by many ants transporting a load. This interpretation allows individual ants to stochastically join or leave a collective path. Coarse-graining the action density thus links microscopic events to macroscopic observables, providing a unified framework for describing system dynamics across spatial and temporal scales.

> Quantum Mechanics Reimagined (`ant` = `kinesin/step motor` = `action agent`)
{: .prompt-info }
{% include embed/youtube.html id='uGQh19-jhXY' %}
