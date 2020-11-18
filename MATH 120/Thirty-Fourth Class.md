# Thirty-Fourth Class
Nov 11, 2019
* Inverse functions
  * Recall: let $f$ be a function. The range of $f$ is the set $\{f(x):x\in D(f)\}$
  * We say $f$ is one-to-one or injective if whenever $x_1\neq x_2$, $f(x_1)\neq f(x_2)$
    * Equivilantly, $f(x_1)=f(x_2)$ if and only if $x_1=x_2$
  * Definition: Let $f$ be a one-to-one function. We define the inverse function, $f^{-1}$ as follows: $f^{-1}(y)$ is the (unique) $x\in D(f)$ so that $f(x)=y$
    * $D(f^{-1})=R(f)$
    * e.g. $f(x)=x^2$, $D(f)=[0, \infty), R(f)=[0, \infty)$
      * $f^{-1}(x)=\sqrt x$, $D(f^{-1})=R(f)=[0, \infty), R(f^{-1})=D(f)=[0, \infty)$
    * e.g. $f(x)=x^2$, $D(f)=(-\infty, 0], R(f)=[0, \infty)$
      * $f^{-1}(x), D(f^{-1})=[0, \infty), R(f^{-1})=(-\infty, 0]$
  * Careful: $F^{-1}(x)$ is not $\frac{1}{f(x)}$
  * The graph of $f^{-1}$ is obtained by reflecting the graph of $f$ accross the line $y=x$
* Properties of inverses
  * $(f^{-1})^{-1}=f$
  * If $x\in D(f)$, then $f^{-1}(f(x))=x$
  * If $x\in D(f^{-1}=R(f)$, then $f(f^{-1}(x))=x$
* If $x\in D(f^{-1}$, $f^{-1})$ is differentiable at $x$, and $f$ is differentiable at $f^{-1}(x)$, then $1=x^\prime=f^\prime(f^{-1}(x))(f^{-1})^\prime(x)$
  * Hence, $(f^{-1})^\prime(x)=\frac{1}{f^\prime(f^{-1}(x))}$ if $f^\prime(f^{-1}(x))\neq0$
  * e.g. $f(x)=x^2, D(f)=[0, \infty)$. $f^{-1}(x)=\sqrt x$
    * $(f^{-1})^\prime(x)=\frac{1}{f^\prime(f^{-1}(x))}=\frac{1}{2\sqrt x}$
* Recall from last class: If $f$ is differentiable on $(, \infty)$ and satisfies $f(xy)=f(x)+f(y) (*)$ for all $x, y\in (0, \infty)$, then $f(1)=0, f^\prime(x)=\frac{f^\prime(x)}{x}$ and either $f$ is constant or $f(x)\log_bx$, where $b>1$ is the unique number satisfying $f(b)=1$
  * If $f^\prime(x)=\frac{1}{x}$, then the corresponding number $b>1$ that satisfies $f(b)=1$ is roughly equal to $2.71\ldots$. We call this number $e$
  * We will call $\log_e(x)$ just $\log x$
* Question: what is the inverse function of $\log(x)$
  * It is a function whose domain is $\R$ and whose range is $(0, \infty)$. We will call this function $E(x)$
  * $\log(e)=1\to E(1)=e$
  * $E(a+b)=E(a)E(b)a, b\in \R$
    * Proof: Let $x=E(a)$, let $y=E(b)$, and let $c=\log(xy)$. So $\log(x)=a, \log(y)=b, E(c)=xy$. But $c=\log(xy)=\log(x)=\log(y)=a+b$, i.e. $c=a+b$