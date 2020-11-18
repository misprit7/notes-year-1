# Thirtieth Class
Oct 29, 2019
* Summation notation
  * $\sum_{k=1}^{n-1}$
    * $k$ is the indexing variable
    * $1$ is the starting value
    * $n-1$ is the ending value
  * e.g. $\sum_{k=1}^{10}k=55$
  * $\sum_{i=1}^ni-\frac{n(n+1)}{2}$
    * Proof: we will prove this by induction on $n$
    * Base case: $\sum_{i=1}^1i=1=\frac{1(1+1)}{2}$
    * Induction step: Suppose $\sum_{i=1}^ni=\frac{n(n+1)}{2}$. Now $\sum_{i=1}^{n+1}i=\sum_{i=1}^ni+n+1=\frac{n(n+1)}{2}+\frac{2(n+1)}{2}$
    * $=\frac{(n+1)((n+1)+1)}{2}$
* Taylor's Theorem
  * Let $f:[a, b]\to\R$, suppose $f$ is $n$-times differentiable on $[a, b]$ and $f^{(n)}$ is continuous on $[a, b]$. Let $c\in[a, b]$. Then, for every $x\in[a, b]$ with $x\neq c$, there is a point $x_1$ in the open interval between $x$ and $c$ so that
$$
f(x)=\sum_{k=0}^{n-1}\frac{f^{(k)}(c)}{k!}(x-c)^k+\frac{f^{(n)}(x_1)}{n!}(x-c)^n
$$
* Proof of Taylor's theorem
  * Let's assume that $c<b$ (if $c=b$, a similar argument works). Lets aslso assume that $x<c$ ( if $x<c$, some signs get flipped). Define $F(t)=f(t)+\sum_{k=1}^{n-1}\frac{f^{(k)}(t)}{k!}(x-t)^k$ for all $t\in[c, x]$. Define $G(t)=(t-c)^n+\sum_{k=1}^{n-1}(x-t)^k(t-c)^{n-k}$
  * Both $F$ and $G$ are continuous on $[c, x]$ and differntiable on $(c, x)$, so we can apply the generalized mean value theorem. We conclude there exists a point $x_1\in(c, x)$ so that 
  * $F^\prime(x_1)(g(x)-g(c))=G^\prime(x_1)(F(x)-F(c))$ ( * )
  * Now, $G(x)=(x-c)^n$ and $F(x)=f(t)$. So ( * ) becomes $F^\prime(x_1)((x-c)^n-g(c))=G^\prime(x_1)(f(x)-F(c))$
  * Let's compute $F(t)$: $F^\prime(t)=f^\prime(t)+\sum_{k=1}^{n-1}(\frac{f^{(k)}(t)}{k!}(x-t)^k)^\prime=f^\prime(t)+\sum_{k=1}^{n-1}\frac{f^{(k+1)}(t)}{k!}(x-t)^k+\frac{f^{(k)}(t)}{k!}(-k)(x-t)^{k-1}$
  * $=f^\prime(t)+\sum_{k=1}^{n-1}\frac{f^{(k+1)}(t)}{k!}(x-t)^k-\frac{f^{(k)}(t)}{(k-1)!}(x-t)^{k-1}$. When you write it out, it becomes a telescoping sum and all the terms cancel out (I'm too lazy to actually write it out). Thus $F^\prime(t)=\frac{f^{(n)}(t)(x-t)^{n-1}}{(n-1)!}$
  * Hence $F^\prime(x_1)=\frac{f^{(n)}(x_1)(x-x_1)^{n-1}}{(n-1)!}$. A similar computation (exercise) shows that $G^\prime(t)=n(x-t)^{n-1}$. Thus $\frac{f^{(n)}(x_1)}{(n-1)!}(x-x_1)^{n-1}((x-c)^n-0)=n(x-x_1)^{n-1}(f(x)-f(c)-\sum_{k=1}^{n-1}\frac{f^{(k)}(c)}{k!}(x-c)^k)$. We get
  * $\frac{f^{(n)}(x_1)}{n!}(x-c)^n=f(x)-f(c)-\sum_{k=1}^{n-1}\frac{f^{(k)}(c)}{k!}(x-c)^k$. Rearranging, we get Taylor's theorem. 