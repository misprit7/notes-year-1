# Thirty-Seventh Class
Nov 13, 2019
* Last class, we proved that $\lim_{\theta\to0}\frac{\sin\theta}{\theta}$
  * Next, using the half angle formula $\cos\theta = 1-2(\sin(\theta/2))^2$, we have $\cos^\prime(0)=\lim_{h\to0}\frac{\cos(0+h)-\cos(0)}{h-0}=\lim_{h\to0}\frac{\cos(h)-1}{h}=\lim_{h\to0}(-1)\frac{2(\sin\frac{h}{2})^2}{h}=(-1)\lim_{h\to0}\frac{\sin(h/2)\sin(h/2)}{h/2}$
  * $=(-1)\lim_{h\to0}\frac{\sin(h/2)}{h/2}\cdot\lim_{h\to0}\sin(h/2)=(-1)(1)(0)=0$
* Theorem: The function $\sin(\theta)$ is differentiable, and $\sin^\prime(\theta)=\cos(\theta)$
  * Proof: $\sin^\prime(\theta)=\lim_{h\to0}\frac{\sin(\theta+h)-\sin(\theta)}{h}=\lim_{h\to0}\frac{\sin(\theta)\cos(h)-\cos(\theta)\sin(h)-\sin(\theta)}{h}=\lim_{h\to0}\frac{\sin(\theta)(\cos(h)-1)+\cos(\theta)\sin(h)}{h}$
  * $=\lim_{h\to0}\sin(\theta\frac{\cos(h)-1}{h}+\lim_{h\to0}\cos(\theta)\frac{\sin(h)}{h}=\cos(\theta)$
* Theorem: $\cos(\theta)$ is differentiable and $\cos^\prime(\theta)=-\sin(\theta)$
  * Proof: Recall that $\sin(\pi/2-\theta)=\cos(\theta)$ and $\cos(\pi/2-\theta)=\sin(\theta)$. So $\cos^\prime(\theta)=\frac{d}{d\theta}\cos(\theta)=\frac{d}{d\theta}\sin(\pi/2-\theta)=-\cos(\pi/2-\theta)=-\sin(\theta)$
* Let's apply Taylor's theorem to the functions $\sin(\theta)$ and $\cos(\theta)$ at the point $c=0$. 
$$
\sin(\theta)=\sin(0)+\sum_{k=1}^{n-1}\frac{\sin^{(k)}(0)}{k!}\theta^k+\frac{\sin^{(n)}(0)}{n!}\theta^n=0+\theta-0-\frac{\theta^3}{3!}+0+\frac{\theta_5}{5!}-\ldots+\underbrace{\frac{\sin^{(n)}(\theta_1)}{n!}\theta^n}_{\textrm{absolute value $\leq \theta^n/n$}}
$$
* In particular, if $-\pi\leq\theta\leq\pi$, then 
$$
  |\sin(\theta)-(\theta-\frac{\theta^3}{3!}+\frac{\theta_5}{5!}-\ldots)|\leq\pi^n/n!
$$
* What about $\cos(\theta)$?
$$
  \cos(\theta)=1-\frac{\theta^2}{2!}+\frac{\theta^4}{4!}-\frac{\theta^6}{6!}+\ldots +\frac{\cos^{(n)}(\theta_1)}{n!}\theta^n
$$
* Landav "big-O" notation
  * Definition: If $f$ and $g$ are functions, we say "$f(x)=O(g(x))$ as $x\to0$" if:
    * There is a number $t>0$ and a number $C>0$ so that $|f(x)|\leq C|g(x)|$ for all $x\in(-t, t)$
    * e.g. $f(x)=2x^2+3x^3+4x^4$
      * $f(x)=O(x^2)$ as $x\to0$
* Using big-O notation, $\sin(\theta)=\theta-\frac{\theta^3}{3!}+\frac{\theta_5}{5!}-\ldots+O(\theta^n)$ as $\theta\to 0$