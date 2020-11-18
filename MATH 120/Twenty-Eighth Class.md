# Twenty-Eighth Class
Oct 25, 2019
* Rolles Theorem: Let $f:[a, b]\to\R$. Suppose $f$ is continuous on $[a, b]$, differentiable on (a, b), and $f(a)=f(b)$. Then there exists $c\in(a, b)$ with $f^\prime(c)=0$
  * Proof: By the extreme value theorem, there are points $c_1$ and $c_2\in[a, b]$ so that $c_1\leq f(x)\leq c_2$ for all $x\in(a, b)$. If either $c_1$ or $c_2$ is in $(a, b)$, then $c_1$ or $c_2$ is a local minimum or maximimum, and thus the derivative is $0$ at that point. If this does not happen, then either 
    * $c_1=c_2$. Then $f$ is constant, so $f^\prime(c)=0$ for every $c\in(a, b)$
    * $c_1=a$ and $c_2-b$ or vice versa. Since $f(a)=f(b)$, we have $f(c_1)=f(c_2)$, so $f$ is constant and $f^\prime(c)=0$ for every $c\in(a, b)$
* Mean value theorem: Let $f:[a, b]\to\R$. Suppose $f$ is continuous on $[a, b]$ and differentiable on (a, b). Then there exists $c\in(a, b)$ such that $f(b)-f(a)=f^\prime(c)\cdot (b-a)$
  * General proof talk through: Let $f_1(x)=f_1(x)-\frac{f(b)-f(a)}{b-a}x$, so $f_1(a)=f_1(b)$. Then you can apply Rolles theorem
  * Essentially subtracting a linear function that satisfies the hypothesis for Rolles theorem
* Generalized mean value theorem: Let $f:[a, b]\to\R$ and $g:[a, b]\to\R$. These two functions are continuous on $[a, b]$ and differentiable on $(a, b)$. Then there is a point $c\in(a, b)$ so that $f^\prime(c)\cdot (g(b)-g(a))=g^\prime(c)\cdot (f(b)-f(a))$
  * Note: setting $g(x)=x$, we recover the mean value theorem
  * Proof: Let $h(x)=f(x)(g(b)-g(a))-g(x)(f(b)-f(a))$. This function is continuous on $[a, b]$, and differentiable on $(a, b)$. Thus $h(a)=h(b)$: 
    * $h(a)=f(a)(g(b)-g(a))-g(a)(f(b)-f(a))=f(a)g(b)-g(a)f(b)$
    * $h(b)=f(b)(g(b)-g(a))-g(b)(f(b)-f(a))=f(a)g(b)-g(a)f(b)$
  * By Rolle's theorem, there exists $c\in(a, b)$ with $h^\prime(c)=0$. Thus, $0=h^\prime(c)=f^\prime(c)(g(b)-g(a))-g^\prime(c)(f(b)-f(a))$
* Higher derivatives: Let $f$ be a function. We write $f^\prime(c)$ to be the derivative of $f$ at $c$. Then $D(f^\prime)=\{c\in\R: f\textnormal{ is differentiable at }c\}$. Since $f^\prime$ is a function (with domain $D(f^\prime)$, make sense to ask whether $f^\prime$ is differentiable at a point $c\in\R$. If it is, we denote its derivative by $(f^\prime)^\prime=f^{\prime\prime}(c)$ or $f^{(2)}(c)$. We can continue this process, and define $f^{\prime\prime\prime}$ (or $f^{(3)}$), etc. 
  * Some alternate notations: 
    * $f^\prime(x)=f^{(1)}(c)=\frac{df}{dx}(c)=\frac{df(x)}{dx}|_{x=c}$
    * $f^{\prime\prime\prime\ldots}=f^{(n)}=\frac{d^nf}{dx^n}(c)=\frac{d^nf(x)}{dx^n}|_{x=c}$ 



