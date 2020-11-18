# Twenty-First Class
Sep 11, 2019
* Polynomials are continuous
  * Proof 1: We will prove the theorem by induction on the number of terms in the polynomial. We will call this number $t$. 
    * Base case $t=0$: If a polynomial $P$ has $0$ terms, then it is the zero polynomial and that is continuous since constant functions are continuous. 
    * Induction step: Let $t\geq 0$ be an integer, and suppose that all polynomials with $t$ terms are continuous. We need to show that all polynomials with $t+1$ terms are continuous. Let $P$ be a polynomials with $t+1$ terms. we can express $P(x)=c_nx^n+Q(x)$, where $c_n\neq 0$ and $Q$ is a polynomial with $t$ terms. By the induction hypothesis, $Q$ is continuous. By our lemma, $x^n$ is continuous, so $c_nx^n$ is continuous. By the sum rule for continuous functions, $c_nx^n+Q(x)$ is continuous. 
  * Proof 2: We will prove the theorem by total induction on the degree of the polynomial. Let $n$ denote the degree of the polynomial. 
    * Base cases:
      * $n=-1$: The zero polynomial is continuous
      * $n=0$: Constant polynomials are continuous
    * Induction step: Let $n\geq$ be an integer, and suppose that all polynomials of degree $\leq n$ are continuous. We need to show that all polynomials of degree $n+1$ are continuous. Let $P$ be a polynomial of degree $n+1$. We can write 
$$
P(x)=\overbrace{\underbrace{c_{n+1}x^{n+1}}_{\textrm{cts. by lemma}}+\underbrace{Q(x)}_{\textrm{cts. by induction hypothesis}}}^{\textrm{cts. by sum rule}}
$$
* Types of discontinuities
  * $c\in(a, b)$, $f$ is continuous on $a, b)\setminus\{c\}$. $f$ is not continuous at $c$. 
  * Removable discontinuity: 
    * $\lim_{x\to c}f(x)$ exists as a real number, but either $c\notin D(f)$ (i.e. $f(c)$ does not exist) or $f(c)\neq \lim_{x\to c}f(x)$
  * Jump discontinuity: 
    * $\lim_{x\to c}f(x)$ does not exists, $\lim_{x\to c^+}f(x)$ and $\lim_{x\to c^-}f(x)$ exist as real numbers. 
  * Infinite Discontinuity
    * At least one of the one-sided limits is $\infty$ or $-\infty$, and the other one sided limit exists, either as a real number, $\infty$ or $-\infty$
  * Essential Discontinuity
    * None of the above
    * e.g. $f(x)=sin(\frac{1}{x})$




