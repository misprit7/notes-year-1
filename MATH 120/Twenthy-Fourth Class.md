# Twenthy-Fourth Class
Oct 18, 2019
* Power rule: If $f(x)=x^n, n\geq 2$, $f^\prime(x)=nx^{n-1}$
  * Proof: We will prove this by induction on $n$. 
  * Base case: $n=2$. If $f(x)=x^2=x\cdot x$, then by the product rule, $f^\prime(x)=(x^\prime)(x)+(x)(x^\prime)=x+x=2x$
  * Induction step: Suppose that the result is true for some $n\geq2$, and let $f(x)=x^{n+1}=x^n\cdot x$. $f^\prime(x)=(x^\prime)(x^n)+(x)(x^n)^\prime=x^n+x(nx^{n-1})=(n+1)x^n$
* Corollary of the power rule
  * If $P(x)=a_nx^n+a_{n-1}x^{n-1}+\ldots +a_0$, then $P^\prime(x)=na_nx^{n-1}+(n-1)a_{n-1}x^{n-2}+\ldots +a_1$
* Reciprocal rule: If $f$ is differentiable at $x$, and $f(x)\neq 0$, then $(\frac{1}{f})^\prime(x)=\frac{-f^\prime(x)}{(f(x))^2}$
  * $D(\frac{1}{f})=D(f)\setminus \{x\in\R:f(x)=0\}$
  * Proof: $(\frac{1}{f})^\prime=\lim_{h\to 0}\frac{\frac{1}{f(x+h}-\frac{1}{f(x)}}{h}=$
  * $\lim_{h\to 0}\frac{-1}{f(x)+h)f(x)}\cdot \frac{f(x)+h-f(x)}{h}=(\lim_{h\to 0}\frac{1}{f(x)+h})\cdot (\lim_{h\to 0}\frac{-1}{f(x)})\cdot (\lim_{h\to 0}\frac{f(x+h)-f(x)}{h})$
  * $=\frac{1}{f(x)}\cdot \frac{-1}{f(x)}\cdot f^\prime(x)=\frac{-f^\prime(x)}{(f(x))^2}$
* Corallary of the reciprocal rule: If $n\geq 1$ is an integer and $f(x)=x^{-n}$, then $f^\prime=-nx^{-n-1}$
  * Proof: left as an exercise (of course)
* Quotient rule: Let $f$ and $g$ be differentiable at $x$, and suppose $g(x)\neq 0$. Then $(\frac{f}{g})^\prime(x)=\frac{g(x)f^\prime(x)-f(x)g^\prime(x)}{(g(x))^2}$
  * Proof: Write $(\frac{f}{g})(y)=f(y)\cdot \frac{1}{g(y)}$. Apply the product rule, then the reciprocal rule. $(\frac{f}{g})(x)=f^\prime(x)\cdot \frac{1}{g}(x)+f(x)\cdot (\frac{1}{g})^\prime(x)=f^\prime\cdot \frac{1}{g}(x)+f(x)\cdot \frac{(-1)g^\prime(x)}{(g(x))^2}=\frac{f^\prime(x)g(x)-f(x)g^\prime(x)}{(g(x))^2}$
* Theorem: Let $:(a, b)\to \R$, let $c\in(a, b)$ and suppose $f$ is differentiable at $c$. Then there exists a function $f^*:(a, b)\to\R$ ($f^*$ depends on $f$ and $c$) so that $f^*$ satisfies the equation $f(x)-f(c)=(x-c)f^*(x)$ (for all $x\in(a, b)$) and $f^*$ is continuous at $c$
  * Thinking about what this means:
    * If $f$ is a polynomial, then we can write $f(x)-f(c)=(x-c)g(x)$, where $g$ is a polynomial of one lower degree