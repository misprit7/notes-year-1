# Twenty-Third Class
Oct 16, 2019
* $f(x)=|x|$, $D(f)=\R$
* Last time, $f$ is differentiable at $x$ for all $x\neq 0$
  * Next, we will show $f$ is not differentiable at $0$. Lets evaluate $\lim_{x\to 0}\frac{f(0+h)-f(0)}{h}=\lim_{x\to 0}\frac{|h|}{h}$. This limit does not exist, since $\lim_{x\to 0^-}\frac{|h|}{h}=-1\neq 1=\lim_{x\to 0^+}\frac{|h|}{h}$
* One sided derivatives: If $\lim_{x\to 0^+}\frac{f(x+h)-f(x)}{h}$ exists as a real number, then we say that $f$ is right differentiable at $x$. Similarly for being left differentiable at $x$. 
  * $f^{\prime}_+(x)=\lim_{x\to 0^+}\frac{f(x+h)-f(x)}{h}$
  * $f^{\prime}_-(x)=\lim_{x\to 0^-}\frac{f(x+h)-f(x)}{h}$
* Recall: if $f:(a, b)\to\R$ we say $f$ is differentiable on $(a, b)$ if it is differentiable at every point $x\in(a, b)$. 
* If $f:[a, b]\to\R$, we say $f$ is differentiable on $[a, b]$ if $f$ is differentiable at every point $x\in(a, b)$, $f$ is right differentiable at $a$ and $f$ is left differentiable at $b$
  * e.g. We could say $f(x)=|x|$ is differentiable on $(0, 1)$. We could also say $f$ is differentiable on $(0, \infty)$. $f$ is not differentiable on $(-1, 1)$
  * $f(x)=|x|$ is continuous at $0$. 
    * Proof: Let $\epsilon>0$. Select $\delta=\epsilon$. If $|x|<\delta$, then $|f(x)-f(0)|=||x||=|x|\leq \delta=\epsilon$
* The example $f(x)=|x|$ shows that it is possible for a function to be continuous at a point $c\in\R$, but to not be differentiable at $c$. 
  * However, the converse (opposite) is not true (see below)
* Theorem: If  $f$ is differentiable at $x$, then $x$ is continuous at $x$
  * $f$ is continuous at $x$ if $\lim_{x\to y}f(y)=f(x)$. Equivalently, $\lim_{h\to 0}f(x+h)=f(x)$. 
  * $\lim_{h\to 0}f(x+h)-f(x)=\lim_{h\to 0}(f(x+h)-f(x))=\lim_{h\to 0}(f(x+h)-f(x))\frac{h}{h}$
  * $=\lim_{h\to 0}\frac{f(x+h)-f(x)}{h}\cdot h=\lim_{h\to 0}\frac{f(x+h)-f(x)}{h}\cdot \lim_{h\to 0}h=f^\prime(x)\cdot 0=0$
* Differentiability rules: Let $f$ and $g$ be differentiable at $c$. 
  * Constants: If $h(x)=k$, $h^\prime(x)=0$ for all $x$
  * Identity: If $h(x)=x$, then $h^\prime(x)=1$ for all $x$
  * Sums/differences: $(f+g)^\prime(c)=f^\prime(c)+g^\prime(c)$ and $(f-g)^\prime(c)=f^\prime(c)-g^\prime(c)$
  * Product rule: $(f+g)^\prime(c)=f^\prime(c)g(c)+f(c)g^\prime(c)$
    * Proof: $(fg)^\prime=\lim_{h\to 0}\frac{f(c+h)g(c+h)-f(c)g(c)}{h}=\lim_{h\to 0}\frac{f(c+h)g(c+h)-f(c)g(c+h)+f(c)g(c+h)-f(c)g(c)}{h}$
    * $=\lim_{h\to 0}\frac{f(c+h)g(c+h)-f(c)g(c+h)}{h}+\lim_{h\to 0}\frac{f(c)g(c+h)-f(c)g(c)}{h}=$
    * $(\lim_{h\to 0}g(c+h))\lim_{h\to 0}\frac{f(c+h)-f(c)}{h}+(\lim_{h\to 0}f(c))\lim_{h\to 0}\frac{g(c+h)-g(c)}{h}$





