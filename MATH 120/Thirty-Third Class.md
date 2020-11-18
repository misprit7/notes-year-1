# Thirty-Third Class
Nov 4, 2019
* Review of last class
  * $f(xy)=f(x)+f(y)$ $(*)$
  * $D(f)=(0, \infty)$
  * $f$ is differentiable on $(0, \infty)$
  * What does this tell us? 
    * $F(1)=0$
    * $f^\prime(x)=\frac{f^\prime(1)}{x}=\frac{b}{x}$, where $b\in\R$, b=$f^\prime(1)$
* Lemma: For every integer $n\geq 1$, $f(2^n)=nf(2)$
  * Can be proven by induction
* Lemma: $\lim_{x\to\infty}f(x)=\infty$
  * Since $D(f)=(0, \infty)$, the domain requirement is met. Next, let $M\in\R$. Select $n$ to be a non-negative integer so that $nf(2)>M$ (If $M\leq 0$, let $n=1$. Otherwise, let $n$ be an integer larger than $\frac{M}{f(2)}$). Let $=2^n$. If $x\in\R$ and $x>\R$, then $f(x)>f(R)=f(2^n)=nf(2)>M$
* Lemma: For every integer $n\geq 1$, $f(2^{-n})=-nf(2)$
  * Proof: $0=f(1)=f(2^{n}\cdot 2^{-n})=f(2^n)+f(2^{-n})=nf(2)+f(2^{-n})$
* Lemma: $\lim_{x\to0^+}f(x)=-\infty$
  * Proof left as an exercise
* Lemma: If $f$ is a strictly increasing continuous function on the interval $(0, \infty)$ and if $\lim_{x\to0^+}f(x)=-\infty$ and $\lim_{x\to\infty}f(x)=\infty$, then for every $y\in\R$, there is a unique $x\in(0, \infty)$ so that $f(x)=y$
  * Proof 1: $\forall y\in\R$, $\exists x\in(0, \infty)$ such that $f(x)=y$
    * Intermediat value theorem
  * Proof 2: there is at most one such $x$
    * $f$ is strictly increasing
* Definition: Let $f$ be a nonzero function with domain $(0, \infty)$ that is differentiable on $(0, \infty)$ and satisfies $f(x\cdot y)=f(x)+f(y)$ for all $x, y\in(0, \infty)$. Let $b$ be the unique number so that $f(b)=1$. We will call $f(x)$ $\textnormal{``} \log_b(x)\textnormal{''}$