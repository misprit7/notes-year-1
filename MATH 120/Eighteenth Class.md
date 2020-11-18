# Eighteenth Class
Oct 7, 2019
* Let $f$ be a function and let $A\in\R$. We say that $f$ is continuous at $a$ if $\lim_{x\to a}f(x)=f(a)$. In particular, this implies that $a\in D(f)$, $f(a)\in\R$, and $\lim_{x\to a}f(x)$ exists as a real number. 
  * If $f$ is not coninuous at $a$, we say it is discontinuous at $a$
    * $a$ should be in the domain of $f$
  * e.g. $f(x)=\{x if x\in\mathbb{Q}, 0 if x\notin\mathbb{Q}\}$
    * Continuous at 0, since $\lim_{x\to 0}f(x)=0=f(0)$
* If $\lim_{x\to a^+}f(x)=f(a)$, we say $f$ is right continuous. If $\lim_{x\to a^-}f(x)=f(a)$, we say $f$ is left continuous. 
* Let $f$ be a function, and let $(a, b)$ be an open interval. We say that $f$ is continuous on $(a, b)$ is it is continuous at every point $c\in(a, b)$
  * More advaned way of saying this: Let $I$ be an open interval, and let $f$ be continuous on $I$. 
* If $[a, b]$ is a closed interval, $f$ is a function, we say $f$ is continuous on $[a, b]$ if $\lim_{x\to c}f(x)=f(c)$ for all $c\in(a, b)$, $\lim_{x\to a^+}f(x)=f(a)$, $\lim_{x\to b^-}f(x)=f(b)$
* Lemma 1: Let $f$ be a function that is continuous at the point $c\in\R$. If $f(c)>0$, then there exists $\delta>0$ so that $f(x)$ is defined and $f(x)>0$ for all $x\in(c-\delta, c+\delta)$. SImilarly, if $f(c)<0$, then there exists $\delta>0$ so that $f(x)<0$ for all $x\in(c-\delta, c+\delta)$ (slightly modified on Sep 7th, so the below proof isn't perfect)
  * Since $f$ is continuous at $c$, $\lim_{x\to c}f(x)=f(c)\neq 0$. Choose $\epsilon=|\frac{f(c)}{2}|$. Then $\exists\delta>0$ such that $\forall x\in\R$ with $0<|x-c|<\delta$ we have that $f(x)$ exists and $|f(x)-f(c)|<\epsilon=|\frac{f(c)}{2}|$. Thus $|f(x)|>\frac{\epsilon}{2}=\frac{|f(c)|}{4}$, so in particular $f(x)\neq 0$ since $f(c)\neq 0$. 
* Bolzano's theorem: Let $f$ be continuous on the closed interval $[a, b]$. Suppose that $f(a)$ and $f(b)$ have opposite signs, i.e. $f(a)>0$ and $f(b)<0$ or $f(a)<0$ and $f(b)>0$. Then there exists $c\in(a, b)$ such that $f(c)=0$
  * Theorem isn't true when just considering the rationals
    * Counterexample: $f(x)=x^2-2$, since its roots are $\sqrt{2}$







