# Twentieth Class
Sep 9, 2019
* Intermediate value theorem: Let $f:[a, b]\to\R$ be continuous. If $f(a)<f(b)$, then for every $y\in(f(a), f(b))$, there exists $x\in(a, b)$ so that $f(x)=y$. If $f(a)>f(b)$, then for every $y\in(f(b), f(a))$, there exists $x\in(a, b)$ so that $f(x)=y$
  * Define $g(x)=f(x)-y$. Then $g(x)$ is continuous on $[a, b]$ and $g(a)$ and $g(b)$ have opposite signs. By Bolzano's theorem, there exists $c\in(a, b)$ so that $g(c)=0$, hence $f(c)=y$
* Extreme value theorem: Let $f:[a, b]\to \R$ be continuous. Then there exist numbers $c, d \in[a, b]$ so that $f(x)\leq f(c)$ for all $x\in[a, b]$ and $f(x)\geq f(d)$ for all $x\in[a, b]$
  * $c$ and $d$ aren't necessarily unique
  * non-example: $f:[0, 1]\to\R, f(x)=x$
    * $c=1$, but there's no $d$ that is a minimum
* If $f$ and $g$ are continuous at a point $c\in\R$, then
  * $f+g, f-g, f\cdot g$ are continuous at $c$
  * $\frac{f}{g}$ is continuous at $c$, provided $g(c)\neq 0$
  * All of these statements are true if "continuous" is replaced by "right continuous" or "left continuous"
  * This follows from the rules for limits
* Constant functions $f(x)=k, k\in\R$ and the identity function $f(x)=x$ are also continuous (at every point $c\in\R$)
* Lemma: For every $n\in\Z, n\geq1$, the function $f(x)=x^n$ is continuous. 
  * We will prove this by induction on $n$. 
  * Base case: $n=1$. $f(x)=x$ is continuous, since $\lim_{x\to c}x=x\forall c\in\R$
  * Induction step: suppose the result is true for some positive integer $n$. We want to show the result is true for $n+1$. Let $f(x)=x^{n+1}=x^nx$. By the the "induction hypothesis", $x^n$ is continuous, and we know $x$ is continuous, so by the product rule for continuous functions, $f(x)=x^nx$ is continuous. 
* Theorem: Polynomials are continuous
  * We will prove the statement by induction on the degree of the polynomial. Let $n$ be the degree. 
  * Base case: $n=0$. If $P$ is a polynomial of degree $0$, then $P$ is a constant function and hence continuous
  * Induction step: Suppose the result is true for some positive integer n
  * Ran out of time, left as an "excercise$s"




