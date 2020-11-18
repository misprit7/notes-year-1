# Twenty-Fifth Class
Oct 21, 2019
* Theorem: Let $f:(a, b)\to \R$, let $c\in(a, b)$ and suppose $f$ is differentiable at $c$. Then there exists $f^*:(a, b)\to\R$ that satisfies the equation $f(x)-f(c)=(x-a)f^*(x)$, $f^*$ is continuous at $c$ and $f^*(c)=f^\prime(c)$
  * Proof: for $x\in(a, b)$, define $f^*(x)=\begin{cases}\frac{f(x)-f(c)}{x-c}, x\neq c\\f^\prime(c), x=c\end{cases}$
  * The main thing to show is that $f^*$ is continuous at $c$, i.e. $\lim_{x\to c}f^*(x)=f(c)=f^\prime(c)=\lim_{x\to c}\frac{f(x)-f(c)}{x-c}$
* Conversely (to the above theorem and proof), if $f:(a, b)\to\R$, if $c\in(a, b)$ and if there exists a function $f^*:(a, b)\to\R$, that is continuous at $c$ and satisfies $f(x)-f(c)=(x-c)f^*(x)$ for all $x\in(a, b)$, then $f$ is differentiable at $c$, and $f^\prime(c)=f^*(c)$
  * Proof is an exercise (because why could he make it easy?)
* Chain rule: If $g$ is differentiable at $c$, and if $f$ is differentiable at $g(c)$, then the composition $f\circ g$ is differentiable at $c$, and $(f\circ g)^\prime(c)=f^\prime(g(c))g^\prime(c)$
  * Proof: Since $g$ is differentiable at $c$, there exists $t_1>0$ so that $(\underbrace{c-t_1}_{a_1}, \underbrace{c+t_1}_{b_1})\sub D(g)$. Let $d=g(c)$. Since $f$ is differentiable at $d$, there exists $t_2>0$ so that $(\underbrace{d-t_2}_{a_1}, \underbrace{d+t_2}_{b_2})\sub D(f)$. Using our previous theorem, we can write $g(x)-g(c)=(x-c)g^*(x)$ for all $x\in(a_1, b_1)$ where $g^*(x):(a, b)\to\R$ is continuous at $c$ and $g^*(c)=g^\prime(c)$. Similarly, we can write $f(x)-f(d)=(x-d)f^*(x)$ for all $x\in(a_2, b_2)$, where $f^*:(a, b)\to\R$ is at $d$ and $f^*(d)=f^\prime(d)$. 
  * Since $g$ is continuous at $c$ (since it's differentiable at $c$), there exists $\delta>0$ so that for all $x\in\R$ with $|x-c|<\delta$, we have $|g(x)-d|<t_2$, i.e. $g(x)\in (a_2, b_2)$, so $f\circ g(x)$ makes sense. In other words, $x\in D(f\circ g)$
  * Let $t_1^\prime=\min(t_1, \delta)$. Then if $x\in(c-t_1^\prime, c+t_1^\prime)$, $f(g(x))-f(g(c))=(g(x)-g(c))f^*(g(x))=(x-c)g^*(x)f^*(g(x))$ (using the fact that $g(x)\in(a_2, b_2)$), so $f\circ g(x)-f\circ (c)=(x-c)g^*(x)f^*(g(x))$. If $x\neq c$, then $\frac{f\circ g(x)-f\circ g(c)}{x-c}=g^*(x)f^*(g(x))$
  * Observations: 
    * $\lim_{x\to c}\frac{f\circ g(x)-f\circ g(c)}{x-c}=(f\circ g)^\prime(c)$ (if it exists)
    * $\lim_{x\to c}g^*(x)=g^*(c)=g^\prime(c)$
    * $\lim_{x\to c}f^*(g(x))=f^*(g(c))=f^\prime(g(c))$
      * Recall homework 2: if $\lim_{x\to a}g(x)=b$ and $\lim_{x\to b}f(x)=L$, it need not be true that $\lim_{x\to a} f(g(x))=L$
  * Putting it together, we conclude that $(f\circ g)^\prime(x)$ exists and is equal to $f^\prime(g(c))g^\prime(c)$