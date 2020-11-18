# Ninth Class
Sep 18, 2019
* Let $f: D\to \mathbb{R}$, let $a\in \mathbb{R}$, let $L\in\mathbb{R}$ we say $\lim_{x\to a}f(x)=L$ if $\exists t>0$ s.t. $(a-t, a)\cup(a, a+t)\subset D(f)$ and $\forall \epsilon>0, \exists \delta>0$ s.t. $\forall x\in \mathbb{R}$ with $0<|x-a|<\delta$, we have $|f(x)-L|<\epsilon$
  * e.g. $f(x)=x^2, a=4, \lim_{x\to 4}f(x)=16$. Let's prove this using $\epsilon - \delta$ definition of a limit 
    * Since the domain of $f$ if $\mathbb{R}$, the domain requirement is met (i.e. take t=1)
    * Let $\epsilon>0$. Select $\delta =$min$(1, \epsilon /9)$
    * Let $x\in\mathbb{R}$ with $0<|x-4|<\delta$. Then
      * $|f(x)-L|=|x^2-16|=|(x+4)(x-4)|=|x+4|\cdot |x-4|<|x+4|\delta$
      * (cont.) $\leq (|x|+4)\delta\leq (5+4)\delta=9\delta$
  * e.g. $f(x)=2x\sin{\frac{1}{x}}, D(f)=\mathbb{R}\setminus\{0\}, \lim_{x\to0}f(x)=0$
    * Since $D(f)=\mathbb{R}\setminus \{0\}$, we can select $t=1$, and $(-1, 0)\cup(0, 1)\subset D(f)$
    * Let $\epsilon>0$. Select $\delta=\epsilon/2$
    * Let $x\in\mathbb{R}$ with $0<|x-0|<\delta$
    * Then $|f(x)-L|=|2x\sin(\frac{1}{x})|= 2|x||\sin(\frac{1}{x})|\leq 2|x|$
      * Since $R(\sin(x))\subset[-1, 1]$ so $|\sin(1/x)|\leq 1$
* Triangle Inequality
  * If $a, b, \in \mathbb{R}, |a+b|\leq |a|+|b|$