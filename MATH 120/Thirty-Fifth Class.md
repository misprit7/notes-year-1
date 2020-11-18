# Thirty-Fifth Class
Nov 8, 2019
* If $f, g:(0, \infty)\to\R$, both are differentiable,$f(xy)=f(x)+f(y)$ and $g(xy)=g(x)+g(y)$ and $f^\prime(1)=g^\prime(1)$, then $f(x)=g(x)$ for all $x\in(0, \infty)$
  * To be proved in homework
* $\log(x)$
  * $D(\log)=(0, \infty)$
  * $R(\log)=\R$
  * $\log$ is strictly increasing
  * We defined $E(x)$ to be the inverse function of $\log(x)$
  * $E(a+b)=E(a)E(b)$
  * $E(1)=e$
* Lemma: If $n\geq1$ is an integer, then $E(n)=e$
  * Proof: induction
  * Also, $E(0)=1$
* Lemma: If $n\geq1$ is an integer, then $E(-n)=e^{-n}$
  * Proof: $1=E(0)=E(n-n)=E(n)E(-n)=e^nE(-n)$, so $E(-n)=\frac{1}{e^n}=e^{-n}$
* Lemma: If $\frac{p}{q}$ is rational, then $E(p/q)=e^{p/q}$
  * Proof: $e^p=E(q\cdot p/q)=E(p/q)^q$, so $e^{p/q}=E(p/q)$
  * We have shown that $E(x)=e^x$ if $x$ is rational
* What if $x$ is irrational? 
  * We define $e^x$to be $E(x)$
* Let's investigate the derivative of $E(x)$. 
  * We can apply our result about the derivatives of inverse functions to conclude: $E^\prime(x)=\frac{1}{\log^\prime(E(x)}=\frac{1}{\frac{1}{E(x)}}=E(x)$
  * By induction, $E^{(n)}(x)=E(x)$ for all $n\geq0, n\in\Z$
* Definition: a function is infinitely differentiable if you can take as many derivatives of the function as you want and it is still defined
* Question: what happens when we apply Taylor's theorem to $E(x)$? 
  * Select $c=0$, and choose $n>1$
  * We can write
$$
E(x)=E(0)+\sum_{k=1}^{n-1}\frac{E^{(k)}(0)}{k!}x^k+\frac{E^{(n)}(x_1)}{n!}x^n
$$
* Where $x_1$ is a point in the interval between $0$ and $x$
  * Since $E^{(k)}(0)=1$ for every $k$, 
$$
E(x)=1+\sum_{k=1}^{n-1}\frac{x^k}{k!}+\frac{E(x_1)}{n!}x^n\ (1)
$$
* Let's use $(1)$ to compute/approximate $e=E(1)$
$$
e=E(1)=\sum_{k=0}^{n-1}\frac{1}{k!}+\frac{E(x_1)}{n!}
$$
* Where $x_1\in(0, 1)$
  * Since $0<E(x)<E(1)=e$, we have
$$
\sum_{k=0}^{n-1}\frac{1}{k!}<e<\sum_{k=0}^{n-1}\frac{1}{k!}+\frac{e}{n!}\ (2)
$$
$$
e\frac{n!-1}{n!}<\sum_{k=0}^{n-1}\frac{1}{k!}
$$
$$
e<\frac{n!}{n!-1}\sum_{k=0}^{n-1}\frac{1}{k!}
$$
$$
e<\frac{6}{5}(1+1+\frac{1}{2})=3
$$
* So $(2)$ beomes
$$
\sum_{k=0}^{n-1}\frac{1}{k!}<e<\sum_{k=0}^{n-1}\frac{1}{k!}+\frac{3}{n!}
$$