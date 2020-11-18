# Thirty-Sixth Class
Nov 12, 2019
* Trigonometric functions
  * $\sin(\theta)$ is the $y$ cordinate of point of a unit circle $\theta$ radians around the circles
  * $\cos(\theta)$ is the $x$ cordinate of point of a unit circle $\theta$ radians around the circles
* Lemma: $\sin\theta$ is continuous
  * First, we will show that $\lim_{\theta\to0}\sin\theta=0$ and $\lim_{\theta\to0} \cos\theta=1$
    * Let $O$ be the origin, $A$ be $(1, 0)$ and $P$ be a point on the unit circle $\theta$ radians around the circles
    * Lenth of segment $AP\leq$ length of chord $AP$
    * $\sqrt{(\cos\theta-1)^2+(\sin\theta)^2}\leq\theta$
    * $(\cos\theta-1)^2+(\sin\theta)^2\leq\theta^2$
    * We conclude that $(\sin\theta)^2\leq\theta^2(1)$ and $(\cos\theta-1)^2\leq\theta^2(2)$ (this follows since $(\sin\theta)^2$ and $(\cos\theta-1)^2$ are not negative)
    * $(1)$ implies $|\sin\theta|\leq|\theta|$ and $(2)$ implies $|\cos\theta-1|\leq|\theta|$
    * Now use squeeze theorem (with functions$|\theta|, 0$)
  * Next let $\theta\in\R$, $h\in\R$. By the product rule, $\lim_{h\to0}\sin\theta\cos h=\sin\theta$ and $\lim_{h\to0}\sin h\cos\theta=0$
    * By the sum rule for limits, $\lim_{h\to0}\sin\theta\cos h+\sin h\cos\theta=\sin\theta$, i.e. $\lim_{h\to0}\sin(\theta+h)=\sin\theta$
    * We can also conclude $\cos\theta$ is continuous since $\cos\theta=\sin(\frac{\pi}{2}-\theta)$
* Lemma: $\lim_{\theta\to0}\frac{\sin\theta}{\theta}=1$
  * Proof: First, observe that $\frac{\sin\theta}{\theta}=\frac{\sin(-\theta)}{-\theta}$, so it suffices to prove that $\lim_{\theta\to0^+}\frac{\sin\theta}{\theta}=1$ (if we prove this, if follows that the left sided limit also equals $1$ and the regular limit exists as well)
  * Let $0<\theta<\frac{\pi}{2}$
  * Use the same definitions for $O, A$ and $T$ as above, and $T$ is the point $(1, \tan\theta)$
  * The area of the circular sector $OAP$ is larger than the area of the triangle $OAP$ and smaller than the area of the triangle $OAT$. 
  * Triangle Area of $\Delta OAP\leq$ area of sector $OAP\leq$ area $\Delta OAT$
  * $\frac{1}{2}\cdot \sin\theta\leq\frac{\theta}{2}\leq \frac{1}{2}\frac{sin\theta}{\cos{\theta}}$
  * $1\leq\frac{\theta}{\sin{\theta}}\leq \frac{1}{\cos\theta}$
  * $1\geq \frac{\sin\theta}{\theta}\leq \cos\theta$
  * Use squeeze theorem