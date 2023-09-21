# Laplace Transform formulae

## Definition
If the function $f(t)$ is defined for $t \geq 0$ and is of exponential order, then the Laplace transform of $f(t)$ is defined as the improper integral
$F(s) = L\big[f(t)\big] = \int_0^\infty e^{-st} f(t) \, dt$
where $s$ is a complex number frequency parameter.

## Properties
### Linearity
1. $L\big[f(t) \pm g(t)\big] = F(s) \pm G(s)$

1. $L\big[c f(t)\big] = c F(s)$

## Laplace Transforms of Common Functions
1. $L\big[1\big] = \frac{1}{s}$

1. $L\big[t^n\big] = \frac{n!}{s^{n+1}}$

1. $L\big[e^{\alpha t}\big] = \frac{1}{s-a}$

1. $L\big[\sin(\alpha t)\big] = \frac{\alpha}{s^2 + \alpha^2}$

1. $L\big[\cos(\alpha t)\big] = \frac{s}{s^2 + \alpha^2}$

1. $L\big[\sinh(\alpha t)\big] = \frac{\alpha}{s^2 - \alpha^2}$

1. $L\big[\cosh(\alpha t)\big] = \frac{s}{s^2 - \alpha^2}$