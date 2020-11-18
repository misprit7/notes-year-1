# Seventh Class
Sep 16, 2019
* Putnam exam
  * Practice sessions
  * Prof. Dragos Chioca
  * Meetings Tuesdays at 11a.m.
  * First meeting tommorw
  * In LSK 462
* Def: A function $f$ is called one-to-one or injective if whenever $x\neq y$, $f(x)\neq f(y)$. Equivalently, for all $x, y\in D(f)$, $x=y$ if and only if $f(x)=f(y)$
  * e.g. $f(x)=2x+1$ Is this one-to-one?
    * Yes
    * Proof: Let $x, y\in \mathbb{R}$, and suppose $f(x)=f(y)$. We need to prove that $x=y$. $f(x)=f(y)$ implies $2x+1=2y+1$. Subtracting $1$ from both sides, we get $2x=2y$. Dividing both sides by $2$, we conclude $x=y$. 
  * Horizontal line test
    * A function $f$ is one-to-one if and only if every horizontal line in the $xy$ plane intersects the graph of $f$ in at most one point
  * e.g. $f(x) = x^2+1, D=[0, \infty)$ Is this one-to-one
    * Yes
    * Proof: We will do a proof by contradiciton. Suppose $f$ is not one-to-one i.e. there exist real numbers $x, y\in D = [0, \infty)$ so that $x\neq y$, but $f(x)=f(y)$. Without loss of generality (wlog), we can assume that $x<y$. This implies that $x^2=x\cdot x \leq x\cdot y < y\cdot y = y^2$. This is because $x\in [0, \infty)$ implies $x\geq 0$. $y>x$ implies $y>0$, hence $xy<y^2$, and $xy\leq y^2$ follows from $x\geq 0$. Since $x^2 < y^2$, we have $x^2+1<y^2+1$, i.e. $f(x)< f(y)$, but this contradicts the assumption that $f(x)=f(y)$
* Def: A function $f: D\to S$ is called onto or surjective if $R(f)=S$ i.e. for every $y\in S$, there exists $x\in D$ such that $f(x)=y$
  * $\forall y\in S \exists x\in D$ s.t. $f(x)=y$
* If a function is both one-to-one and onto, we say it is "one-to-one and onto" or "bijective"
  * For every $y\in S$, there exists a unique $x\in D$ such that $f(x)=y$
    * $\forall y\in S, \exists !x\in D$ s.t. $f(x)=y$
    * e.g. $f(x) = 2x+1$ prove that $f$ is surjective/onto