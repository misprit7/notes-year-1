# Thirteenth Class
Sep 25, 2019
* MLC M-F 12:00-17:00
  * LSK 301
* Quotient Rule: If $\lim_{x\to a}f(x)=L$, and $\lim_{x\to a}g(x)=M$, then $\lim_{x\to a}(\frac{f}{g})(x)=\frac{L}{M}$
  * Proof: From last class, $\lim_{x\to a} (\frac{1}{g(x)})=\frac{1}{M}$, now apply the product rule to $f$ and $\frac{1}{g}$ 
* "Limits are a local property": Let $f$ and $g$ be functions, and let $a\in\mathbb{R}$. If there exists $t>0$ so that $f(x)=g(x)$ for all $(1-t, a)\cup(a+t)$ (and in particular, both functions are defined), then if $\lim_{x\to a}f(x)=L$, we have $\lim_{x\to a}g(x)=L$
  * This small region is called a punctured region
  * e.g. $f(x)=x, g(x)=x$, but $D(g)=[-1, 1]\setminus\{0\}$
    * Since $\lim_{x\to 0}f(x)=0$ (limit rule for the identity) and $f(x)=g(x)$ for all $x\in(-1, 0)\cup(0, 1)$. By LAALP (limits are a local property), $\lim_{x\to 0}g(x)=0$
* Applications of limit rules
  * $\lim_{x\to a}(2x^2+x)=2a^2+a$
* Squeeze theorem
  * Let $f$, $g$ and $h$ be functions, and let $a\in\mathbb{R}$. Suppose there exists $t>0$ so that $f(x)\leq g(x)\leq h(x)$ for all $x\in(a-t, a)\cup(a, a+t)$. Suppose also that $\lim_{x\to a}f(x)=\lim_{x\to a}h(x)=L$. Then $\lim_{x\to a}g(x)=L$. 
  * Proof: The domain requirement is met because by the hypothesis of the theorem, there exists $t>0$ so that $x\in(a-t, a)\cup(a, a+t)$ is in the domain of $g(x)$. Next let $\epsilon>0$. 
    * Select $\epsilon_1=\epsilon/3$ and $\epsilon_2=\epsilon/3$
    * Since $\lim_{x\to a}f(x)=L$, there exists $\delta_1>0$ so that for all $x\in\mathbb{R}$ with $0<|x-a|<\delta_1$, we have $|f(x)-L|<\epsilon_1$. Similarly, there exists a $\delta_2$ analogous for $h(x)$. Let $\delta=\min(\delta_1, \delta_2, t)$. 
      * $t$ has to be included since the hypothesis of the theorem required that $x\in(a-t, a)\cup(a, a+t)$
    * Them, for all $x\in\mathbb{R}$ with $0<|x-a|<\delta$, we have $|g(x)-L|=|g(x)-f(x)+f(x)-L|\leq|g(x)-f(x)|+|f(x)-L|\leq |h(x)-f(x)|+|f(x)-L|$ for all $x\in(a-t, a)\cup(a, a+t)$. Therefore, $|h(x)-L+L-f(x)|+|f(x)-L|\leq |h(x)-L|+|f(x)-L|+f(x)-L|<\epsilon_2+\epsilon_1+\epsilon_1=\epsilon$
  * e.g. $g(x)=2x\sin{(\frac{1}{x})}$
    * Let $f(x)=-2|x|$ and $h(x)=2|x|$
    * $|g(x)|=2|x||\sin{(\frac{1}{x})}\leq 2|x|\Rightarrow |g(x)|\leq h(x)\Rightarrow g(x)\leq h(x)\forall x\neq0$ and $|g(x)|\geq -f(x)\Rightarrow g(x)\geq f(x) \forall x\neq 0$