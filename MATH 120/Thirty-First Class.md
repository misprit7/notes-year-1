# Thirty-First Class
Oct 30, 2019
* Newton's method analysis
  * $f:\R\to\R$, $f(x)=x^2-2$
  * Suppose $f$ is twice differentiable on $\R$, and $f^{\prime\prime}$ is continuous. Let $c$ be a root of $f$, i.e. $f(c)=0$. Let $x_1$ be our first guess for $c$. Perform a Taylor expansion  (i.e. apply Taylor's theorem) around $x_1$. 
  * Reminder: Taylor's theorem for $n=2$
    * $c$: point around which we are doing expansion
    * $x$: point where we are evaluating $f$
    * $x_1$: point where the error in approximation is begin computed
    * $f(x)=f(c)+f^\prime(c)(x-c)+\frac{f^{\prime\prime}(x_1)}{2!}(x-c)^2$
  * $f(c)=0=f(x_1)+f^\prime(x_1)(c-x_1)+\frac{f^{\prime\prime}(y_1)}{2}(c-x_1)^2$
  * If $f^\prime(x_1)\neq0$, then we can divide and rearange to obtain:
  * $c-x_1+\underbrace{\frac{f(x_1)}{f^\prime(x_1)}}_{\Delta_1}=\frac{-f^{\prime\prime}(y_1)}{2f^\prime(x_1)}(c-x_1)^2$
  * Recall: we define $x_2=x_1-\Delta_1$, so it becomes:
  * $c-x_2=\frac{-f^{\prime\prime}(y_1)}{2f^\prime(x_1)}(c-x_1)^2$, so
  * $|c-x_2|=\frac{|f^{\prime\prime}(y_1)|}{2|f^\prime(x_1)|}|c-x_1|^2$
  * Returning to our example of $f(x)=x^2-2$:
    * $f^\prime(x)=x^2$
    * $f^{\prime\prime}(x)=2$
    * So, if $1\leq x\leq2$, then $f^\prime(x)\geq 2$ and if $1\leq y\leq2$, then $|f^{\prime\prime}(y)|\leq 2$. 
    * If $x, y\in[1, 2]$, then $|\frac{f^{\prime\prime}(y_1)}{2f^\prime(x_1)}|\leq \frac{1}{2}$
    * Initial guess $x_1=1$. Thus $f(x_1)=1^2-2=-1<0$
    * $f(2)=2^2-2=2>0$, so $c\in(1, 2)$. Since $x_1, y_1\in(1, 2)$, we have $|x_2-c|\leq \frac{1}{2}|x_1-c|^2\leq \frac{1}{2}$
    * $x_2=\frac{3}{2}$, $f(x_2)>0$
    * We know $x_2, y_2\in[1, 2]$, so $|x_3-c|\leq\frac{1}{2}|x_2-c|^2\leq \frac{1}{2}\cdot (\frac{1}{2})^2=\frac{1}{8}$
    * $|x_4-c|\leq\frac{1}{2}|x_3-c|^2\leq \frac{1}{2}\cdot (\frac{1}{8})^2=\frac{1}{128}$
* Logarithms
  * Lets consider the function $\log_{10} x$
  * What is it's definition? 
    * $\log_{10}x=u$ if $10^u=x$
  * But how do we define $10^u$? 
    * If $u$ is an integer, it's easy
    * If $u$ is rational, say $u=\frac{p}{q}$, we define $10^u=(\sqrt[q]{10})^p$
  * We know:
    * $\log_{10}xy=\log_{10}x+\log_{10}y$
    * $10^{x+y}=10^x10^y$
    * We could also use a different base $b>1$
      * $\log_bx=u$ if $x=b^u$
    * Again $\log_{b}xy=\log_{b}x+\log_{b}y$
  * We will define the function $\log_b u$, and use this to define the function $b^x$
  * Suppose we have a function $f$ with the property $f(xy)=f(x)+f(y)$ whenever $x, y, x\cdot y\in D(f)$





