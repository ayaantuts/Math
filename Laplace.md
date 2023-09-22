# Laplace Transform formulae

## Definition
If the function $f(t)$ is defined for $t \geq 0$ and is of exponential order, then the Laplace transform of $f(t)$ is defined as the improper integral  
$F(s) = L\big[f(t)\big] = \int_0^\infty e^{-st} f(t) \, dt$,
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

1. $L\big[erf (\sqrt t)] = \frac{1}{s \sqrt {s + 1}}$ where $erf(\sqrt t) = \frac{2}{\sqrt \pi} \int_0^t e^{-u^2} \, du$
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
If $L\big[f(t)\big] = F(s)$ then $L\big[\frac{f(t)}{t}\big] = \int_s^\infty F(s) \, ds$
___
### Laplace Transform of Derivative
If $L\big[f(t)\big] = F(s)$ then $L\big[\frac{d^n(f(t))}{dt^n}\big] = s^n F(s) - s^{n-1} f(0) - s^{n-2} \frac{d}{dt} f(0) - \cdots - \frac{d^{n-1}}{dt^{n-1}} f(0)$
___
### Laplace Transform of Integral &rarr; **Definite Integrals only**
If $L\big[f(t)\big] = F(s)$ then $L\big[\int_0^t f(u) \, du\big] = \frac{1}{s} F(s)$
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
### Using First Shifting Theorem
If $F(s) = L^{-1}\big[f(t)\big]$ then $L^{-1}\big[F(s - a)\big] = e^{at}f(t)$ and $L^{-1}\big[F(s + a)\big] = e^{-at}f(t)$
___
### Using Second Shifting Theorem
If $F(s) = L^{-1}\big[f(t)\big]$, then $`L^{-1}\big[e^{-as} F(s)\big] = g(t) = 
	\begin{cases}
	f(t - a) &, t > a \\
	0 &, t < a
	\end{cases}`$