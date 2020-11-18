# Thirty-Eighth Class
Nov 15, 2019
* We defined last class $f(x)=O(g(x))$ as $x\to0$
  * e.g. $f(x)=\begin{cases}1, x\in\mathbb{Q}\\ 0, x\in\R\setminus\mathbb{Q}\end{cases}$
    * $f(x)=O(1)$ as $x\to0$
    * i.e. $\exists t>0, C>0$ so that for all $x\in\R$ with $|x|<t$, $|f(x)|\leq C|g(x)|$
* $\sin(x)=O(x)$ as $x\to0$
* Definition: We say $f(x)=O(g(x))$ as $x\to\infty$ if there exists a number $R\in\R$ and $C>0$ so that $|f(x)|\leq C|g(x)|$ for all $x>R$
  * e.b. $\sin(x)=O(1)$ as $x\to\infty$
  * e.g. $f(x)=2x^3+3x^2+4=O(x^3)$ as $x\to\infty$
* Last time: $|\sin(\theta)-(\theta-\frac{\theta^3}{3!}+\frac{\theta^5}{5!}-\ldots)|\leq\frac{|\theta|^n}{n!}$
  * Same as $|\sin(\theta)-\sum_{k=1\textnormal{, k odd}}^{n-1}(-1)^{\frac{k-1}{2}}\frac{\theta^k}{k!}|\leq\frac{|\theta|^n}{n!}$
  * How to turn this into a practical algorithm?
    * Let $N=\lfloor\frac{\theta}{2\pi}\rfloor$ ($\lfloor n\rfloor$ represent the floor of $n$)
    * Let $\theta^\prime=\theta-2\pi N$. $\sin(\theta^\prime)=\sin(\theta)$
    * $0\leq\theta^\prime<2\pi$
    * Next, compute $\sin(\theta^\prime)$. Say we want to compute it up to accuracy $\epsilon$. How large does $n$ need to be? 
    * Choose $n$ large enought that $(2\pi)^n<\epsilon n! (1)$
* Stirling's formula/Stirling's approximation
  * $n!\approx\sqrt{2\pi n}(\frac{n}{e})^n$
  * More precisely, $\sqrt{2\pi}\frac{n^{(n+1)/2}}{e^n}\leq n!\leq \frac{n^{(n+1)/2}}{e^{n-1}}$
  * To solve $(1)$, it suffices to solve $\epsilon\leq \frac{(2\pi)^n}{n!}\leq(\frac{(2\pi e)}{n})^n$
    * Define $f(x)=(\frac{(2\pi e)}{x})^x-\epsilon$
    * Use Newton iteration to find a solution