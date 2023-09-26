# Laplace Transform formulae

## Definition
If the function $f(t)$ is defined for $t \geq 0$ and is of exponential order, then the Laplace transform of $f(t)$ is defined as the improper integral  
$F(s) = L\big[f(t)\big] = \int_0^\infty e^{-st} f(t) \ dt$,
where $s$ is a complex number frequency parameter.

___

## Sufficient Conditions for Existence of Laplace Transform
if $f(t)$ defined for $t \geq 0$ is :-
1. Piecewise continuous in the interval $0 \leq t < N$ for every finite $N > 0$.
1. of exponential order $\alpha$ for some $\alpha > 0$ as $t$ &rarr; $\infty$ then the Laplace transform of $f(t)$ exists for $s > \alpha$.

___

## Laplace Transforms of Standard Functions
1. $L\big[1\big] = \frac{1}{s}$

1. $L\big[t^n\big] = \frac{n!}{s^{n+1}}$

1. $L\big[e^{\alpha t}\big] = \frac{1}{s-a}$

1. $L\big[\sin(\alpha t)\big] = \frac{\alpha}{s^2 + \alpha^2}$

1. $L\big[\cos(\alpha t)\big] = \frac{s}{s^2 + \alpha^2}$

1. $L\big[\sinh(\alpha t)\big] = \frac{\alpha}{s^2 - \alpha^2}$

1. $L\big[\cosh(\alpha t)\big] = \frac{s}{s^2 - \alpha^2}$

1. $L\big[erf (\sqrt t)] = \frac{1}{s \sqrt {s + 1}}$ where $erf(\sqrt t) = \frac{2}{\sqrt \pi} \int_0^t e^{-u^2} \ du$

___

## Linearity Property
1. $L\big[f(t) \pm g(t)\big] = F(s) \pm G(s)$

1. $L\big[c f(t)\big] = c F(s)$

___

## Properties of Laplace theorems
### First Shifting Theorem
If $L\big[f(t)\big] = F(s)$ then $L\big[e^{at} f(t)\big] = F(s-a)$ and $L\big[e^{-at} f(t)\big] = F(s+a)$

___

### Second Shifting Theorem
If $L\big[f(t)\big] = F(s)$, & if
$`g(t) =
	\begin{cases}
	f(t - a) &, t > a \\
	0 &, t < a
	\end{cases}`$

then $L\big[g(t)\big] = e^{-as} F(s)$

___

### Multiplication by power of t
If $L\big[f(t)\big] = F(s)$ then $L\big[t^n f(t)\big] = (-1)^n \frac{d^n}{ds^n} F(s)$

___

### Division by t
If $L\big[f(t)\big] = F(s)$ then $L\big[\frac{f(t)}{t}\big] = \int_s^\infty F(s) \ ds$

___

### Laplace Transform of Derivative
If $L\big[f(t)\big] = F(s)$ then $L\big[\frac{d^n(f(t))}{dt^n}\big] = s^n F(s) - s^{n-1} f(0) - s^{n-2} \frac{d}{dt} f(0) - \cdots - \frac{d^{n-1}}{dt^{n-1}} f(0)$

___

### Laplace Transform of Integral &rarr; **Definite Integrals only**
If $L\big[f(t)\big] = F(s)$ then $L\big[\int_0^t f(u) \ du\big] = \frac{1}{s} F(s)$

___

### Change of Scalar Theorem
If $L\big[f(t)\big] = F(s)$ then $L\big[f(at)\big] = \frac{1}{a} F(\frac{s}{a})$

___

## Inverse Laplace Transform
If $L\big[f(t)\big] = F(s)$, then $f(t) = L^{-1}\big[F(s)\big]$

### Inverse Laplace Transform of Standard Functions
1. $L^{-1}\big[\frac{1}{s}\big] = 1$

1. $L^{-1}\big[\frac{1}{s^2}\big] = \frac{t}{1!}$

1. $L^{-1}\big[\frac{1}{s^3}\big] = \frac{t^2}{2!}$

1. $L^{-1}\big[\frac{1}{s^{n+1}}\big] = \frac{t^n}{n!}$ or $L^{-1}\big[\frac{1}{s^{n}}\big] = \frac{t^{n-1}}{(n-1)!}$

1. $L^{-1}\big[\frac{1}{s-\alpha}\big] = e^{\alpha t}$

1. $L^{-1}\big[\frac{1}{s+\alpha}\big] = e^{-\alpha t}$

1. $L^{-1}\big[\frac{1}{(s^2+\alpha^2)}\big] = \frac{\sin(\alpha t)}{\alpha}$

1. $L^{-1}\big[\frac{s}{(s^2+\alpha^2)}\big] = \cos(\alpha t)$

1. $L^{-1}\big[\frac{1}{(s^2-\alpha^2)}\big] = \frac{\sinh(\alpha t)}{\alpha}$

1. $L^{-1}\big[\frac{s}{(s^2-\alpha^2)}\big] = \cosh(\alpha t)$

1. $L^{-1}\big[\frac{1}{(s^2+a^2)^2}\big] = \frac{\sin(\alpha t) - \alpha t \cos(\alpha t)}{2\alpha^3}$

1. $L^{-1}\big[\frac{s}{(s^2+a^2)^2}\big] = \frac{t\sin(\alpha t)}{2\alpha}$

1. $L^{-1}\big[\frac{s^2}{(s^2+a^2)^2}\big] = \frac{\sin(\alpha t) + \alpha t \cos(\alpha t)}{2\alpha}$

1. $L^{-1}\big[\frac{1}{(s^2+a^2)^3}\big] = \cos(\alpha t) - \frac{1}{2}\alpha t\sin(\alpha t)$

1. $L^{-1}\big[\frac{s^2-\alpha^2}{(s^2+\alpha^2)^2}\big]=t\cos(\alpha t)$

1. $L^{-1}\big[\frac{1}{(s^2-\alpha^2)^2}\big] = \frac{at\cosh(\alpha t) - \sinh(\alpha t)}{2\alpha^3}$

1. $L^{-1}\big[\frac{s}{(s^2-\alpha^2)^2}\big] = \frac{t\sinh(\alpha t)}{2\alpha}$

1. $L^{-1}\big[\frac{s^2}{(s^2-\alpha^2)^2}\big] = \frac{\alpha t\cosh(\alpha t) + \sinh(\alpha t)}{2\alpha}$

1. $L^{-1}\big[\frac{s^3}{(s^2-a^2)^2}\big] = \cosh(\alpha t) + \frac{1}{2}\alpha t\sinh(\alpha t)$

1. $L^{-1}\big[\frac{s^2+a^2}{(s^2-a^2)^2}\big] = t\cosh(\alpha t)$

___

### Linearity Property
If $F(s) = L\big[f(t)\big]$ and $G(s) = L\big[g(t)\big]$ then
1. $L^{-1}\big[F(s) \pm G(s)\big] = f(t) \pm g(t)$
2. $L^{-1}\big[cF(s)\big] = cL^{-1}\big[F(s)\big]$ for any constant $c$.

___

## Methods to find Inverse Laplace Transform
### Using above formulae
[Inverse Laplace Transform of Standard Functions](#inverse-laplace-transform-of-standard-functions)

___

### Using Laplace transform properties
[Laplace Transform properties](#properties-of-laplace-theorems)
#### Using [First Shifting Theorem](#first-shifting-theorem)
If $L^{-1}\big[F(s)\big] = f(t)$ then $L^{-1}\big[F(s - a)\big] = e^{at}f(t)$ and $L^{-1}\big[F(s + a)\big] = e^{-at}f(t)$

___

#### Using [Second Shifting Theorem](#second-shifting-theorem)
If $L^{-1}\big[F(s)\big] = f(t)$, then $`L^{-1}\big[e^{-as} F(s)\big] = g(t) = 
	\begin{cases}
	f(t - a) &, t > a \\
	0 &, t < a
	\end{cases}`$

___

#### Using [Multiplication by power of t](#multiplication-by-power-of-t)
$L^{-1}\big[F(s)\big] = \frac{-1}{t}L^{-1}\big[\frac{d(F(s))}{ds}\big]$

Similarly, $L^{-1}\big[\frac{d^n(F(s))}{ds^n}\big] = (-1)^n t^n L^{-1}\big[F(s)\big]$

___

#### Using [Division by t](#division-by-t)
$L^{-1}\big[F(s)\big] = t L^{-1}\big[\int_s^\infty F(s) ds\big]$

___

#### Using [Laplace Transform of Derivative](#laplace-transform-of-derivative)
Let $L^{-1}\big[F(s)\big] = f(t)$ & $f(0) = 0$ then $L^{-1}\big[sF(s)\big] = \frac{d(f(t))}{dt}$

Similarly, $L^{-1}\big[s^nF(s)\big] = \frac{d^n(f(t))}{dt^n} \cdots f(0) = f'(0) = \cdots = f^{n-1}(0) = 0$

___

#### Using [Laplace Transform of Integral](#laplace-transform-of-integral) &rarr; **Definite Integrals only**
Let $L^{-1}\big[F(s)\big] = f(t)$ then $L^{-1}\big[\frac{F(s)}{s}\big] = \int_0^t f(u) \ du$

___

### By partial fractions expansions

## Convolution theorem
### Definition of convolution theorem of two functions
If $L\big[f(t)\big] = F(s)$ and $L\big[g(t)\big] = G(s)$ then $L\big[f(t) * g(t)\big] = F(s)G(s)$

where $f(t) * g(t) = \int_0^t f(u)g(t-u) \ du$ is the convolution of $f(t)$ and $g(t)$

It can proved that $f(t) * g(t) = g(t) * f(t)$ using the substitution the property of definite integrals $\int_a^b f(x) \ dx = \int_a^b f(b + a - x) \ dx$

___

## Applications of Laplace Transform
### Solving Differential Equations
#### To solve initial and boundary value problems involving ordinary differential equations with one dependent variable.
1. Take Laplace transform of both sides of the equation.
1. Solve the resulting algebraic equation for the Laplace transform of the dependent variable.
1. Take the inverse Laplace transform of both sides of the equation.
1. Solve the resulting algebraic equation for the dependent variable.

___

#### To solve system of simultaneous ordinary differential equations.
1. Take Laplace transform of both sides of the equation.
1. Solve the resulting simulaneous equations for the Laplace transform.
1. Take the inverse Laplace transform of both sides of the equation.
1. Solve the resulting simulaneous equations for the dependent variable.

___

## Laplace Transform of Periodic Functions
### Definition of Laplace transform of periodic function
A function $f(t)$ is said to be periodic with period $T$ if $f(t) = f(t + T)$ for all $t$.

**OR**

In general $f(t + nT) = f(t) \ \forall \ t$

The Laplace transform of a periodic function $f(t)$ is given by

$L\big[f(t)\big] = \frac{1}{1-e^{-sT}} \int_0^T e^{-st} f(t) \ dt$

___

## Laplace Transform of Heaviside unit step Function
### Definition of Heaviside unit step Function
Denoted by $H(t)$ or $U(t)$

$`H(t) = 
	\begin{cases}
	0 &, t < 0 \\
	1 &, t > 0
	\end{cases}`$

___

### Displaced Heaviside unit step Function
$`H(t-a) = 
	\begin{cases}
	0 &, t < a \\
	1 &, t > a
	\end{cases}`$

___

### Laplace transform of a function using heaviside unit step function
If a given function is not defined in the interval $(0, \infty)$, but it is defined in, say $(0, a), (0, b), (b, \infty)$
Then, by using [heaviside unit step function](#definition-of-heaviside-unit-step-function), it can be extended to the interval $(0, \infty)$

___

#### Rules
1. If $f(t)$ is defined in $(a, b)$, we write

$g(t) = f(t) H(t-a) - f(t) H(t-b)$,

where $`g(t) = \begin{cases}
		0 &, 0 < t < a \\
		f(t) &, a < t < b \\
		0 &, t > b
		\end{cases}`$

1. If $f(t)$ is defined in $(0, a)$, we write

$g(t) = f(t) H(t) - f(t) H(t-a)$,

where $`g(t) =
		\begin{cases}
		f(t) &, 0 < t < a \\
		0 &, a < t < \infty
		\end{cases}`$

1. If $f(t)$ is defined in $(a, \infty)$, we write

$g(t) = f(t) H(t-a)$,

where $`g(t) = 
		\begin{cases}
		0 &, 0 < t < a \\
		f(t) &, a < t < \infty
		\end{cases}`$

#### Formula for Laplace transform of [Heaviside unit step function](#definition-of-heaviside-unit-step-function)

1. $L\big[H(t)\big] = \frac{1}{s}$

1. $L\big[H(t-a)\big] = \frac{e^{-as}}{s}$

1. $L\big[f(t-a)H(t-a)\big] = e^{-as}L\big[f(t)\big]$

1. $L\big[f(t)H(t)\big] = L\big[f(t)\big]$

1. $L\big[f(t)H(t-a)\big] = e^{-as}\big[L\big[f(t)\big] - L\big[f(t-a)\big]\big]$

## Laplace Transform of Dirac Delta Function
### Definition of Dirac Delta Function
Consider the function F(t) defined by

$`F(t) = 
	\begin{cases}
	0 &, 0 < t < a \\
	\frac{1}{\epsilon} &, a < t < a + \epsilon \\
	0 &, t > a + \epsilon \\
	\end{cases}`$

The limiting value of $F(t)$ as $\epsilon \rightarrow 0$ is called the unit impulse function or Dirac delta function and is denoted by $\delta(t - a)$
i.e. $\delta(t - a) = \lim_{\epsilon \rightarrow 0} F(t)$

Imp note about why $\delta(t - a)$ is called unit impulse function is that, $\int_0^\infty \delta(t - a) \ dt = 1$

___

### Laplace Transform of [Dirac Delta Function](#definition-of-dirac-delta-function)
1. $L\big[\delta(t - a)\big] = e^{-as}$

1. $L\big[\delta(t)\big] = 1$

___

### Relation between [Heaviside unit step function](#definition-of-heaviside-unit-step-function) and [Dirac delta function](#definition-of-dirac-delta-function)
We have
$`F(t) = \begin{cases}
		0 &, 0 < t < a \\
		\frac{1}{\epsilon} &, a < t < a + \epsilon \\
		0 &, t > a + \epsilon \\
		\end{cases}`$

$F(t) = \frac{1}{\epsilon} H(t-a) - \frac{1}{\epsilon} H(t-a-\epsilon)$

$\delta(t-a) = \lim_{\epsilon \rightarrow 0} F(t)$

$ = \lim_{\epsilon \rightarrow 0} \frac{1}{\epsilon} H(t-a) - \lim_{\epsilon \rightarrow 0} \frac{1}{\epsilon} H(t-a-\epsilon)$

$ = \frac{H(t-a) - H(t-a-\epsilon)}{\epsilon}$

$ \therefore \delta(t - a) = H'(t - a) $

___

### Shifting property of [Dirac delta function](#definition-of-dirac-delta-function)
#### Theorem
$\int_0^\infty f(t) \delta(t - a) \ dt = f(a)$, where 
$`\delta(t - a) = \lim_{\epsilon \rightarrow 0} F(t), F(t) = \begin{cases}
		0 &, 0 < t < a \\
		\frac{1}{\epsilon} &, a < t < a + \epsilon \\
		0 &, t > a + \epsilon \\
		\end{cases}`$

#### Corollary of above theorem
$L\big[f(t)\delta(t - a)\big] = e^{-as} f(a)$

If a = 0, then $L\big[f(t)\delta(t)\big] = f(0)$

___

# THE END