# Twenty-Second Class
Oct 15, 2019
* Let $f:(a, b)\to\R$, and let $c\in(a, b)$. We say that $f$ is differentiable at $c$ if $\lim_{x\to c}\frac{f(x)-f(c)}{x-c}$ exists (as a real number). We call this number $f^\prime(c)$
  * Note: $\frac{f(x)-f(c)}{x-c}$ is the slope ot the line connecting the points $(x, f(x))$ and $(c, f(c))$
  * Suppose $f$ is differentiable at $c$. Define $T(x)=f(c)+(x-c)f^\prime(c)$
    * A.K.A. $y=\underbrace{f^\prime(c)}_m+\underbrace{f(c)-cf^\prime(c)}_b$
  * Note: $\lim_{x\to c}\frac{f(x)-f(c)}{x-c}=\lim_{x\to 0}\frac{f(c+h)-f(c)}{h}$. It doesn't matter whcih variable we use for $c$, so we could also write $f^\prime(x)=\lim_{x\to 0}\frac{f(x+h)-f(x)}{h}$
* We say that a function $f$ is differentiable on an interval $(a, b)$ if it is differentiable at every point $x\in(a, b)$
  * i.e. $f^\prime(x)$ makes sense for every $x\in(a, b)$
  * e.g. $f(x)=k$ (constant function)
    * Let $x\in\R$ and $f^\prime(x)=\lim_{h\to 0}\frac{f(x+h)-f(x)}{h}=\lim_{h\to 0}\frac{k-k}{h}=\lim_{h\to 0}\frac{0}{h}=0$
  * e.g. $f(x)=x$
    * $f^\prime(x)=\lim_{h\to 0}\frac{f(x+h)-f(x)}{h}=\lim_{h\to 0}\frac{x+h-x}{h}=\lim_{h\to 0}\frac{h}{h}=1$
  * e.g. $f(x)=\begin{cases}x^2, x\in\mathbb{Q}\\ 0, x\in\R\setminus \mathbb{Q}\end{cases}$ For which $x\in\R$ is $f$ is differentiable? 
    * Let's try to show that $f$ is differentiable at $0$, i.e. $\lim_{h\to 0}\frac{f(h)-f(0)}{h}$ exists as a real number
    * Since $f(0)=0$, our job is to evaluate $\lim_{h\to 0}\frac{f(h)}{h}$
    * Let $g(h)=\begin{cases}h, x\in\mathbb{Q}\\ 0, x\in\R\setminus \mathbb{Q}\end{cases}$. We have $\frac{f(h)}{h}=g(h)$ for all $h\neq 0$
    * By limits are a local property, $\lim_{h\to 0}\frac{f(h)}{h}=\lim_{h\to 0}g(h)=0$ (proved in lecture)
  * e.g. $f(x)=x^2$. 
    * $\lim_{h\to 0}\frac{(f(x+h)-f(x)}{h}=\lim_{h\to 0}\frac{(x+h)^2-x^2}{h}=\lim_{h\to 0}\frac{x^2+2xh+h^2-x^2}{h}$
    * $=\lim_{h\to 0}\frac{2xh+h^2}{h}=\lim_{h\to 0}(\frac{2xh}{h}+\frac{h^2}{h})=\lim_{h\to 0}\frac{2xh}{h}+\lim_{h\to 0}\frac{h^2}{h}$. This will be justified by the sum rule for limits once both limits are shown to exist. The next step is justified by limits are a local property
    * $=\lim_{h\to 0}2x+\lim_{h\to 0}h=2x$
  * e.g. $f(x)=|x|$ For which $x$ is this function differentiable? What about not differentiable? 
    * Everywhere exept 0
    * If $x>0$, then $f^\prime(x)=\lim_{h\to 0}\frac{f(x+h)-f(x)}{h}$. Let $g(y)=y$. $g(y)=f(y)$ for all $y\in(x-t, x+t)$, where $t=x$. By limits are a local property, $\lim_{h\to 0}\frac{f(x+h)-f(x)}{h}=\lim_{h\to 0}\frac{g(x+h)-g(h)}{h}=1$ since $g(y)=y$. If $x<0$, then we can do the same thing with $g(y)=-y$. If $x=0$, we need to prove that $f$ is not differentiable.  






