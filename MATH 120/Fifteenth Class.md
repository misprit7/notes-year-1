# Fifteenth Class
Sep 30, 2019
* Announcements
  * Extra office hours
    * Monday 6-8p.m.
  * Midterm material up to and including friday sep 27
* Infinite limits
  * Let $f$ be a function and $a\in\R$. We say $\lim_{x\to a}f(x)=\infty$ if
    * $\exists t>0s.t.\{x\in\R: 0<|x-a|<t\}\subset D(f)$
    * $\forall M\in\R, \exists \delta s.t. \forall x\in\R with 0<|x-a|<\delta$, $f(x)>M$
    * e.g. $f(x)=\frac{1}{x^2}, \lim_{x\to 0}f(x)=\infty$
      * Since $D(f)=\R\setminus \{0\}$, any $t>0$ will work. In particular, $(-1 ,0)\cup (0, 1)\subset D(f)$. 
      * Next, let $M\in\R$. Select $\delta=\frac{1}{\sqrt{|M|+1}}$. Observe that $\delta\in\R$, $\delta>0$ and $\frac{1}{\delta^2}\geq M$. If $|x-a|=|x|<\delta$, then $f(x)=\frac{1}{x^2}=\frac{1}{|x|^2}>\frac{1}{\delta^2}>M$
    * e.g. $f(x)=\frac{1}{x}, \lim_{x\to 0}f(x)=\infty$
      * We define $\lim_{x\to a^+}f(x)=\infty$ or $\lim_{x\to a^-}f(x)=\infty$ in the obvious way. 
      * $\forall M\in\R, \exists \delta>0 s.t. \forall x\in\R with 0<|x-a|<\delta, f(x)> M$
* We say $\lim_{x\to \infty}f(x)=\infty$ if 
  * $\exists T\in\R s.t. (T, \infty)\subset D(f)$
  * $\forall M\in\R, \exists R\in\R s.t. \forall x\in\R with x>\R$, we have $f(x)>M$
* We can also define $\lim_{x\to\infty}f(x)=-\infty$, $\lim_{x\to-\infty}f(x)=-\infty$ and $\lim_{x\to-\infty}f(x)=\infty$in the obvious way
* Recall if $f$ is a function and $a\in\R$, if for $\forall L\in\R$, the statement $\lim_{x\to a}f(x)=L$ is false, the we say $\lim_{x\to a}f(x)$ does not exist as a real number
* If $f$ is a function, $a\in\R$, we say $\lim_{x\to a}f(x)$ does not exists if $\forall L\in\R$, $\lim_{x\to a}f(x)=L$ is false, and $\lim_{x\to a}f(x)=\infty$ is false and $\lim_{x\to a}f(x)=-\infty$ is false
* A polynomial is a function of the following form: $f(x)=a_n x^n+a_{n-1} x^{n-1} + \ldots + a_1 x +a_0$, $n\geq 0$, where $a_n, \ldots, a_0$ are real numbers and $a_n\neq 0$. We define the degree of $f$ to be $n$, we write this as $\deg(f)$. Additionally, we say that the function $f(x)=0$ is also a polynomial, and we define its degree to be $-1$




