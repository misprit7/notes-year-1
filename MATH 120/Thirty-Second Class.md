# Thirty-Second Class
Nov 1, 2019
* Suppose we have a function $f$ that satisfies $f(xy)=f(x)+f(y)$ $(*)$ whenever $x, y, xy\in D(f)$
  * $f(x)=0$ for all $x$ satisfies $(*)$
    * If $D(f)=\R$, then $f(x)=0$ is the only solution
    * Proof: Let $f$ satisfy $(*)$ and have domain $D(f)=\R$. Let $x\in\R$. Then $f(0)=f(x\cdot 0)=f(x)+f(0)\to f(x)=0$
    * Indeed, if $0\in D(f)$ and $f$ satisfies $(*)$ then $f(x)=0$ for all $x\in D(f)$
  * What about functions satisfying $(*)$ who's domain is $\R\setminus\{0\}$
    * Well, $f(1)=f(1\cdot 1)=f(1)+f(1)=2f(1)$, so $f(1)=0$
    * Also, $0=f(1)=f((-1)(-1))=f(-1)+f(-1)=2f(-1)$, so $f(-1)=0$
    * Next, $f(-x)=f((-1)x)=f(-1)+f(x)=f(x)$, so for all $x\in D(f)=\R\setminus \{0\}$, $f(x)=f(-x)$
    * Definition: If $g$ is a function satisfying $g(x)=g(-x)$ for all $x\in D(g)$, then $g$ is called an even function
    * Definition: If $g$ is a function satisfying $g(-x)=-g(x)$ for all $x\in D(g)$, then $g$ is called odd
  * Thus, we can restrict our attention to functions $f$ satisfying $(*)$ who's domain is $(0, \infty)$. Let's add one more assumption, which is that $f$ is differentiable on $(0, \infty)$
    * Lets fix a number $y\in(0, \infty)$, and define $g(x)=f(x\cdot y)$ ($D(g)=(0, \infty)$)
    * We have $g^\prime(x)=yf^\prime(xy)$
    * We also know $g(x)=f(x)+f(y)$, so $g^\prime(x)=f^\prime(x)$
    * Thus, $yf^\prime(xy)=f^\prime(x)$ for all $x\in(0, \infty)$
    * Setting $x=1$, we have $yf^\prime(y)=f^\prime(1)$ and $f^\prime(y)=\frac{f^\prime(1)}{y}$ $(**)$
    * $(**)$ is called a differentiable equation
    * What is $f^\prime(1)$? A real number, call it $c$
    * We want to understand a function $f$ that satisifies $f^\prime(1)-0$, and $f^\prime(y)=\frac{c}{y}$
    * We will borrow from Math 121, so $f(x)$ is $c$ times the area under graph of the function $g(x)=\frac{1}{x}$ from $1$ to $x$
  * Let's assume that $f^\prime(1)>0$ (if $f^\prime(1)<0$, then everything that follows remains true, but "increasing" changes to "decreasing")
    * Observe that $f^\prime(x)>0$ for all $x\in (0, \infty)$
    * Definition: Let $S\sub\R$ be a set and let $g$ be a function whose domain contains $S$. We say that $g$ is increasing on $S$ if for all $x, y\in S$ with $x\geq y$, we have $g(x)\geq g(y)$. We say $g$ is strictly increasing on $S$ if for all $x, y\in S$ with $x>y$, $g(x)>g(y)$ (same but opposite for decreasing and strictly decreasing analogously)