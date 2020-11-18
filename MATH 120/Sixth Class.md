# Sixth Class
Sep 13, 2019
* The domain convention
  * If the domain of a functions isn't specified, we assume the domain is the largest subset of the real numbers for which $f(x)$ "makes sense" as a real number
    * Not well defined in the complex plane
  * We write this as $D(f)$ (the domain of $f$) or $D$, if $f$ is obvious from context
    * e.g. $f(x) = x^2+2, D(f)=\mathbb{R}$
    * e.g. $f(x)=\log{(x)}, D(f)=(0, \infty)$
    * e.g. $f(x)=\log{|x|}, D(f)=(-\infty, 0)\cup (0, \infty)$ or $\{x\in \mathbb{r}: x\neq 0\}$ or $\mathbb{R}\backslash \{0\}$
    * e.g. $f(x) = \frac{1}{x^2}, D(f)=\mathbb{R}\backslash \{0\}$
* Def: if $f$ is a function, the graph of $f$ is the set of ordered pairs $\{x, f(x): x\in D(f)\}$. This is a subset of the $xy$ plane $\{(x, y): x, y\in \mathbb{R}\}=\mathbb{R}^2$
  * $\{(x, y): x\in D(f), y=f(x)\}$
  * $\{(x, y)\in \mathbb{R}^2: x\in D(f), y=f(x)\}$
  * $\mathbb{R}$ represents the cartesian $xy$ plane
  * We can draw the graphs of the functions from our previous examples
    * i.e. $f(x)=x$
    * i.e. $f(x)=\sin{x}$
    * i.e. $f(x)=\log{|x|}$
* Is i true that for every curve, or more generally any for any subset of the plane, there is a function whose graph is that set
  * No
* Vertical line test
  * a subset $T\subset \mathbb{R}^2$ is the graph of a function if and only if every vertical line in the $xy$ plane ($\mathbb{R}^2$) intersects $T$ at most once
    * If and only if can be written as iff
    * $A$ if and only if $B$ is equal to $A\iff B$
* Piecewise notation
  * $f(x)=\{x, \textnormal{ if } x\geq 0; -x, \textnormal{ if } x<x\}=|x|$
  * Filled dot represents closed interval, while open dot implies open interval
  * $f(x)=\{1, x\in\mathbb{Q}; 0, x\notin \mathbb{Q}\}$
* Def: If $f$ is a function, the range of $f$ is the set $\{f(x): x\in D(f)\}$. We write this as $R(f)$
  * e.g. $f(x)=x$
    * $D(f)=\mathbb{R}$
    * $R(f)=\mathbb{R}$
  * e.g. f(x) = \sin{x}
    * $D(f)=\mathbb{R}$
    * $R(f)=[-1, 1]$
  * e.g. $f(x) = \{1, x\in\mathbb{Q}; 0, x\notin \mathbb{Q}\}$
    * $D(f)=\mathbb{R}$
    * $R(f)=\{0, 1\}$




