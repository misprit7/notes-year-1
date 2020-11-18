# Twenty-Seventh Class
Oct 23, 2019
* Newtons method: Let $f$ be a function with $D(f)=\R$ and suppose $f$ is differentiable at every point $x\in\R$. We want to find a solution to $f(x)=0$ (if $f(x)=0$, then $x$ is called a root of $f$). 
  * According to Zahl, the "most applicable thing we'll learn in this class"
  * Idea: Start with a guess $x_1\in\R$. If $f^\prime>0$, then $f$ is increasing near $x_1$, so if $f(x_1)<0$, we should increase our guess for $x$, while if $f(x_1)>0$, we should decrease our guess for $x$. If $f^\prime(x)<0$, then we do the opposite. 
  * Question: By how much should we increase or decrease our guess $x_1$? 
    * If $f$ was linear, i.e. $f(x)=ax+b$, then we do know the answer: we add $\frac{-f(x_1)}{a}=\frac{-f(x_1)}{f^\prime(x)}$ to $x$. We could define $\Delta_1=\frac{f(x_1)}{f^\prime(x)}=$, and $x_2=x_1-\Delta_1$
    * This approach can be used more broadly, even if it won't give the exact answer after the first iteration
  * Let's use Newton's method to approximate $\sqrt2$, i.e. find the positive root of $f(x)=x^2-2$
    * We will begin with the guess $x_1=1$
    * $f(x)=-1$, $f^\prime(1)=2$, $\Delta_1=\frac{f(x_1)}{f^\prime(x_1))}=-\frac{1}{2}$
    * $x_2=x_1-\Delta_1=1-(-\frac{1}{2})=\frac{3}{2}$
    * $f(x_2)=(\frac{3}{2})^2-2=\frac{1}{4}$, $f^\prime(x_2)=3$, $\Delta2=\frac{f(x_2)}{f^\prime(x_2)}=\frac{1}{12}$
    * $x_3=x_2-\Delta_2=\frac{3}{2}-\frac{1}{12}=\frac{17}{12}$
    * $f(x_3)=\frac{289}{144}-2=\frac{1}{144}$, $f^\prime(x)=\frac{17}{6}, \Delta_3=\frac{\frac{1}{144}}{\frac{17}{6}}=\frac{1}{408}$
    * $x_4=x_3-\Delta_3=\frac{17}{2}-\frac{1}{408}=\frac{577}{408}\approx1.41422\ldots$
    * Correct answer: $\sqrt2=1.41421\ldots$
  * Be careful: Newton's method doesn't always work
    * e.g. $f(x)=x^3-2x+2$
      * Start with guess $x_1=0, f(x_1)=2, f^\prime(x_1)=-2, \Delta_1=\frac{f(x_1)}{f^\prime(x_1)}=-1$
      * $x_2=1, f(x_2)=1, f^\prime_2)=1, \Delta_2=\frac{f(x_2)}{f^\prime(x_2)}=1$
      * $x_3=x_2-\Delta_2=0=x_1$
      * Just keeps on looping forever
  * Later, we will find sufficient conditions to ensure that Newton's method will work
    * We need Taylor's theorem to do so