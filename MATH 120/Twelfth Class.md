# Twelfth Class
Sep 24, 2019
* If $\lim_{x\to a}f(x)=L$, and $\lim_{x\to a}g(x)=M$, then $\lim_{x\to a}(f\cdot g)(x)=L\cdot M$
  * Proof: The domain requirement is met, as it's the same proof as for the sum rule. Next, let $\epsilon>0$. Choose $\epsilon_1=\textrm{min}(\sqrt{\epsilon/3}, \frac{\epsilon}{3|M|+1})$ and $\epsilon=\textrm{min}(\sqrt{\epsilon/3}, \frac{\epsilon}{3|L|+1})$. With this choice, we have $\epsilon_1<\sqrt{\epsilon/3}$, and if $M\neq 0$, then $\epsilon_1<\frac{\epsilon}{3|M|+1}$ and $\epsilon_2<\sqrt{\epsilon/3}$, and if $L\neq 0$, then $\epsilon_2<\frac{\epsilon}{3|L|+1}$
  * Since $\lim_{x\to a}f(x)=L$, there exists $\delta_1$ such that for all real numbers $x$ with $0<|x-a|<\delta_1$, we have $|f(x)-L|<\epsilon_1$. The same is true for $\lim_{x\to a}g(x)=M$. 
  * Let $\delta=min(\delta_1, \delta_2)$. Then for all $x\in\mathbb{R}$ with $0<|x-a|<\delta$, we have $|f(x)-L|<\epsilon_1$, so
    * (1) $|f(x)-L|<\sqrt{\epsilon/3}$
    * (2) $|f(x)-L)M|<\epsilon/3$
  * $|g(x)-M|<\epsilon_2$, so
    * (1) $|g(x)-M|<\sqrt{\epsilon/3}$
    * (2) $|g(x)-M)L|<\epsilon/3$
  * Finally, $|f(x)-LM|\leq|(f(x)-L)(g(x)-M)|+|(f(x)-L)M|+|(g(x)-M)L|\leq |\sqrt{\epsilon/3}\cdot \sqrt{\epsilon/3} +\epsilon/3+\epsilon/3=\epsilon$
    * $f(x)g\cdot g(x)-LM=\underbrace{|(f(x)-L)(g(x)-M)|}_{<\epsilon/3}+\underbrace{|(f(x)-L)M|}_{<\epsilon/3}+\underbrace{|(g(x)-M)L|}_{<\epsilon/3}$
      * We want all three of the above terms to be smaller than $\epsilon/3$
* "Reciprical" rule: If $\lim_{x\to a}g(x)=M$ and $M\neq 0$, the $\lim_{x\to a}\frac{1}{g(x)}=\frac{1}{M}$
  * Proof: FIrst, we have to check the domain requirement. let $\epsilon_1=|M|$. Since $\lim_{x\to a}g(x)=M$, there exists $\delta>0$ such that $\forall x\in\mathbb{R}$ with $0<|x-a|<\delta_1$, we have $|g(x)-M|<\epsilon_1=|M|$. In particular, $g(x)neq 0$ (since if $g(x)=0$ then $|g(x)-M|=|M|$, but this isn't allowed). Let $t=\delta_1$. Then the set $\{x\in\mathbb{R}: 0<|x-a|<t\}\subset D(\frac{1}{g})$. In particular, the domain requirement is met. 
  * Scratch work
    * $|\frac{1}{g(x)}-\frac{1}{M}|=|\frac{M-g(x)}{g(x)M}|\geq \frac{g(x)}{(M/2)M}$