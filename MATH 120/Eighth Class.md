# Eighth Class
Sep 17, 2019
* If $f$ and $g$ are functions with odmains $D(f)$ and $D(g)$, we then can define the functions $f+g$, $f-g$, and $f\cdot g$ in the obvious way
  * The domain of each of these new functions is $D(f)\cap D(g)$
  * e.g. $f(x)=x^2; g(x)=\frac{1}{x}$
    * $f\cdot g(x)=x$, with domain $D=\mathbb{R}\setminus \{0\}$ or $f\cdot g(x)=\{x, x\neq 0; \textnormal{undefined}, x=0\}$ or $f\cdot g(x)=x$ for all $x\neq 0$
* We can also define $(f/g)(x)=\frac{f(x)}{g(x)}$
  * $D(f/g)=(D(f)\cap D(g)) \setminus \{x\in D(g): g(x)=0\}$
    * or $\{x\in D(f)\cap D(g): g(x)\neq 0\}$
* Compostion of functions
  * If $f$ and $g$ are functions, we can define the composition $f\circ g(x)=f(g(x))$, i.e. first apply $g$, then $f$
    * $D(f\circ g)=\{x\in D(g): g(x)\in D(f)\}$
    * e.g. $g(x) = \frac{1}{x}; f(x)=\frac{1}{x}$
      * $f\circ g(x)=x$, if $x\neq 0$
* Def: Let $f$ be a function, let $a\in \mathbb{R}$ and $L\in \mathbb{R}$. We say $\lim_{x\to a} f(x) = L$ is true if the following two criteria hold: 
  * There exists a number $t>0$ so that $\{x\in \mathbb{R}: 0<|x-a|<t\}\subset D(f)$
    * Essentially means that the function exists for some finite amount around $a$
    * If the domain of a function was the rationals, then there would be infinite gaps such that a limit can't exist
    * Called the domain requirement
  * For every real number $\epsilon>0$, there exists a real number $\delta>0$ so that the following is true: For every real number $x$ satisfying the inequality $0<|x-a|<\delta$, we have $|f(x)-L|<\epsilon$
    * Equivialently, $\forall \epsilon>0 \exists\delta>0$ s.t. $\forall x\in\mathbb{R}: 0<|x-a|<\delta$, we have $|f(x)-L|<\epsilon$
  * e.g. 1: $f(x)=x$
    * $D(f)=\mathbb{R}$
    * $a=0, L=0$
    * $\lim_{x\to 0}f(x)=0$
  * e.g. 2: $f(x) = 2x$
    * $D(f) = \mathbb{R}$
    * $a=3, L=0$
    * We will prove $\lim_{x\to 3} f(x) = 6$
      * Step 1: Find a $t>0$ so that $\{x\in \mathbb{R}: 0<|x-3|<t\}\subset D(f)$
        * Any $t>0$ value works, e.g. $t=1$
      * Step 2: Let $\epsilon >0$. Set $\delta = \epsilon/2$. Let $x\in\mathbb{R}$ with $0<|x-3|<\delta$. Then $|2x-6|=|2(x-3)|=2|x-3|<2\delta=\epsilon$
















