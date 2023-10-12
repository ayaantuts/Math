# Fourier Series Formulae

## Definition
Any function can be expressed as a sum of sines and cosines of different frequencies. This is called the Fourier Series of the function.

## Definition of Periodicity
A function $f(x)$ is said to be periodic if there exists a positive real number $T$ such that $f(x+T) = f(x) \forall x$.

In general, $f(x+nT) = f(x) \forall x$.

## Some important results of Integration
1. $`\int_c^{c+2\pi} \cos{mx} \cos{nx} \, dx =
	\begin{cases}
	0 &, m \neq n \\
	2\pi &, m = n = 0 \\
	\pi &, m = n \\
	\end{cases}`$
1. $`\int_c^{c+2\pi} \sin{mx} \sin{nx} \, dx =
	\begin{cases}
	0 &, m \neq n \\
	0 &, m = n = 0 \\
	\pi &, m = n \\
	\end{cases}`$
1. $\int_c^{c+2\pi} \sin{mx} \cos{nx} \, dx = 0\ \forall\ m,n $
1. $`\int_c^{c+2\pi} \cos{mx} = 
	\begin{cases}
	0 &, m > 0 \\
	2\pi &, m = 0 \\
	\end{cases}`$
1. $`\int_c^{c+2\pi} \sin{mx} = 0\ \forall\ m`$

## Euler's Formula to determine the Fourier constants
The Fourier expansion of $f(x)$ expanded in $(c, c + 2\pi)$ is given by
$$f(x) = \frac{a_0}{2} + \sum_{n=1}^{\infty} \left[ a_n \cos{nx} + b_n \sin{nx} \right]$$
where $a_0$, $a_n$ and $b_n$ are called the Fourier constants and are given by
$$a_0 = \frac{1}{\pi} \int_c^{c+2\pi} f(x) \, dx ,\quad a_n = \frac{1}{\pi} \int_c^{c+2\pi} f(x) \cos{nx} \, dx ,\quad b_n = \frac{1}{\pi} \int_c^{c+2\pi} f(x) \sin{nx} \, dx$$

## Dirichlet's Conditions for Fourier Series expansion
Suppose $f(x)$ is defined in $(c, c + 2\pi)$ is periodic with period $2\pi$. The conditions are
1. $f(x)$ is single valued and finite in $(c, c + 2\pi)$
1. $f(x)$ has a finite number of maxima and minima in $(c, c + 2\pi)$
1. $f(x)$ has a finite number of discontinuities in $(c, c + 2\pi)$

then, the Fourier series of $f(x)$ converges to $\frac12\big[f(x^+) + f(x^-)\big]$ for every value of x.

**Note:** If a function has $\infty$ discontinuities and thus, does not possess a Fourier Series expansion. Thus, $\tan{x}$ does not have a Fourier Series expansion.

### If c = 0
$f(x)$ is defined in $(0, 2\pi)$ (also known as **Full range series**)

Then, the Fourier series is given by,
$$f(x) = \frac{a_0}{2} + \sum_{n=1}^{\infty} \left[ a_n \cos{nx} + b_n \sin{nx} \right]$$
where
$$a_0 = \quad \frac{1}{\pi} \int_0^{2\pi} f(x) \, dx, \quad a_n = \frac{1}{\pi} \int_0^{2\pi} f(x) \cos{nx} \, dx, \quad b_n = \frac{1}{\pi} \int_0^{2\pi} f(x) \sin{nx} \, dx$$