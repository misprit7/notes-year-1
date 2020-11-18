# Sixteenth Class
Oct 1, 2019
* A polynomial is a function of the following form: $f(x)=a_n x^n+a_{n-1} x^{n-1} + \ldots + a_1 x +a_0$, $n\geq 0$, where $a_n, \ldots, a_0$ are real numbers and $a_n\neq 0$. We define the degree of $f$ to be $n$, we write this as $\deg(f)$. Additionally, we say that the function $f(x)=0$ is also a polynomial, and we define its degree to be $-1$
  * Polynomials have to have a domain of all real numbers
* A rational function is a function of the form $f(x)=\frac{P(x)}{Q(x)}$ where $P$ and $Q$ are polynomials and $Q$ is not the zero polynomial. 
  * e.g. $f(x)=\frac{x^2+1}{2x+4}, D(f)=\R\setminus\{-2\}$
  * e.g. $f(x) = \frac{x^3+2x+4}{1}$
* Let $P$ and $Q$ be nonzero polynomials of degree $n$ and $m$ respectively. Let $f(x)=\frac{P(x)}{Q(x)}$. 
  * (1) If $\deg(P)<\deg(Q)$, then $\lim_{x\to\infty}f(x)=0$. 
  * (2) If $\deg(P)=\deg(Q)$, then $\lim_{x\to\infty}f(x)=\frac{a_n}{b_m}$. 
  * (3) If $\deg(P)>\deg(Q)$, then $\lim_{x\to\infty}f(x)=\infty$ if $\frac{a_n}{b_m}>0$ and $\lim_{x\to\infty}f(x)=-\infty$ if $\frac{a_n}{b_m}<0$
* Proof of (2): Let $P(x) = a_nx^n+\ldots a_0$ and $Q(x) = b_nx^n+\ldots b_0$ be polynomials. We want to show that $\lim_{x\to\infty}\frac{P(x)}{Q(x)}=\frac{a_n}{b{n}}$
  * Scratch
    * Let $P(x) = a_nx^n+\ldots a_0$, and define $A=|a_n|+\ldots+|a_0|$. If $x\geq1$, then $|a_{n-1}x^{n-1}+\ldots+a_0|\leq A|x|^{n-1}$
      * Iterated use of the triangle inequality gives $|a_{n-1}x^{n-1}+\ldots+a_0|\leq|a_{n-1}||x|^{n-1}+\ldots +|a_0|1$. Since $x\geq 1$, $\leq |a_{n-1}||x|^{n-1}+\ldots +|a_0|x^{n-1}=A|x|^{n-1}$. We conclude: if $x\geq 1$, then $a_nx^n -Ax^{n-1}\leq P(x)\leq a_nx^n + Ax^{n-1}$. Similarly for $Q(x)$ except with $B$ instead of $A$
    * $\frac{P(x)}{Q(x)}-\frac{a_n}{b_n}=\frac{P(x)b_n-a_nQ(x)}{Q(x)b_n}=\frac{(a_nx^n+\ldots a_0)b_n-a_n(b_nx^n+\ldots b_0)}{b_n(b_nx^n+\ldots b_0)}=\frac{a_{n-1}b_n-anb_{n-1}x^{n-1}+\ldots a_0b_n-a_0b_n}{b_n\cdot b_nx^n+\ldots b_n\cdot b_0)}$








