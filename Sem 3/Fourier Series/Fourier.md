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
$$a_0 = \frac{1}{\pi} \int_c^{c+2\pi} f(x) \ dx ,\quad a_n = \frac{1}{\pi} \int_c^{c+2\pi} f(x) \cos{nx} \ dx ,\quad b_n = \frac{1}{\pi} \int_c^{c+2\pi} f(x) \sin{nx} \ dx$$

## Dirichlet's Conditions for Fourier Series expansion
Suppose $f(x)$ is defined in $(c, c + 2\pi)$ is periodic with period $2\pi$. The conditions are
1. $f(x)$ is single valued and finite in $(c, c + 2\pi)$
1. $f(x)$ has a finite number of maxima and minima in $(c, c + 2\pi)$
1. $f(x)$ has a finite number of discontinuities in $(c, c + 2\pi)$

then, the Fourier series of $f(x)$ converges to $\frac12\big[f(x^+) + f(x^-)\big]$ for every value of x.

**Note:** If a function has $\infty$ discontinuities does not possess a Fourier Series expansion. Thus, $\tan{x}$ does not have a Fourier Series expansion.

## Full range series (period = 2&pi;)
### If c = 0
$f(x)$ is defined in $(0, 2\pi)$

Then, the Fourier series is given by,
$$f(x) = \frac{a_0}{2} + \sum_{n=1}^{\infty} \left[ a_n \cos{nx} + b_n \sin{nx} \right]$$
where
$$a_0 = \quad \frac{1}{\pi} \int_0^{2\pi} f(x) \ dx, \quad a_n = \frac{1}{\pi} \int_0^{2\pi} f(x) \cos{nx} \ dx, \quad b_n = \frac{1}{\pi} \int_0^{2\pi} f(x) \sin{nx} \ dx$$

___

### If c = -&pi;
$f(x)$ is defined in $(-\pi, \pi)$

Then, the Fourier series is given by,
$$f(x) = \frac{a_0}{2} + \sum_{n=1}^{\infty} \left[ a_n \cos{nx} + b_n \sin{nx} \right]$$
where
$$a_0 = \quad \frac{1}{\pi} \int_{-\pi}^{\pi} f(x) \ dx, \quad a_n = \frac{1}{\pi} \int_{-\pi}^{\pi} f(x) \cos{nx} \ dx, \quad b_n = \frac{1}{\pi} \int_{-\pi}^{\pi} f(x) \sin{nx} \ dx$$

___

### If f(x) is defined in (0, 2L)
Then, the Fourier series is given by,
$$f(x) = \frac{a_0}{2} + \sum_{n=1}^{\infty} \left[ a_n \cos{\left(\frac{n\pi x}{L}\right)} + b_n \sin{\left(\frac{n\pi x}{L}\right)} \right]$$
where
$$a_0 = \quad \frac{1}{L} \int_0^{2L} f(x) \ dx, \quad a_n = \frac{1}{L} \int_0^{2L} f(x) \cos{\left(\frac{n\pi x}{L}\right)} \ dx, \quad b_n = \frac{1}{L} \int_0^{2L} f(x) \sin{\left(\frac{n\pi x}{L}\right)} \ dx$$

___

### If f(x) is defined in (-L, L)
Then, the Fourier series is given by,
$$f(x) = \frac{a_0}{2} + \sum_{n=1}^{\infty} \left[ a_n \cos{\left(\frac{n\pi x}{L}\right)} + b_n \sin{\left(\frac{n\pi x}{L}\right)} \right]$$
where
$$a_0 = \quad \frac{1}{L} \int_{-L}^{L} f(x) \ dx, \quad a_n = \frac{1}{L} \int_{-L}^{L} f(x) \cos{\left(\frac{n\pi x}{L}\right)} \ dx, \quad b_n = \frac{1}{L} \int_{-L}^{L} f(x) \sin{\left(\frac{n\pi x}{L}\right)} \ dx$$

___

## Even and odd functions
### Even function (symmetric about y-axis)
A function $f(x)$ is said to be even if $f(-x) = f(x) \forall x$.

### Odd function (symmetric about origin)
A function $f(x)$ is said to be odd if $f(-x) = -f(x) \forall x$.

### Even and odd functions in Fourier Series
1. If $f(x)$ in $(-\pi, \pi)$ and even function
	$$a_0 = \frac{2}{\pi} \int_0^{\pi} f(x) \ dx, \quad a_n = \frac{2}{\pi} \int_0^{\pi} f(x) \cos{nx} \ dx, \quad b_n = 0$$
1. If $f(x)$ in $(-\pi, \pi)$ and odd function
	$$a_0 = 0, \quad a_n = 0, \quad b_n = \frac{2}{\pi} \int_0^{\pi} f(x) \sin{nx} \ dx$$
1. If $f(x)$ in $(-L, L)$ and even function
	$$a_0 = \frac{2}{L} \int_0^{L} f(x) \ dx, \quad a_n = \frac{2}{L} \int_0^{L} f(x) \cos{\left(\frac{n\pi x}{L}\right)} \ dx, \quad b_n = 0$$
1. If $f(x)$ in $(-L, L)$ and odd function
	$$a_0 = 0, \quad a_n = 0, \quad b_n = \frac{2}{L} \int_0^{L} f(x) \sin{\left(\frac{n\pi x}{L}\right)} \ dx$$

## Half range series (period = &pi;)
The function $f(x)$ is defined in $(0, \pi)$ and is extended to $(-\pi, 0)$ as an even or odd function.

### Even extension (Half range cosine series)
1. Let $f(x)$ be defined in $(0, \pi)$

$$F(x) = 
	\begin{cases}
	f(x) &, 0 < x < \pi \\
	f(-x) &, -\pi < x < 0 \\
	\end{cases}$$

Then, the Fourier series is given by,
$$F(x) = \frac{a_0}{2} + \sum_{n=1}^{\infty} \left[ a_n \cos{nx} \right]$$
where
$$a_0 = \quad \frac{2}{\pi} \int_0^{\pi} f(x) \ dx, \quad a_n = \frac{2}{\pi} \int_0^{\pi} f(x) \cos{nx} \ dx$$

1. Let $f(x)$ be defined in $(0, L)$

$$F(x) = 
	\begin{cases}
	f(x) &, 0 < x < L \\
	f(-x) &, -L < x < 0 \\
	\end{cases}$$

Then, the Fourier series is given by,
$$F(x) = \frac{a_0}{2} + \sum_{n=1}^{\infty} \left[ a_n \cos{\left(\frac{n\pi x}{L}\right)} \right]$$
where
$$a_0 = \quad \frac{2}{L} \int_0^{L} f(x) \ dx, \quad a_n = \frac{2}{L} \int_0^{L} f(x) \cos{\left(\frac{n\pi x}{L}\right)} \ dx$$

### Odd extension (Half range sine series)
1. Let $f(x)$ be defined in $(0, \pi)$

$$F(x) = 
	\begin{cases}
	f(x) &, 0 < x < \pi \\
	-f(-x) &, -\pi < x < 0 \\
	\end{cases}$$

Then, the Fourier series is given by,
$$F(x) = \sum_{n=1}^{\infty} \left[ b_n \sin{nx} \right]$$
where
$$b_n = \frac{2}{\pi} \int_0^{\pi} f(x) \sin{nx} \ dx$$

1. Let $f(x)$ be defined in $(0, L)$

$$F(x) = 
	\begin{cases}
	f(x) &, 0 < x < L \\
	-f(-x) &, -L < x < 0 \\
	\end{cases}$$

Then, the Fourier series is given by,
$$F(x) = \sum_{n=1}^{\infty} \left[ b_n \sin{\left(\frac{n\pi x}{L}\right)} \right]$$
where
$$b_n = \frac{2}{L} \int_0^{L} f(x) \sin{\left(\frac{n\pi x}{L}\right)} \ dx$$

## Parseval's Identity
### For interval (-L, L)
If the Fourier series of $f(x)$ is defined in $(-L, L)$ coverges uniformly to $f(x)$, then
$$\frac{1}{L}\int_{-L}^{L} \left[f(x)\right]^2 \ dx = \frac{a_0^2}{2} + \sum_{n=1}^{\infty} \left[ a_n^2 + b_n^2 \right]$$

___

### For interval (-&pi;, &pi;)
If the Fourier series of $f(x)$ is defined in $(-\pi, \pi)$ coverges uniformly to $f(x)$, then
$$\frac{1}{\pi}\int_{-\pi}^{\pi} \left[f(x)\right]^2 \ dx = \frac{a_0^2}{2} + \sum_{n=1}^{\infty} \left[ a_n^2 + b_n^2 \right]$$