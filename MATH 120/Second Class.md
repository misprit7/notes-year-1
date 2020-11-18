# Second Class
Sep 6, 2019
* Some more definitions: 
  * If $S$ and $T$ are sets, their union is also a set consisting of all elements that are elements of $S$ or are elements in $T$ or both
    * We write this as $S \cup T$
    * Different notation: $S \cup T = \{x: x \in S \textnormal{ or } x \in T (\textnormal{or both})\}$
    * eg. $S = \{1, 2, 3\}, S \cup \mathbb{N} = \mathbb{N}$
  * If S and T are sets, the intersection of $S$ and $T$ is the set consisting of all elements that are in $S$ and in $T$
    * We write this as $S\cap T = \{x: x \in S \textnormal{ and } x \in T\}$
  * If $S$ and $T$ are sets and every element of $S$ is also an element of $T$, then we say $T$ contains $S$ and we write this as $S \subset T$. 
    * eg. $\{1, 2, 3\}\subset \mathbb{N}$
    * If $S = T$, $S \subset T$ and $S \supset T$
  * If $S$ and $T$ are sets, we define $S\setminus T = \{x: x\in S \textnormal{ and } x \notin T\}$
    * The same as $\{x \in S: x \notin T\}$
    * Set subtraction
  * Exclusive or
    * $(S\setminus T)\cup (T\setminus S) = \{x: x \in S \textnormal{ or } x \in T, \textnormal{ but not both}\}$
    * $(S \cup T)\setminus (S\cap T)$ is written as $S \triangle T$
* Defining the real numbers
  * The real numbers $\mathbb{R}$ is the set of all decimal expansion, i.e. 10.20000000... or 0.111111... or 3.1415...
    * Problem: is $1.000\ldots = 0.999\ldots$? 
  * Too complicated to define fully in this class
* Properties of real numbers
  * Rather than define the real numbers, we will describe some of their properties
    * $\mathbb{R}$ is a set
    * It contains the rational numbers, i.e. $\mathbb{Q} \subset \mathbb{R}$
    * Real numbers can be added and subtracted, i.e. if $x, y \in \mathbb{R}, x+y \in \mathbb{R}, x-y \in \mathbb{R}$
    * Real numbers can be multiplied and divided, i.e if $x, y \in \mathbb{R}, x\times y \in \mathbb{R}$ and $\frac{x}{y} \in \mathbb{R}$
    * Real numbers are ordered, i.e. if $x, y \in \mathbb{R}$, then exactly one of the following three things is true
      * $x<y$
      * $x>y$
      * $x=y$
    * The real numbers satisfy the least upper bound property
      * If $S$ is a set of real numbers i.e. $S \subset \mathbb{R}$, a number $x\in \mathbb{R}$ is called an upper bound for $S$ if for every $y\in S$, we have $y\leq x$
        * e.g. $S = \{1, 2, 3, 6\}$, least upper bound is $6$








