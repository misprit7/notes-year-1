# Twenty-Sixth Class
Oct 22, 2019
* Theorem (positive derivative implies increasing): Let $f(a, b)\to\R$, let $c\in(a, b)$. Suppose $f$ is differentiable at $c$ and $f^\prime(c)>0$. Then there exists $t>0$ so that the follwoing two hold:
  * If $c<x<c+t$, then $f(x)>f(c)$
  * If $c-t<x<c$, then $f(x)<f(c)$
  * Analogous result holds if $f^\prime(c)<0$
  * Proof in homework (question 3)
* Let $f$ be a function, and let $c\in D(f)$. We say that $c$ is a local maximum of $f$ if there exists $t>0$ so that for all $x\in D(f)$ with $|x-c|<t$ we have $f(x)\leq f(c)$. Similarly, $c\in D(f)$ is a local minimum if there exists $t>0$ so that for all $\underbrace{x\in D(f)\cap(c-t, c+t)}_{\textrm{equivalent to the requirements for x above}}$, we have $f(x)\geq f(c)$ 
  * e.g. $f(x)=2$
    * Every $x\in\R$ is a local maximum and minimum
  * e.g. $f(x)=x$ if $x\in\Z$
    * Every $x\in D(f)=\Z$ is a local maximum and local minimum
  * e.g. $f(x)=\begin{cases}\frac{1}{q}, x\in\frac{p}{q}\textrm{ in lowest form}\\0, \textrm{otherwise}\end{cases}$
    * Thomae's function
    * Every $x\in\R\setminus\mathbb{Q}$ is a local minimum and every $x\in\mathbb{Q}$ is a local maximum
      * Very similar proof to homework 5
* Theorem: Let $f:(a, b)\to\R$, let $c\in(a, b)$ and suppose $f$ is differentiable at $c$. If $c$ is a local min, then $f^\prime(c)=0$. 
  * Proof: Suppose not. Then there is a point $c$ so that $c$ is a local maximum or minimum of $f$ and $f^\prime(c)>0$ or $f^\prime(c)<0$. We will consider the case where $c$ is a local maximum, and $f^\prime(c)>0$. Then other cases can be handled similarly, or dealt with by using the transformations $f\to-f$ or $f(x)\to f(-x)$. By our positive derivative implies increasing theorem, there exists $t_0>0$ so that for all $x\in(c, c+t_0)$, we have $f(x)>f(c)$. Since by assumption $c$ is a local max, there exists $t>0$ so that $f(x)\leq f(c)$ for all $x\in(c-t, c+t$)$. 
  * Let $x=c+\frac{1}{2}\min(t_0, t)$. Then $x\in(c, c+t_0)$ so $f(x)>f(c)$ and $x\in(c-t, c+t) so f(x)\leq f(c)$, implying a contradiction. 
* If $f$ is a function, a point $c\in D(f)$ is a global maximum of $f$ if $f(x)\leq f(c)$ for all $x\in D(f)$. Global minima are defined similarly. Strict global maxima/minima are when when the $\leq$ above is instead $<$, i.e. $f(x)<f(c)$ for all $x\in D(f)$
  * e.g. $\sin(x)+\frac{1}{100}x^2$