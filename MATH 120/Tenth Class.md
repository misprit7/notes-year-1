# Tenth Class
Sep 20, 2019
* Negating statements involving quantifiers (e.g. $\forall, \exists,$ etc. )
  * Every well crafted mathematical statment is either true or false
  * If $S$ is a statmenet, either $S$ is true, or $S$ is false (equivalent to) "$S$ is false" is true
    * e.g. $\forall x\in \mathbb{R}, x^2\geq 0$
      * Negation is "$\forall x\in \mathbb{R}, x^2\geq 0$ is false"
      * i.e. $\exists x\in \mathbb{R}$ s.t. $x^2<0$
    * e.g. $\forall x\in \mathbb{R}, \exists y\in\mathbb{R}$ s.t. $y>x$
      * Negations is $\exists x\in\mathbb{R}$ s.t. $\forall y\in\mathbb{R}, y\leq x$
    * e.g. $\forall x\in\mathbb{R}, \exists y\in\mathbb{R}$ s.t. $\forall z\in\mathbb{R}, z>y>x$
      * Negation is $\exists x\in\mathbb{R}$ s.t. $\forall y\in\mathbb{R}, \exists z\in\mathbb{R}$ s.t. $z>y>x$ is false
        * Or $z\leq y$ or $y\leq x$, or both is true
        * Or $z>y$ and $y>x$ is false
* $\forall \epsilon>0, \exists \delta>0$ s.t. $\forall x\in\mathbb{R}$ with $0<|x-a|<\delta$, we have $|f(x)-L|<\epsilon$
* Negation: $\exists \epsilon>0$ s.t. $\forall \delta>0$, $\exists x\in\mathbb{R}$ with $0<|x-a|<\delta$, s.t. $|f(x)-L|\geq \epsilon$
  * e.g. $f(x)=2x, a=1, L=3, \lim_{x\to 1} f(x) = 3$ is false
    * The domain requirement holds (unfortunately)
    * Choose $\epsilon=\frac{1}{2}$
    * Let $\delta>0$
    * Choose $x=$min$(1, 1+\delta/2)$, then $0<|x-a|<\delta$
    * Then, $|f(x)-L|=|2x-3|\geq \epsilon<|2\cdot 1.1-3|=0.8\geq\frac{1}{2}=\epsilon$
    * Lets think about $|2x-3|$. Since $\epsilon>0, x=min(1.1, 1+\delta/2)$, we have $x>0$ and $x\leq 1.1$, so $|2x-3|=3-2x\geq 3-2\cdot 1.1$, since $x\leq 1.1$
  * e.g. Let $f(x)=\{1, x\in\mathbb{Q}; 0, x\notin\mathbb{Q}\}. lim_{x\to0} f(x)=\frac{1}{2}$
    * $\forall \epsilon>0, \exists \delta>0$ s.t. $\forall x\in\mathbb{R}$ with $0<|x|<\delta, |f(x)-\frac{1}{2}|<\epsilon$
    *  $\forall \epsilon>0, \exists \delta>0$ s.t. $\forall x\in\mathbb{R}$ with $0<|x|<\delta$, we have $|f(x)-\frac{1}{2}|<\epsilon$
    *  For every $L\in\mathbb{R}$, the statement $\lim_{x\to 0} f(x)=L$ is false
    * A.K.A. $\lim_{x\to 0} f(x)$ does not exist as a real number
    * $\forall L\in\mathbb{R}, \exists \epsilon > 0$ s.t. $\forall \delta>0, \exists x\in\mathbb{R}$ with $0<|x|<\delta$ s.t. $|f(x)-L|\geq \epsilon$
      * Let $L\in\mathbb{R}$
      * Select $\epsilon=\frac{1}{2}$
      * Let $\delta>0$
      * If $L\geq 1/2$, select a number $x\in(0, \delta)$ with $x\notin\mathbb{Q}$. The existance of such an $x$ was proved in homework 2. Then $|f(x)-L|=|0-L|=|L|\geq \frac{1}{2} \geq \epsilon$
      * If $L<1/2$, choose $x\in(0, \delta)$ with $x\in \mathbb{Q}$. Then $|f(x)-L|=|1-L|>\frac{1}{2}=\epsilon$








