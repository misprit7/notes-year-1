# Eleventh Class
Sep 23, 2019
* Limit rules
  * If $F(x)=k$ for alll $x\in\mathbb{R}$, then for every $a\in\mathbb{R}$, $\lim_{x\to a}f(x)=k$. We write this as $\lim_{x\to a}k=k$
  * If $f(x)=x$ for all $x\in\mathbb{R}$, the for every real number $a$, $\lim_{x\to a}f(x)=x$. We write this as $\lim_{x\to a}x=a$
    * Proof: Domain requirement is met
    * Let $a\in\mathbb{R}$
    * Let $\epsilon>0$. 
    * Choose $\delta=\frac{\epsilon}{2}$
    * Let $x\in\mathbb{R}$ with $0<|x-a|<\delta$. 
    * Then $|f(x)-L|=|x-a|<\delta=\epsilon/2<\epsilon$
  * Let $a\in\mathbb{R}$. If $\lim_{x\to a}f(x)=L$, and $\lim_{x\to a}g(x)=M$, then $\lim_{x\to a}(f+g)(x)=L+M$
    * Proof: Let $a$ be a real number, let $f$ and $g$ be functions, and suppose that $\lim_{x\to a}f(x)=L$ and $\lim_{x\to a}g(x)=M$. We will prove that $\lim_{x\to a}(f+g)(x)=L+M$. 
    * Domain requirement
      * Since $\lim_{x\to a}f(x)=L$, the domain requirement is met, thus there exists$t_1>0$ such that $\{x\in\mathbb{R}:0<|x-a|<t_1\}\subset D(f)$. In this same way, there exists a $t_2>0$ for $\lim_{x\to a}g(x)=M$ that fulfills the domain requirement. Hence, if we define $t=\textnormal{min}(t_1, t_2)$, then $t>0$ and $\{x\in\mathbb{R}:0<|x-a|<t_1\}\subset D(f)$ and $\{x\in\mathbb{R}:0<|x-a|<t_1\}\subset D(g)$. Therefore, $\{x\in\mathbb{R}:0<|x-a|<t_1\}\subset D(f)\cap D(g)=D(f+g)$
      * Let $\epsilon>0$. Define $\epsilon_1=\epsilon/2$ and $\epsilon_2=\epsilon/2$. Since we know that $\lim_{x\to a}f(x)=L$, there exists a number $\delta_1$ such that whenever $0<|x-a|<\delta_1$, we have $|f(x)-L|<\epsilon_1$. Similarily, since we know that $\lim_{x\to a}g(x)=M$, there exists a number $\delta_2$ such that whenever $0<|x-a|<\delta_2$, we have $|g(x)-M|<\epsilon_2$. Let $\delta=\textnormal{min}(\delta_1, \delta_2). Then \delta>0$. Observe that if $x$ is a real number with $0<|x-a|<\delta$, then $|f(x)-L|<\epsilon=\epsilon/2$ and $|g(x)-M|<\epsilon_2=\epsilon/2$. Hence, $|(f+g)(x)-(L+M)|=|(f(x)-L)+(G(x)-M)|\leq|f(x)-L|+|g(x)-M|<\epsilon/2+\epsilon/2=\epsilon$
  * If $\lim_{x\to a}f(x)=L$, and $\lim_{x\to a}g(x)=M$, then $\lim_{x\to a}(f-g)(x)=L-M$
  * If $\lim_{x\to a}f(x)=L$, and $\lim_{x\to a}g(x)=M$, then $\lim_{x\to a}(f\cdot g)(x)=L\cdot M$
  * If $\lim_{x\to a}f(x)=L$, and $\lim_{x\to a}g(x)=M\neq0$, then $\lim_{x\to a}(\frac{f}{g})(x)=\frac{L}{M}$