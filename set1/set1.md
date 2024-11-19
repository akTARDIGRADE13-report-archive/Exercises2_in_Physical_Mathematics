---
title: Set 1
---

## Problem 1

### (a)

$$
\begin{aligned}
e^{-2x} &= 1 - 2x + \frac{4x^2}{2!} - \frac{8x^3}{3!} + \frac{16x^4}{4!} - \frac{32x^5}{5!} + \cdots \\
&= \sum_{n=0}^{\infty} (-2)^n \frac{x^n}{n!} .
\end{aligned}
$$

### (b)

$$
(1+x)^3 = 1 + 3x + 3x^2 + x^3 = \sum_{n=0}^{3} \binom{3}{n} x^n .
$$

### (c)

If $0 < r < 1$ ,

$$
\sum_{n=0}^{\infty} r^n = \frac{1}{1-r} .
$$

Therefore,

$$
\frac{1}{1-x} = \sum_{n=0}^{\infty} x^n .
$$

## Problem 2

### (a)

$$
\begin{aligned}
e^{-2} &= e^{-2} - 2e^{-2}(x-1) + \frac{4}{2!} e^{-2}(x-1)^2 - \frac{8}{3!} e^{-2}(x-1)^3 + \cdots \\
&= e^{-2} \sum_{n=0}^{\infty} (-2)^n \frac{(x-1)^n}{n!} .
\end{aligned}
$$

### (b)

$$
\begin{aligned}
(1+x)^3 &= {1+(t+1)}^3 \quad \text{where } t = x-1 \\
&= t^3 + 6t^2 + 12t + 8 \\
&= (x-1)^3 + 6(x-1)^2 + 12(x-1) + 8 .
\end{aligned}
$$

### (c)

$$
\begin{aligned}
\frac{1}{1-2x} &= \frac{1}{1-2(t+1)} \quad \ \text{where } t = x-1 \\
&= \frac{1}{1-2t-2} \\
&= -\frac{1}{1+2t} \\
&= -\sum_{n=0}^{\infty} (-2t)^n \\
&= \sum_{n=0}^{\infty} (-1)^{n+1} 2^n (x-1)^n .
\end{aligned}
$$

## Problem 3

### (a)

$$
(3)_2 = 3 \times 4 = 12 .
$$

### (b)

$$
\qty(\frac{1}{2})_3 = \frac{1}{2} \times \frac{3}{2} \times \frac{5}{2} = \frac{15}{8} .
$$

### (c)

$$
(-3)_2 = (-3) \times (-2) = 6 .
$$

### (d)

$$
(-3)_4 = (-3) \times (-2) \times (-1) \times 0 = 0 .
$$

## Problem 4

### (a)

$$
(1-x)^{1/2} = \sum_{n=0}^{\infty} \frac{\qty(-\frac{1}{2})_n}{n!} x^n .
$$

### (b)

$$
(2+3x)^{-2} = \qty(\frac{1}{2})^{-2} \qty(1+\frac{3}{2}x)^{-2} = 4 \sum_{n=0}^{\infty} \frac{\qty(2)_n}{n!} \qty(\frac{3}{2}x)^n .
$$

## Problem 5

$$
\begin{aligned}
E = \frac{mc^2}{\sqrt{1-\frac{v^2}{c^2}}} &= mc^2 (1-x)^{-1/2} \quad \text{where } x = \frac{v^2}{c^2} \\
&= mc^2 \sum_{n=0}^{\infty} \frac{\qty(\frac{1}{2})_n}{n!} x^n \\
&= mc^2 \sum_{n=0}^{\infty} \frac{\qty(\frac{1}{2})_n}{n!} \qty(\frac{v^2}{c^2})^n .
\end{aligned}
$$

## Problem 6

### (a)

$$
\begin{aligned}
(x)_{2n} &= x(x+1)(x+2) \cdots (x+2n-1) \\
&= x(x+2)(x+4) \cdots (x+2n-2) (x+1) (x+3) \cdots (x+2n-1) \\
&= 2^{2n} \frac{x}{2} \qty(\frac{x}{2}+1) \qty(\frac{x}{2}+2) \cdots \qty(\frac{x}{2}+n-1) \frac{x+1}{2} \qty(\frac{x+1}{2}+1) \cdots \qty(\frac{x+1}{2}+n-1) \\
&= 2^{2n} \qty(\frac{x}{2})_n \qty(\frac{x+1}{2})_n .
\end{aligned}
$$

### (b)

$$
\begin{aligned}
\cos x &= \sum_{n=0}^{\infty} \frac{(-1)^n}{(2n)!} (x^2)^n \\
&= \sum_{n=0}^{\infty} \frac{1}{\qty(\frac{1}{2})_n (1)_n} \qty(\frac{-x^2}{4})^n \quad \because \ \text{Problem 6 (a)} \\
&= \sum_{n=0}^{\infty} \frac{1}{\qty(\frac{1}{2})_n n!} \qty(\frac{-x^2}{4})^n .
\end{aligned}
$$

## Problem 7

$$
\begin{aligned}
\cos (x+y) + i \sin (x+y) = e^{i(x+y)} &= e^{ix} e^{iy} \\
&= (\cos x + i \sin x) (\cos y + i \sin y) \\
&= \cos x \cos y - \sin x \sin y + i (\cos x \sin y + \sin x \cos y) .
\end{aligned}
$$

Therefore,

$$
\begin{aligned}
\cos (x+y) &= \cos x \cos y - \sin x \sin y , \\
\sin (x+y) &= \cos x \sin y + \sin x \cos y .
\end{aligned}
$$

## Problem 8

First, we compute the following integral:

$$
\int_0^x \frac{1}{\sqrt{1-t^2}} dt.
$$

Using the substitution $t = \sin u$, we have $dt = \cos u du$ and the limits of integration transform as follows: $t = 0 \to u = 0$,and $t = x \to u = \arcsin x$. Substituting, we get:

$$
\int_0^x \frac{1}{\sqrt{1-t^2}} dt = \int_0^{\arcsin x} \frac{1}{\cos u} \cos u du = \int_0^{\arcsin x} du = \arcsin x.
$$

Next, we expand $\arcsin x$ as a power series:

$$
\begin{aligned}
\arcsin x &= \int_0^x \frac{1}{\sqrt{1-t^2}} dt \\
&= \int_0^x \sum_{n=0}^{\infty} \frac{\qty(\frac{1}{2})_n}{n!} (t^2)^n dt \\
&= \sum_{n=0}^{\infty} \int_0^x \frac{\qty(\frac{1}{2})_n}{n!} t^{2n} dt \\
&= \sum_{n=0}^{\infty} \frac{1}{2n+1} \frac{\qty(\frac{1}{2})_n}{n!} x^{2n+1} \\
&= x \sum_{n=0}^{\infty} \frac{(1/2)_n}{(3/2)_n} \frac{(1/2)_n}{n!} x^{n}.
\end{aligned}
$$

## Problem 9

### (a)

$$
\begin{aligned}
\qty(x \dv{x} - a) y(x) &= 0 \\
x \dv{x} y(x) &= a y(x) \\
\int \frac{1}{y} \dd{y} &= a \int \frac{1}{x} \dd{x} \\
\ln y &= a \ln x + C' \quad \text{where } C' \text{ is const} \\
y &= C x^a \quad \text{where } C = e^{C'} .
\end{aligned}
$$

### (b)

$$
x \dv{x} y(x) - a y(x) = c x^b.
$$

The homogeneous solution is given by $y_h = C x^a$. For the particular solution, assume $y_p = K x^b$. Substituting $y_p$ into the differential equation yields:

$$
\begin{aligned}
b K x^b - a K x^b &= c x^b \\
b K - a K &= c \\
K &= \frac{c}{b-a} .
\end{aligned}
$$

Thus, the general solution is:
$$
y = C x^a + \frac{c}{b-a} x^b.
$$

### (c)

Applying $(\theta - a)$ to $x^b$, we get:

$$
(\theta - a) x^b = (b - a) x^b.
$$

If $b - a \neq 0$, the operator $(\theta - a)$ is invertible when acting on $x^b$. Its inverse operates as:

$$
\frac{1}{\theta - a} x^b = \frac{1}{b - a} x^b.
$$

Therefore, we can express the particular solution $y_p(x)$ formally as:

$$
y_p(x) = c \frac{1}{\theta - a} x^b = \frac{c}{b - a} x^b.
$$

This result aligns with the particular solution found in Problem 9 (b). Hence, the special solution of the differential equation is:

$$
y(x) = c \frac{1}{\theta - a} x^b.
$$

### (d)

First, consider a particular solution of the form:

$$
y_p(x) = Cx^{a + \varepsilon} \quad \text{where } C \text{ is const}.
$$

Applying $(\theta - a)$ to $y_p(x)$:

$$
\begin{aligned}
(\theta - a) y_p(x) &= \qty( x \frac{d}{dx} - a ) Cx^{a + \varepsilon} \\
&= \qty( x \frac{d}{dx} Cx^{a + \varepsilon} - a Cx^{a + \varepsilon} ) \\
&= \qty{ (a + \varepsilon) Cx^{a + \varepsilon} - a Cx^{a + \varepsilon} } \\
&= \qty{ (a + \varepsilon - a) Cx^{a + \varepsilon} } \\
&= \varepsilon Cx^{a + \varepsilon}.
\end{aligned}
$$

Thus, the particular solution is:

$$
y_p(x) = Cx^{a + \varepsilon}.
$$

In the limit $\varepsilon \to 0$, the particular solution becomes:

$$
\lim_{\varepsilon \to 0} y_p(x) = Cx^a.
$$

Because of Problem 9 (a), the homogeneous solution is given by $y_h = C x^a$. 

Therefore, in the limit $\varepsilon \to 0$, the specialsolution of the differential equation

$$
(\theta - a) y(x) = \varepsilon x^{a + \varepsilon}
$$

reduces to the solution of the homogeneous equation.

## Problem 10

The left-hand side of the differential equation can be written as:

$$
\text{LHS} = \theta f(x) = x \dv{x} f(x).
$$

The right-hand side of the differential equation can be written as:

$$
\text{RHS} = x (\theta + a) f(x) = x^2 \dv{x} f(x) + a x f(x).
$$

Therefore, the differential equation can be written as:

$$
x \dv{x} f(x) - x^2 \dv{x} f(x) - a x f(x) = 0.
$$

If $x \neq 0$, 

$$
\begin{aligned}
(1 - x) \dv{x} f(x) - a f(x) &= 0 \\
\frac{1}{f(x)} \dv{x} f(x) - a f(x) &= 0 \\
\int \frac{1}{f(x)} \dd{f(x)} &= a \int \frac{1}{1-x} \dd{x} \\
\ln f(x) &= a \ln (1-x) + C' \quad \text{where } C' \text{ is const} \\
f(x) &= C (1-x)^{-a} \quad \text{where } C = e^{C'} \\
&= C \sum_{n=0}^{\infty} \frac{\qty(a)_n}{n!} x^n. 
\end{aligned}
$$

## Problem 11

The homogeneous solution is

$$
f_h = C (1-x)^{-a} = C \sum_{n=0}^{\infty} \frac{\qty(a)_n}{n!} x^n \quad \because \ \text{Problem 10} .
$$

For the general solution, assume 

$$
f = C(x) (1-x)^{-a} = C(x)\sum_{n=0}^{\infty} \frac{\qty(a)_n}{n!} x^n
$$

Substituting it into the differential equation yields:

$$
\begin{aligned}
\theta f - x(\theta + a) f &= c x^b \\
(1-x) \theta f - a x f &= c x^b \\
(1-x) x \qty[C'(x)(1-x)^{-a} + a C(x)(1-x)^{-a-1}] - a x C(x)(1-x)^{-a} &= c x^b \\
x (1-x)^{-a+1} C'(x) &= c x^b
\end{aligned}
$$

where $C'(x) = \dv{C(x)}{x}$. Therefore,

$$
\begin{aligned}
C(x) &= c \int x^{b-1} (1-x)^{a-1} \dd{x} \\
&= c \int x^{b-1} \sum_{n=0}^{\infty} \frac{\qty(1-a)_n}{n!} x^n \dd{x} \\
&= c \sum_{n=0}^{\infty} \frac{\qty(1-a)_n}{n!} \int x^{b+n-1} \dd{x} \\
&= c \sum_{n=0}^{\infty} \frac{\qty(1-a)_n}{n!} \frac{x^{b+n}}{b+n} + C'' \quad \text{where } C'' \text{ is const} \\
f &= c \qty(\sum_{n=0}^{\infty} \frac{\qty(a)_n}{n!} x^n) \qty(\sum_{n=0}^{\infty} \frac{\qty(1-a)_n}{n!} \frac{x^{b+n}}{b+n} + C'') 
\end{aligned}
$$

