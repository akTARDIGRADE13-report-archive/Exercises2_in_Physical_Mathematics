---
title: Set 0
---

## Problem 1

### (a)

Let $z$ be defined as follows:

$$
z = \sin \theta = \frac{e^{i\theta} - e^{-i\theta}}{2i}.
$$

Solving the above equation for $\theta$, we obtain:

$$
\begin{aligned}
e^{i\theta} - e^{-i\theta} &= 2i z \\
e^{2i\theta} - 1 &= 2iz e^{i\theta} \\
e^{2i\theta} - 2iz e^{i\theta} - 1 &= 0 \\
e^{i\theta} &= iz \pm \sqrt{1 - z^2} \\
\theta &= -i \log(iz \pm \sqrt{1 - z^2}).
\end{aligned}
$$

To ensure continuity with the real-valued $\sin \theta$, we choose the $+$ branch:

$$
\theta = \arcsin z = -i \log(iz + \sqrt{1 - z^2}).
$$

Choosing the $+$ branch maps the domain $-1 \leq z \leq 1$ to $-\frac{\pi}{2} \leq \theta \leq \frac{\pi}{2}$. This can be verified by the following calculation.

If $-1 \leq z \leq 1$, using $a, \ b \in \mathbb{R}$, we have:

$$
z = \frac{b}{\sqrt{a^2 + b^2}}.
$$

Then, we can find $\theta$ as follows:

$$
\begin{aligned}
\arcsin z &= -i \log\qty(i \frac{b}{\sqrt{a^2 + b^2}} + \sqrt{1 - \frac{b^2}{a^2 + b^2}}) \\
&= -i \qty{\log \abs{ i\frac{b}{\sqrt{a^2 + b^2}} + \sqrt{1 - \frac{b^2}{a^2 + b^2}} } + i \arg \qty(i\frac{b}{\sqrt{a^2 + b^2}} + \sqrt{1 - \frac{b^2}{a^2 + b^2}})} \\
&= -i \qty{\log 1 + i \arctan \frac{b}{a}} \\
&= \arctan \frac{b}{a}.
\end{aligned}
$$

Therefore, $\arcsin z = \arctan \frac{b}{a}$, which is in the range of $-\frac{\pi}{2} \leq \theta \leq \frac{\pi}{2}$.


### (b)

Let $z$ be defined as follows:

$$
z = \tan \theta = \frac{\sin \theta}{\cos \theta} = \frac{e^{i\theta} - e^{-i\theta}}{i(e^{i\theta} + e^{-i\theta})}.
$$

Solving the above equation for $\theta$, we obtain:

$$
\begin{aligned}
e^{i\theta} - e^{-i\theta} &= i z (e^{i\theta} + e^{-i\theta}) \\
e^{2i\theta} - 1 &= iz e^{2i\theta} - iz \\
e^{2i\theta} \qty(1 - iz) &= 1 + iz \\
e^{2i\theta} &= \frac{1 + iz}{1 - iz} \\
\theta &= -\frac{i}{2} \log \frac{1 + iz}{1 - iz} \\
&= \frac{i}{2} \qty{\log (1 - iz) - \log (1 + iz)}.
\end{aligned}
$$

Therefore, 

$$
\theta = \arctan z = \frac{i}{2} \qty{\log (1 - iz) - \log (1 + iz)}.
$$

### (c)

$$
\begin{aligned}
i ^ {\frac{1}{3}} &= e^{i \frac{\frac{\pi}{2}+2k\pi}{3}} \\
&= e^{i \frac{\pi}{6} + \frac{2k\pi}{3}} \quad (k = 0, 1, 2).
\end{aligned}
$$

Therefore,

$$
i ^ {\frac{1}{3}} = \frac{\sqrt{3}}{2} + \frac{1}{2}i, \ -i, \ -\frac{\sqrt{3}}{2} + \frac{1}{2}i.
$$


## Problem 2

$$
e^{in\theta} = \cos n\theta + i \sin n\theta.
$$

On the other hand,

$$
\begin{aligned}
e^{in\theta} &= \qty(e^{i\theta})^n \\
&= \qty(\cos \theta + i \sin \theta)^n \\
&= \sum_{k=0}^{n} \binom{n}{k} \qty(\cos^{n-k} \theta) \qty( i \sin^k \theta) \\
&= \sum_{k=0}^{\floor{n/2}} (-1)^k \binom{n}{2k} \qty(\cos^{n-2k} \theta) \qty( \sin^{2k} \theta) + i\sum_{k=0}^{\floor{(n-1)/2}} (-1)^k \binom{n}{2k+1} \qty(\cos^{n-2k-1} \theta) \qty( \sin^{2k+1} \theta) .
\end{aligned}
$$

Therefore, we get the following:

### (a)

$$
\cos n\theta = \sum_{k=0}^{\floor{n/2}} (-1)^k \binom{n}{2k} \qty(\cos^{n-2k} \theta) \qty( \sin^{2k} \theta),
$$

### (b)

$$
\sin n\theta = \sum_{k=0}^{\floor{(n-1)/2}} (-1)^k \binom{n}{2k+1} \qty(\cos^{n-2k-1} \theta) \qty( \sin^{2k+1} \theta).
$$


## Problem 3

$$
\begin{aligned}
\sin x/2 \sum_{n=0}^{N-1} \cos nx &= \frac{1}{2} \sum_{n=0}^{N-1} \qty{\sin \qty(\frac{2n+1}{2}x) - \sin \qty(\frac{2n-1}{2}x)} \\
&= \frac{1}{2} \qty{\sin \qty(\frac{2N-1}{2}x) - \sin \qty(-\frac{x}{2})} \\
&= \frac{1}{2} \qty{\sin \qty(\frac{2N-1}{2}x) + \sin \qty(\frac{x}{2})} \\
&= \frac{1}{2} \qty{\sin \qty(\frac{N}{2}x + \frac{N-1}{2}x) + \sin \qty(\frac{N}{2}x - \frac{N-1}{2}x)} \\
&= \sin \frac{Nx}{2} \cos \frac{(N-1)x}{2}.
\end{aligned}
$$

Therefore,

$$
\sum_{n=0}^{N-1} \cos nx = \frac{\sin Nx/2 \cos (N-1)x/2}{\sin x/2}.
$$

## Problem 4

Let $I$ be defined as follows:

$$
I = \int_{0}^{\infty} e^{-at} \sin bt \dd{t}.
$$

Then,

$$
\begin{aligned}
I &= \int_{0}^{\infty} e^{-at} \sin bt \dd{t} \\
&= \qty[\frac{-e^{-at}}{a} \sin bt]_{0}^{\infty} - \int_{0}^{\infty} \frac{-e^{-at}}{a} b \cos bt \dd{t} \\
&= \frac{b}{a} \int_{0}^{\infty} e^{-at} \cos bt \dd{t} \\
&= \frac{b}{a} \qty[\frac{e^{-at}}{a} \cos bt]_{0}^{\infty} - \frac{b}{a}\int_{0}^{\infty} \frac{e^{-at}}{a} (-b) \sin bt \dd{t} \\
&= \frac{b}{a^2} - \frac{b^2}{a^2} I .
\end{aligned}
$$

Therefore,

$$
I = \frac{b}{a^2 + b^2} .
$$

## Problem 5

$$
\begin{aligned}
\int_{0}^{\infty} \frac{e^{-s}}{s} (1-e^{-s}) \dd{s} &= \int_{0}^{\infty} \int_{0}^{1} e^{-s(t+1)} \dd{t} \dd{s} \\
&= \int_{0}^{1} \int_{0}^{\infty} e^{-s(t+1)} \dd{s} \dd{t} \\
&= \int_{0}^{1} \frac{1}{t+1} \dd{t} \\
&= \ln 2.
\end{aligned}
$$

The interchange of the order of integration was justified by Tonelli's theorem, as the integrand is non-negative within the integration domain.