# Third Class
Sep 9, 2019
* The least upper bound property
  * Def: If $S \subset \mathbb{R}$, then a real number $x\in \mathbb{R}$ is called an upper bound for $S$ if: 
  * "for all $y\in S$, we have $y \leq x$"
  * Same as above: "$\forall y\in S, y \leq x$"
    * Ex. $S = \{1, 2, 3, 4, 5\}, T = \{x\in \mathbb{R}: x<0\}, U = \{x\in \mathbb{Z}: x \geq 12\}$
    * Let's prove that for every $x\in T$, there exists a number $y\in T$ with $y>x$. 
    * Conclusion: If $x\in T$, then x is not an upper bound for $T$. 
    * Proof:

Let $y=\frac{x}{2}$. 
We need to show two things: 
1) $y\in T$
Since $\frac{1}{2}$ is positive, $y=x/2 = \frac{1}{2}\cdot x$ has the same sign as x. 
since $x<0$, we conclude $y<0$. Hence $y\in T$
2) $y>2$
Since $x<0$ and $0<\frac{1}{2} < 1$, we have $y=x/2>x$
* Some sets $S\subset \mathbb{R}$ have an upper bound; some do not. 
  * Def: If $S\subset \mathbb{R}$ has an upper bound, we say it is bounded above
    * Otherwise it is not bounded above
  * Def: Let $S\subset \mathbb{R}$. A number $x\in \mathbb{R}$ is called a least upper bound for $S$ if $x$ is an upper bound for $S$ and if $z\in \mathbb{R}$ and $z<x$, then $z$ is not an upper bound for $S$
  * Def of least upper bound property: If $S\in \mathbb{R}$ and $S$ is bounded above, then $S$ has a least upper bound. 
* Let $S = \{x\in \mathbb{Q}: x>0 \textnormal{ and } x^2 < 2\}$. We will show:
  * The set $S$ is bounded above. Indeed, if $x\in \mathbb{Q}$ and $x^2 > 2, x>0$, then $x$ is an upper bound for $S$
    * Let $x\in \mathbb{Q}$ with $x>0$ and $x^2>2$
    * Let $y\in S$. We need to show that $y\leq x$. If $y\in S$, then $y^2 < 2$ and $y>0$. If $x^2>2$ and $y^2<2$ and both are positive, then $y<x$
  * If $x\in \mathbb{Q}$ is an upper bound for $S$, then there exists $z\in \mathbb{Q}$ with $z<x$, and $z$ is also an upper bound for $S$
