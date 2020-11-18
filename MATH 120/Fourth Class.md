# Fourth Class 
Sep 10, 2019
* Importance of the least upper bound property
  * If it didn't exist, $f(x) = x^2-2$ wouldn't have any zeros having negative and positive output values
* Useful facts about real numbers that are allowed to be used
  * The product of two positive numbers is positive
  * The product of two negative numbers is positive
  * The product of a negative and positive number is negative
  * Basic facts about inequalities
    * E.g. Multiplying a positive number with a number smaller than one makes it smaller
* Proof by contradiction
  * Goal is to prove mathematical statement $S$
  * Step 1: Suppose that this statement is false
  * Step 2: Using the assumption that the statement is false and any other correct logical deductions or mathematical statements that are useful, arrive at a conclusion that is clearly false 
    * e.g. $1=0$, $2<2$, etc. 
  * Step 3: Conclude that the original statement is true
  * Example: Let $S = \{x\in \mathbb{Q}: x>0 \textnormal{ and } x^2 < 2\}$. $S$ is bounded aboe. Indeed, if $y\in \mathbb{Q}$ and $y^2>2, y>0$, then $y$ is an upper bound for $S$. 
    * Suppose the statement is false, i.e. there exists a number $y\in \mathbb{Q}$ such that $y>0, y^2>2$ and there iexists a number $x\in S$ with $x>y$. In other words, $y$ is not an upper bound for $S$. 
    * Since $x>y$ and both are positive, $2>x^2=x\cdot x>xy>y\cdot y>y^2>2$. 
    * We conclude $2>2$, so the original assumption must be false and $y$ must always be an upper bound for $S$. \qed (in latex)
* We can think of real numbers as points on a number line
  * $S = \{1, 2, 7, 8\}$ can be thought of a subset of points on the number line
  * An open interval is a subset of the real numbers in one of the following forms: 
    * $\{x\in \mathbb{R}: x>a \textnormal{ and } x <b\}$, where $a, b\in \mathbb{R}$ with $a<b$
      * $\{x\in \mathbb{R}: a<x<b\}$
      * $(a, b)$
      * This is called a finite length open interval. It has length $b-a$
    * $\{x\in \mathbb{R}: x>a\}$, where $a\in \mathbb{R}$
      * $(a, \infty)$
    * $\{x\in \mathbb{R}: x<b\}$, where $b\in \mathbb{R}$
      * $(-\infty , b)$
    * $\{x\in \mathbb{R}\}$
      * $(-\infty , \infty)$
  * Which of the following subsets of $\mathbb{R}$ areopen intervals? 
    * $(1, 2)\cup (2, 3)$
      * No, since it doesn't include $2$
    * $(1, 2)\cup (2, 3) \cup \{2\}$
      * Yes
    * $(1, 2)\cup (1, 3)$
      * Yes
    * $(-1, 1)\cup (-2, 2)\cup (-3, 3)\cup ...$
      * Yes, it's the set of all real numbers
  * 




