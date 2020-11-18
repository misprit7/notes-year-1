# Twenty-Ninth Class
Oct 28, 2019
* Recall: If $(a, b)$ is an interval, we say a function $f$ is differentiable on $(a, b)$ if it is differentiable for every point $c\in(a, b)$. Similarly for $[a, b]$. 
* If $(a, b)$ is an interval, and if $f, f^\prime, f^{\prime\prime}, \ldots f^{(n-1)}$ are differentiable at every point $c\in(a, b)$, then we say that $f$ is $n$-times differentiable on $(a, b)$
  * Same idea for $[a, b]$
  * e.g. If $f(x)=x^n, n\geq1$
    * We will prove in the homework that $f(x)$ is $n$-times differentiable, and $f^{(n)}=\frac{d^nf}{dx^n}=n!$
* Definition: If $n\geq1$, we define "$n$ facorial" as $n!=(n)(n-1)\ldots(2)(1)$
  * $0!=1$ by definition
* Taylor's series (intuition, not formal definition yet)
  * We want to approximate a curve at the point $x=0$ with polynomials of degree $i$ as $f_i(0)$
  * $f_1(x)=a_1x+a_0, a_0=f(0), a_1=f^\prime(0)$
  * $f_2(x)=a_2x^2+a_1x+a_0, a_0=f(0), a_1=f^\prime(0), a_2=\frac{f^{\prime\prime}(0)}{2}$
* Taylor's theorem: Let $f:[a, b]\to\R$. Suppose $f$ is $n$-times differentiable on $[a, b]$, and $f^{(n)}$ is continuous on $[a, b]$. Let $c\in[a, b]$. Then, for every $x\in[a, b]$ with $x\neq c$, there is a point $x_1$ in the interval between $c$ and $x$ (i.e. $x_1\in(x, c)$ if $x<c$ or $x_1\in(c, x)$) such that $f(x)=f(c)+\frac{f^{(1)}(c)}{1!}(x-c)+\frac{f^{(2)}(c)}{2!}(x-c)^2+\frac{f^{(3)}(c)}{3!}(x-c)^3+\ldots+\frac{f^{(n-1)}(c)}{(n-1)!}(x-c)^{n-1}+\underbrace{\frac{f^{(n)}(x_1)}{n!}(x-c)^n}_{\textrm{error term}}$. 
  * We can also write Taylor's theorem using summation notation: 
$$
f(x)=f(c)+\sum_{k=1}^{n-1}\frac{f^{(k)}(c)}{k!}(x-c)^k+\frac{f^{(n)}(x_1)}{n!}(x-c)^n
$$