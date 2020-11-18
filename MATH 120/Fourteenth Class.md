# Fourteenth Class
Sep 27, 2019
* One side limits
  * Let $f$ be function and $a, L\in\mathbb{R}$. We say $\lim_{x\to a^+}f(x)=L$ or $\lim_{x\searrow a}f(x)=L$ if the following holds:
    * There exists $t>0$ so that $(a, a+t)\subset D(f)$
    * $\forall\epsilon>0, \exists\delta>0$ such that $\forall x\in\mathbb{R}$ with $\underbrace{0<x-a<\delta}_{\textrm{no absolute values}}$, we have $|f(x)-L|<\epsilon$
  * We say $\lim_{x\to a^-}f(x)=L$ or $\lim_{x\nearrow a}f(x)=L$ if the same requirements hold as above except with $x\in(a-\delta, a)$ and $(a-t)\subset D(f)$
  * Let $f$ be a function, let $a, L\in\mathbb{R}$. Then $\lim_{x\to a}f(x)=L$ if and only if $\lim_{x\to a^+}f(x)=L$ and $\lim_{x\to a^-}f(x)=L$
* Limits at infinity
  * Let $f$ be a function and $L\in\mathbb{R}$. We say $\lim_{x\to\infty}f(x)=L$ if:
    * There exists $T\in\mathbb{R}$ so that $(T, \infty)\subset D(f)$
    * $\forall \epsilon>0, \exists R\in\mathbb{R}$ such that if $x\in\mathbb{R}$ and $x>R$, then $|f(x)-L|<\epsilon$
    * e.g. $f(x)=\frac{1}{x}$
      * Let $\epsilon>0$. Select $R=\frac{2}{\epsilon}$. If $x\in(R, \infty)$, then $|f(x)-L|=|f(x)|=|\frac{1}{x}|=\frac{1}{x}<\frac{1}{R}=\frac{\epsilon}{2}<\epsilon$
  * There is also the analogous definition of limits trending towards negative infinity
* e.g. $f(x)=\sin x$
  * $\sin x=\sin(2\pi+x)$
  * For every $L\in\mathbb{R}$, the statement $\lim_{x\to\infty}\sin x=L$ is false
  * Proof:Let $L\in\mathbb{R}$. Since $D(f)=\mathbb{R}$, the domain requirement is met (unfortunately). Select $\epsilon=1$. Let $R\in\mathbb{R}$. If $L\leq 0$, select a number $x\in\mathbb{R}$ with $x>R$ of the form $x=\pi/2+2\pi n, n\in\mathbb{R}$. Then $f(x)=1$, so $|f(x)-L|=1-L\geq 1=\epsilon$. If $L>0$, then select $x\in\mathbb{R}$ with $x>R$ of the form $x=3\pi/2+2\pi n, n\in\mathbb{R}$. Then $f(x)=-1$, so $|f(x)-L|=|-1-L|=1+L>1=\epsilon$


