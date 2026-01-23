---
title: Action Density
date: 2026-01-15 10:33:00 -0800
categories: [朝花夕拾, Quantum Mechanics Reimagined]
tags: [quantum mechanics, action density]
pin: false
math: true
---

We define $\rho(x,t)$ as a signed action density per unit spacetime, representing the local rate of action events occurring in the vicinity of $(x,t)$. The expected number of net actions within the unit spacetime region

$$
\left[x-\frac{\lambda}{2},x+\frac{\lambda}{2} \right] \times \left[t-\frac{\tau}{2},t+\frac{\tau}{2} \right]
$$

is given by

$$
P(x, t) = \int_{t-\frac{\tau}{2}}^{t+\frac{\tau}{2}}  \int_{x-\frac{\lambda}{2}}^{x+\frac{\lambda }{2}} \rho(x', t') \, \mathrm{d}x' \, \mathrm{d}t'.
$$

Here, $P(x,t) = +1$ if a forward action $h^+$ occurs, $-1$ if a backward action $h^-$ occurs, and $0$ if no action is observed. The sign of $P(x,t)$ encodes the direction of the action, while the magnitude represents the local probability of observing an action event within the unit spacetime. Note that two entities—such as ants or other agents—cannot occupy the same place simultaneously. The exclusion principle ensures the local probablity does not exceed one.

This definition of action density function extends naturally to two- and three-dimensional space, where $x$ represents a position vector. For notational simplicity, we continue to use a single symbol $x$ throughout, with the understanding that it may denote $(x,y)$ in 2D or $(x,y,z)$ in 3D.

For a fixed time $\mathbf{t}$, the spatial integral

$$
P(x, \mathbf{t}) = \int_{x-\frac{\lambda}{2}}^{x+\frac{\lambda }{2}} \rho(x', \mathbf{t}) \, \mathrm{d}x'
$$

takes a snapshot of the system at that instant. Each spatial region of extent $\lambda$ contains a value $P(x,\mathbf{t}) \in [-1,+1]$, where the sign captures the direction of an action occurring at that location and the magnitude represents the progression of the action, with $0$ at initiation and $1$ at completion.

For a fixed reference point $\mathbf{x}$, the temporal integral

$$
P(\mathbf{x}, t) = \int_{t-\frac{\tau}{2}}^{t+\frac{\tau}{2}}  \rho(\mathbf{x}, t') \, \mathrm{d}t'
$$

yields a discrete action signal through $\mathbf{x}$. Each unit pulse corresponds to a single action. The area of a pulse equals one, with its sign encoding the direction of the action.

Because the actions are signed, similar contributions reinforce one another, whereas uncorrelated or opposing contributions may partially or completely cancel. Integrating the action density $\rho(x,t)$ over a region much larger than the unit spacetime ($\Delta t \gg \tau$ and $\Delta x \gg \lambda$) conveniently computes the net effect of all actions within that region:

$$
P(x, t) = \int_{t-\frac{\Delta t}{2}}^{t+\frac{\Delta t}{2}}  \int_{x-\frac{\Delta x}{2}}^{x+\frac{\Delta x}{2}} \rho(x', t') \, \mathrm{d}x' \, \mathrm{d}t'.
$$

To illustrate it, consider two actions observable at different resolutions:

- $h_i$: an individual ant crossing a fixed reference point;

- $h_c$: a group of ants transporting a load across the same point.

Each action is characterized by a pair of spatiotemporal parameters. For the individual action $h_i$, these are the mean step duration $\tau_i$ and the step length $\lambda_i$. For the collective action $h_c$, they are the mean transport duration $\tau_c$ and the spatial extent of the load $\lambda_c$. These parameters satisfy the relation: $\tau_c \gg \tau_i$ and $\lambda_c \gg \lambda_i$

The microscopic dynamics of the system are characterized by the density of the individual action $h_i$, denoted by $\rho_i(x,t)$, while the macroscopic dynamics are described by the density of the collective action $h_c$, denoted by $\rho_c(x,t)$.

At fine resolution, with $\Delta t \sim \tau_i$ and $\Delta x \sim \lambda_i$, the system is resolved into discrete step motions of individual ants. At coarser resolution, with $\Delta t \sim \tau_c$ and $\Delta x \sim \lambda_c$, uncorrelated actions average out, while coordinated actions stand out, giving rise to smooth, collective transport of the load. The two aciton densities are connected through spatiotemporal coarse-graining:

$$
\rho_c(x,t) = \frac{1}{\lambda_c \tau_c } \int_{t-\frac{\tau_c}{2}}^{t+\frac{\tau_c}{2}} \int_{x-\frac{\lambda_c}{2}}^{x+\frac{\lambda_c}{2}}  \rho_i(x',t') \, \mathrm{d}x' \, \mathrm{d}t'.
$$

The normalization factor $(\lambda_c \tau_c)^{-1}$ ensures that $\rho(x,t)$ retains the interpretation of a probability density per unit spacetime. This averaging procedure suppresses uncorrelated microscopic fluctuations while preserving large-scale patterns that emerge at the system level.

The propagation of an action produces distinct energy and momentum signatures. The corresponding energy and momentum signals can be derived from the action density:

$$
E(x,t) = \frac{h}{\tau} P(x,t),
$$

$$
\vec{p}(x,t) = \frac{h}{\lambda} \hat{\mathbf{v}}_x P(x,t),
$$

where $h$ denotes the unit action, $\tau$ its duration, and $\lambda$ its step length. The unit vector $\hat{\mathbf{v}}_x$ specifies the direction of step displacement at position $x$.

If the moving entity—whether an ant or a transported load—carries a finite amount of elementary charges $n^{\pm e}$, the action signal manifests as an electric current:

$$
I(x,t) = n^{\pm e} \, P(x,t).
$$

More generally, any physical quantity observable along an action path can be derived from the action density:

$$
\mathcal{O}(x,t) = \hat{o} \, P(x,t),
$$

where $\hat{o}$ denotes the unit observable associated with the action $h$. Examples include:
- the amount of heat generated per step,
- the number of oxygen molecules consumed,
- the number of carbon dioxide molecules produced,
- or any other quantifiable effect resulting from the execution of a single action.

Because $\rho(x,t)$ is defined as a density of expected action events rather than a density of ants, an action path may be interpreted either as the trajectory of a single ant or as the collective path of a transported load. This definition remains valid even when ants stochastically enter or leave a given path. The probabilistic action density bridges microscopic events and macroscopic observables, providing a consistent description of the system’s dynamics across spatial and temporal scales.
