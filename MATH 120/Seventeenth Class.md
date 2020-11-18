# Seventeenth Class
Oct 4, 2019
(continuation of last class's proof)
* Lets prove $\lim_{x\to\infty}\frac{P}{Q}(x)=0$ if $\deg P<\deg Q$. 
  * First, we will verify the domain requirement. $D(P/Q)=\{x\in\R: Q(x)\neq0\}$. We want to find $T\in\R$ so that $(T, \infty)\subset D(P/Q)$, i.e. $Q(x)\neq 0$ for all $x>T$. Let $B=|B_{m-1}|+\ldots +|b_0|$. Then $b_mx^m-Bx^{m-1}\leq Q(x)\leq b_mx^m+Bx^{m-1}$. So, if $x>\frac{B}{|b_m|}$, then $Q(x)\neq 0$. 
  * $T=\frac{B}{b_m}$, and the domain requirement is met. 
  * Next, let $\epsilon>0$. We need to find $R\in\R$, so that for all $x>R$, $|\frac{P(x)}{Q(x)}|<\epsilon$
  * Select $R=\max(1, 2B/|b_m|, \frac{2C}{|b_m|\epsilon})$. Then, $|\frac{P}{Q}|<\frac{Cx^n}{\frac{1}{2}|b_m|x^m}=\frac{2C}{|b_m|}\frac{1}{x^{m-n}}\leq \frac{2C}{|b_m|}\frac{1}{x}<\frac{2C}{|b_m|}\frac{1}{R}\leq\epsilon$
    * Scratch
      * $|\frac{P(x)}{Q(x)}|=\frac{|P|}{|Q|}$ (I'm using $P=P(x)$ from now on, not in the original)
      * Let $C=|a_n|+\ldots +|a_0|$. Then $|P|\leq Cx^n$ (using the same argument for all of our other inequalities)
      * If $x>T$, then $|Q(x)|\geq |b_m|x^m-Bx^{m-1}=(|b_m|x-B)x^{m-1}$. If $x>2B/|b_m|$, then $|Q(x)|\geq \frac{1}{2}|b_m|x^m$ (just algebra)
        * Triangle inequality also states that $|a+b|\geq |a|-|b|$ and $|a-b|\geq |a|-|b|$
* Back to b. First, $\lim_{x\to\infty}\frac{a_n}{b_n}=\frac{a_n}{b_n}$. Next, $\frac{P}{Q}-\frac{a_n}{b_n}=\frac{b_nP-a_nQ}{b_nQ}\frac{P(x)b_n-a_nQ(x)}{Q(x)b_n}=\frac{(a_nx^n+\ldots a_0)b_n-a_n(b_nx^n+\ldots b_0)}{b_n(b_nx^n+\ldots b_0)}=\frac{a_{n-1}b_n-anb_{n-1}x^{n-1}+\ldots a_0b_n-a_0b_n}{b_n\cdot b_nx^n+\ldots b_n\cdot b_0)}$ $=\frac{S(x)}{b_nQ}$. Now, $\deg S < \deg Q$, so $\lim_{x\to\infty}\frac{P}{Q}-\frac{a_n}{b_n}=\lim_{x\to\infty}\frac{S}{b_nQ}$. Therefore, $\lim_{x\to\infty}\frac{P}{Q}=\lim_{x\to\infty}\frac{P}{Q}-\frac{a_n}{b_n}+\frac{a_n}{b_n}=\frac{a_n}{b_n}$