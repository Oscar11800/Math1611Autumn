***<h1 style="text-align: center;">Script 3</h1>***
**Lemma 3.4: If $A$ is a nonempty, finite subset of a continuum $C$, then $A$ has a first and last point.**
We can prove that $A$ has a first and last point through induction.

Suppose our base case $n=1$ , then $A = \{a_1\}$ where $A$ is a set with a single element thus that single element is both the first and last element (according to *definition 3.3*). 

Now for the inductive hypothesis, we can assume when $n = k$, where $k$ is a positive integer. $A$ has a first element $a_i$ and the last point is $a_k$ such that $a_1 < a_k$. 

Finally, our inductive step proves our assumption holds for when $A$ contains $n=k+1$ elements. There are three possible cases : 
1. $a_{k+1} < a_1 < a_k $
2. $a_1 < a_{k+1} < a_k$
3. $a_1 < a_k < a_{k+1}$

All these are true for the inductive step and maintain the existence of the first and last element, therefore any finite subset $A$ of a continuum $C$, it has a first and last point.

**Theorem 3.5: Suppose that $A$ is a set of $n$ distinct points in a continuum $C$, or, in other words, $A \sub C$ has cardinality $n$. Then symbols $a_1,...a_n$ may be assigned to each point of $A$ so that $a_1, a_2, <... < a_n, \; ie. \; a_i < a_{i+1} \; for \; 1 \leq i \leq n-1$.**
Suppose we have a set $X$ with elements $\{a_1, a_2, < ... < a_n\}$. We can essentially assign the elements of set $X$ to the first point in $A$ according to *Lemma 3.4* which says that $A$ which is a subset of $C$ has a first and last point. Thus as we move through set $X$, we can assign and remove element $a_1$ from set $A$ so that each element in $A$ will be assigned to symbols $a_1,...a_n$ in set $X$.

**Corollary 3.7: Of three distinct points in a continuum, one must be between the two other.**
Consider *Theorem 3.5* where we proved each point in a subset of a continuum $C$ to a symbol $a_1, a_2,...,a_n$ in ascending order. In this case, we can order this set $C = \{c_1, c_2,c_3\}$ where $c_1 < c_2 < c_3$ thus $c_2$ is between $c_1$ and $c_3$.

**Exercise 3.8**: 
**a. We define a relation $<$ on $\Z$ by $m < n $ if $n = m + c$ for some $c \in \N$. Show that, $\Z$, with the ordering $<$, satisfies *Axion 1-3*.**
Let us be reminded of *Axioms 1-3*.
*Axiom 1. A continuum is a nonempty set $C$.* 
First, let us identify $\Z$ as a continuum because it's a nonempty (infinite) set of integers. For example, the set $\Z$ contains elements such as $\{-1,0,1,2\}$. This means $\Z$ fulfills *axiom 1*.


*Axiom 2. A continuum $C$ has an ordering $<$*
We can identify $m$ and $n$ as distinct points in $\Z$ and $c$ as a positive integer. For *Axiom 2* to prove true, an ordering on the set represented by $\Z \times \Z$ with elements $(m,n)$ written as $m < n$ must satisfy these conditions according to *definition 3.1*: 

Trichotomy, where for all $m,n \in \Z$ one of the following holds: $m < n, m = n, \; \textnormal{or} \; m > n $. Because we defined $m < n$ if $n = m + c$, then trichotomy is satisfied as one of the above held true. This is also because when $n=m+c$ and $c \in \N$ and $c = n-m$, $m \neq n$ because $c$ would have to equal $0$, and $m \ngeq n$ because $c$ would have to be negative, both of which are not within the set $\N$ thus, $m < n$ is the only case and trichotomy is true in the continuum $Z$.

Transistivity: where for all $m,n,l \in \Z$, if $m < n$ and $n < l$ then $m < l$. Let's suppose $n = m + a$, $l = n + b$, and $l = m + c$ where $a,b,c \in \N$. From this, we can deduce $n > m$ because $a = m - n$. We can substitute $m+a$ for $n$ to get $l = m + a + b$. If $a,b$ are both positive integers more than $0$, then $l$ must be greater than $m$ which proves that if $n > m$ and $l > n$, then $l > m$. Therefore, the transistivity property is true for an ordering $<$ of continuum $\Z$.

With both Trichotomy and Transistivty satisfied, we can conclude that the continuum $\Z$ has an ordering $<$.

*Axiom 3. A continuum $C$ has no first or last point*

This is true, as $\Z$ has no first nor last point. This is because $\Z$ is an infinite set thus there is no $a_1 \in \Z$ and $a_i \in \Z$ where $a_i$ is any element of $\Z$ and $a_1 < a_i$ for all $i$ nor is there any element $a_n$ that represents the last element of $\Z$ because $\Z$ is an infinite set with no first nor last element.

Therefore, $\Z$ with the ordering $<$, satisfies axioms 1-3.


**b. Show that, for any $p = \{\frac a b\} \in \mathbb{Q}$, there is some $(a_1, b_1) \in p$ with $0 < b_1$.**

Let us first determine if there is some $(a_1, b_1) \in p$. As we have observed in *Exercise 2.6: $[\frac a b] = [\frac {a_1} {b_1}] = (a,b)$ ~ $(a_1, b_1)$.* Thus, we may find an equivalent fraction for any rational number $p$ such that $[\frac a b] = [\frac {a_1} {b_1}]$ by dividing both $a,b$ by their greatest common divisor (GCD). We know based on the equivalence relation established in *Exercise 2.2* that $[\frac a b] = (a,b)$ and conversely $[\frac {a_1} {b_1}]  = (a_1, b_1)$. Thus since $(a,b) \in p$ and $(a,b)$ ~ $(a_1, b_1)$, then $(a_1, b_1) \in p$. Note that by dividing $b$ by a GCD and because $p$ is a rational number and fractions cannot have $0$ in their denominator, $b$ must be a positive integer and thus $b > 0$. 

There exists 3 cases for $(a_1, b_1)$ where $b_1 >0$:
    1. $ \{\frac {a_1} {b_1}\}$ is zero:
   In this case, $a_1$ must be $0$ such that $b_1$ must be either positive or negative so  $\{\frac {a_1} {b_1}\} = 0$ and $0 < b_1$.
    2. $ \{\frac {a_1} {b_1}\}$ is positive:
   In this case, both $a_1$ and $b_1$ are positive or both are negative, thus there exists a $b_1$ such that $b_1 > 0$
    3. $ \{\frac {a_1} {b_1}\}$ is negative:
   In this case, either $a_1$ or $b_1$ is negative so in the case $a_1 <0$ then there is some $b_1$ can be expressed as $b_1 > 0$ 
So for all cases 0, positive, and negative, there exists some $b_1 > 0$.

**c. We define a relation $<_\mathbb{Q}$ on $\mathbb{Q}$ as follows. For $p, q \in \mathbb{Q}$, let $(a_1,b_1) \in p$ be such that $0 < b_1$, and let $(a_2, b_2) \in q$ be such that $0 < b_2$. Then we define $p <_\mathbb{Q} q$ if $a_1b_2 < a_2b_1$. Show that $<_\mathbb{Q}$ is a well-defined relation on $\mathbb{Q}$.** 

Suppose $(a,b)$ ~ $(a',b')$ and $(c,d)$~$(c',d')$, and by *part b* we know that $b,b',d,d'$ can all be $>0$. By definition of the ~ relation in *exercise 2.2 e* we know that $ab' = a'b$ and $cd' = c'd$ such that $[\frac a b] = [\frac {a'} {b'}]$ and $ [\frac c d] = [\frac {c'} {d'}]$. 

We want to show that $[a,b]  <_\mathbb{Q} [c,d]$ is equivalent to $[(a',b')]  < [(c',d')] $. We can suppose $[(a,b)] <_\mathbb{Q} [c,d]$ which means $ad <_\mathbb{Q} cd$ so $[\frac a b] <_\mathbb{Q}[\frac c d] $ which results in $[\frac {a'} {b'}] = [\frac a b] <_\mathbb{Q} [\frac c d] = [\frac {c'} {d'}]$. From this, we know that $a'd' <_\mathbb{Q} b'c'$ so that $[(a'b')] <_\mathbb{Q} (c',d')$.


**d. Show that $\mathbb{Q}$, with the ordering $<_\mathbb{Q}$, satisfies *Axioms 1-3*.**

Let us be reminded of *Axioms 1-3*.
*Axiom 1. A continuum is a nonempty set $C$.* 
First, let us identify $\mathbb{Q}$ as a continuum because it's a nonempty (infinite) set of rational numbers (fractions). For example, the set $\mathbb{Q}$ contains elements such as $\{(\frac 0 1), (\frac 1 1), (\frac {-1} 1), (\frac {1} 2)\}$ and so on. This means $\mathbb{Q}$ fulfills *axiom 1*.


*Axiom 2. A continuum $C$ has an ordering $<$*
 For *Axiom 2* to prove true, an ordering on the set represented by $\mathbb{Q} \times \mathbb{Q}$ with elements $p,q$ written as $p <_\mathbb{Q} q$ must satisfy these conditions according to *definition 3.1*: 

Trichotomy: We can identify $p$ and $q$ as distinct points in $\mathbb{Q}$ where $(a_1,b_1) \in p$ and $(a_2, b_2) \in q$  where for all $p,q \in \mathbb{Q}$ one of the following holds: $p <_\mathbb{Q} q, p =_\mathbb{Q} q, \; \textnormal{or} \; p >_\mathbb{Q} q $. Because we defined $p <_\mathbb{Q} q$ if $a_1b_2 < a_2b_1$, then trichotomy is satisfied as one of the above held true.

Transistivity: We can identify $p$ and $q$ as distinct points in $\mathbb{Q}$ where $(a_1,b_1)$ in $p$ and $(a_2, b_2) \in q$ and define a point $x \in \mathbb{Q}$ and let $(a_3, b_3) \in x$ be such that $0 < b_1,b_2, b_3$ based on *part 2* and let's make $x$ so $q = p +_\mathbb{Q} x$. For all $p,q,x \in \mathbb{Q}$, if $p < q$ and $q < x$ then $p < x$. This is equivalent to $[\frac {a_1} {b_1}] < [\frac {a_2} {b_2}] < [\frac {a_3} {b_3}]$, and by substitution we know that $[\frac {a_1} {b_1}] < [\frac {a_3} {b_3}]$. Therefore, the transistivity property is true for an ordering $<$ of continuum $\mathbb{Q}$.

With both Trichotomy and Transistivty satisfied, we can conclude that the continuum $\mathbb{Q}$ has an ordering $<_\mathbb{Q}$.

*Axiom 3. A continuum $C$ has no first or last point*
This is true, as $\mathbb{Q}$ has no first nor last point. This is because $\mathbb{Q}$ is a dense infinite set thus there is no $a_1 \in \mathbb{Q}$ and $a_i \in \mathbb{Q}$ where $a_i$ is any element of $\mathbb{Q}$ and $a_1 < a_i$ for all $i$ nor is there any element $a_n$ that represents the last element of $\mathbb{Q}$ because $\mathbb{Q}$ is an infinite set where between any two distinct rational numbers, there is another rational number. Thus $\mathbb{Q}$ has no first nor last element.

Therefore, $\mathbb{Q}$ with the ordering $<$, satisfies axioms 1-3.

**Theorem 3.11: If $x$ is a point of a continuum $C$, then there exists a region $\underline{ab}$ such that $x \in \underline{ab}$ .**
Let us remember *Definition 3.9: If $a, b ∈ C$ and $a < b$, then the set of points between $a$ and $b$ is called a region, denoted by $\underline{ab}$.*
Let us mimic this region by creating a subset of $C$ called $A$ of points between $a$ and $b$ where $a$ is the first point and $b$ is the last point then by *axiom 2 and 3*, the point $a < x$ and $b > x$ such that the $a<x<b$ and by transitivity $a<b$. This is possible through *Lemma 3.4* which defines the first and last points of subset $A$ and *Corollary 3.5* which indexes each point point in the subset in ascending order. Because $A$ can be arranged in ascending order $(a_1, a_2, a_3,...a_n)$ where $a_1 = a$ and $a_n = b$ where $n$ is the cardinality of $A$, there must be an $a_i = x$ where $i \in \N$ and is between $1$ and $n$. Therefore, $x$ must be a point existing within the region $\underline{ab}$.


**Theorem 3.13: If $p$ is a limit point of $A$ and $A \sub B$, then $p$ is a limit point of $B$.**
Let us be reminded of *Definition 3.12: a limit point is a point $p$ of continuum $C$ in subset $A$ if every region $R$ containing $p$ has nonempty intersection with $A\backslash \{p\}$ which means for every region $R$ with $p \in R$, we have $R \cap (A \backslash \{p\}) \neq \empty$*. 

Since $p$ is a limit point of $A$, then for all regions $R$ containing $p$,  $R \cap (A \backslash \{p\}) \neq \empty$. Let $q \in A$ be an intersection point with $R \cap (A \backslash \{p\}) \neq \empty$, and since $A \sub B$, then $q \in B$. Thus, given an $R$ containing $p$, there is a $q \in R \cap B \backslash \{p\}$ which means $p$ is a limit point of $B$.


**Lemma: 3.15: If $\underline{ab}$ is a region in a continuum $C$, then,  ext $\underline{ab} = \{x \in C | x < a \} \cup \{x \in C| b < x\}$**

**FIX**
Consider *Definition 3.14: If $\underline{ab}$ is a region of continuum $C$, then $C \backslash (\{a\} \cup \underline{ab} \cup \{b\})$. is called the exterior of $\underline{ab}$ denoted by ext $\underline{ab}$.*

We want to show ext $\underline{ab} = \{x \in C | x < a \} \cup \{x \in C| b < x\}$. We know that:

if $x \nleq a$, then $x \geq a$
if $x \ngeq b$, then $x \leq b$

We can formulate the equation: $C\backslash (\{a\} \cup \underline{ab} \cup \{b\}) = \{x \in C | x < a\} \cup \{x \in C | b< x\}$. We can simplify the LHS to $C\backslash( x\geq a \cap x \leq b)$ which equals to the RHS $\{x \in C| C\backslash(x \geq a) \cup C\backslash (x \leq b)\}$ . 




**Lemma 3.16: No point in the exterior of a region is a limit point of that region. No point of a region is a limit point of the exterior of that region.**

**FIX**

Proof by contradiction: 
Consider the set $E = ext \; \underline{ab}$ where $E \cap R \neq \empty$. Let $e \in E$ where $e$ is a limit point of $\underline{ab}$. If $a$ and $b$ are in the continuum $C$, then $e < a$ where $a'$ is an element such that $a' < e < a$ because the continuum has no first or last point. Or $e > b$ such that there is a $b'$ where $b < e < b'$ because the continuum has no first or last point. Because $\underline{a'a} \cap  \underline{ab} \backslash e = \empty$ or $\underline{bb'} \cap \underline{ab} \backslash e = \empty$ and since $e \in \underline{ab}$, then $a < e < b$ and $a' < a$ which means that $\underline{ab} \cap \underline{a'a} \backslash \{e\} = \empty$. And thus $b < b'$ which means that $\underline ab \cap \underline{bb'} \backslash \{e\} = \empty$ or $\underline{ab} \cap E \backslash \{e\} = \empty$.

**Theorem 3.17: If two regions have a point $x$ in common, their intersection is the region containing $x$.**


Let $x \in \underline{ab}$ and $x \in \underline{cd}$, which means $a,b,c,d \in C$ and $a < b$ and $c < d$. We can infer that $a < x$ and $x < b$ and $c < x$ and $x < d$. By the definition of a region, we know that $a < b$ and $c < d$, and by trichotomy, we know that $a<x<d$ and $c<x<b$. If $x \in \underline{ab} \cap \underline{cd}$, then $x$ is in a region, $R$ that is between the least value (whether $a$ or $c$) and the greatest value $b$ or $d$ 

Be aware of our four cases that results from this: 
1. $a< c < b< d$, intersection of regions is $\underline{cb}$
2. $a < c <d <c$, intersection of regions is $\underline{cd}$
3. $c < a < b <d$, intersection of regions is $\underline{ab}$
4. $c < a < d < b$, intersection of regions is $\underline{ad}$

Because all of the resulting intersections contain $x$, then $x \in (\underline{ab} \cap \underline{cd})$.

**Corollary 3.18: If $n$ regions $R_1,..., R_n$ have a point $x$ in common, then their intersection $R_1 \cup ... \cap R_n$ is a region containing $x$.**
Proof by induction: If a region $R$, $R_n$ $x$, then the intersection $R$ 

Base case $(n=1)$, $R_1$ contains $x$ because it is the only region and has intersection with itself.

Inductive hypothesis, we assume $n = k$, so if $R_1... R_k$ all contains $x$, then $R_1 \cap R_k$ contains $x$.

Inductive step, we can show it holds for $(n = k+1)$. Let $K = R_1 \cap R_n \cap R_n$ based on our hypothesis. We know that $K$ is a region containing $x$. Thus $R_1 \cap R_2 $, $R_k \cap R_{k+1} = K \cap R_{k+1}$. The intersection of 2 regions containing $x$ because $R_{k+1}$ contains $x$. By *theorem 3.17 *, we have $K \cap R_{k+1}$ is a region containing $x$.

**Theorem 3.19: Let $A$, $B$ be subsets of a continuum $C$. Then $p$ is a limit point of $A ∪ B$ if, and only if, $p$ is a limit point of at least one of $A$ or $B$.**

**PROVE REVERSE, IFF, possible to use 1.7 and 3.13**

We can prove this this by contradiction. Let us assume that there exists a $p$ which is a limit point of $A \cup B$ but not a limit point of either $A$ nor $B$. This means $p$ must satisfy 3 conditions:

$p$ is a limit point of $A \cup B$: For $p$ to be a limit point, then for every region $R$ containing $p$ with $p \in R$, $R \cap (A \cup B \backslash \{p\}) \neq \empty$. This means that there must be elements of either $A$ or $B$ for any region $R$ excluding $p$, such that there is an element $x \neq p \in A\cup B$ for regions $R$ containing $p$.

$p$ is not a limit point of $A$: If $p$ is not a limit point of $A$, then for every region $R$ containing $p$ with $p \in R, R \cap (A \backslash \{p\}) = \empty$. This means that there is no element $x \neq p$ in $A$ for any region $R$ containing $p$. 

$p$ is not a limit point of $B$:If $p$ is not a limit point of $B$, then for every region $S$ containing $p$ with $p \in S, S \cap ( B \backslash \{p\}) = \empty$. This means that there is no element $x \neq p$ in $B$ for any region $S$ containing $p$. 

This is contradictory because if $x \notin A$ and $x \notin B$, then $x \notin A\cup B$ which contradicts our assumption that there is an element  $x \in A\cup B$ for regions $R$ and $S$ containing $p$. Therefore, the limit point $p$ is a limit point of $A ∪ B$ if, and only if, $p$ is a limit point of at least one of $A$ or $B$.

**Corollary 3.20: Let $A_1, . . . , A_n$ be $n$ subsets of a continuum $C$. Then $p$ is a limit point of $A_1 ∪ · · · ∪ A_n$ if, and only if, $p$ is a limit point of at least one of the sets $A_k$.**

Let us be reminded of *Theorem 3.19: Let $A$, $B$ be subsets of a continuum $C$. Then $p$ is a limit point of $A ∪ B$ if, and only if, $p$ is a limit point of at least one of $A$ or $B$.* Now, let's solve this with mathematical induction: 

Base case$(n=1)$: We can prove that $p$ is a limit point for a single set $A_1$ if and only if $p$ is a limit point of $A_1$ which is inherently true.

Inductive hypothesis $(n=k)$: We assume that the statement is true when $n=k$ such that for any subsets $A_1, A_2, ...,  A_k$ of a continuum $C$, $p$ is a limit point of $A_1 \cup A_2, ..., \cup A_k$ if and only if $p$ is a limit point of at least one of the sets $A_i$. 

Inductive step $(n=k+1)$: 

To prove that our hypothesis holds for $(n = k+1)$, we must show that for subsets $A_1, A_2, ..., A_{k+1}$ of continuum $C$, $p$ is a limit point of $A_1 \cup A_2, ..., \cup A_{k+1}$ if and only if $p$ is a limit point of at least one of the sets $A_i$.

Let's first consider the forward direction, where $p$ is a limit point of $A_1 \cup A_2, ..., \cup A_{k+1}$. By the inductive hypothesis, we know that if $p$ is a limit point of the union of the first $k$ sets $A_1, A_2, ..., A_k$, then it must be a limit point of at least one of them.

Now, we check the reverse direction. If $p$ is a limit point of at least one of the sets $A_i$, we want to show that it is indeed a limit point of $A_1 \cup A_2, ..., \cup A_{k+1}$.

Consider the case where $p$ is a limit point of $A_k+1$. By *Theorem 3.19*, we can state that the limit point of a set is also a limit point of the union between that set and another. Thus, if $p$ is a limit point of $A_{k+1}$, it is also a limit point of the union $A_1 \cup A_2, ..., \cup A_k \cup A_{k+1}$.

**SHOW IT FOR REERSE OF REVERSE**

We have now proven both directions of the statement, ensuring that $p$ is a limit point of $A_1 \cup A_2, ..., \cup A_{k+1}$ if and only if $p$ is a limit point of at least one of the sets $A_i$. 


**Theorem 3.21: If $p$ and $q$ are distinct points of a continuum $C$, then there exist disjoint regions $R$ and $S$ containing $p$ and $q$, respectively.**

Let's make $p$ and $q$ arbitary points in $C$ and $p < q $. Also, let's assume $p' \in C$ where $p' < p$ and $q' \in C$ where $q' < q$. Now let's examine the possible cases:

1. At least 1 point between $p$ and $q$:
   Let $c$ be the point between $p$ and $q$ forming two regions $R =\underline{cp'}$ and $S= \underline{q'c}$. They must be disjoint because they both have $c$ as one of their limits (but does not include it) and include $p$ and $q$ respectively.

2. No points between $p$ and $q$
   There are two regions $q \in \underline{pp'}$ and $p \in \underline{qq'}$, and because there are no points between $p$ and $q$, then the regions are disjoint as they contain no similar elements in their regions. 

**Corollary 3.22. A subset of a continuum C consisting of one point has no limit points.**

Let us be reminded of the definition of a limit point: *Let $A$ be a subset of a continuum $C$. A point $p$ of $C$ is called a limit point of $A$ if every region $R$ containing $p$ has nonempty intersection with $A \backslash \{p\}$. This means for every region $R$ with $p \in R$, we have $R \cap (A \backslash \{p\}) \neq \empty$ .*

Let us prove by contradiction: 

Assume that a subset $A$ of continuum $C$ consists of one point, $x \in A$ and has a limit point $p$ which is not necessarily in $A$. We have 2 cases:
1. $x=p$
   If $A$ only has $x$ which is a limit point, we can check that $R \cap (\{x\} \backslash \{p\}) = R \cap \empty = \empty$ thus $p$ is not a limit point of $A$.
2. $ x \neq p$
   If $x$ and $p$ are distinct points in $C$, then by *theorem 3.21* there exists disjoint regions $A$ and $R$ containing $x$ and $p$ respectively such that $p$ is not a limit point of $A$.

    2a. $p > x$
    Let $a$ and $b$ be two points such that $x < a < p < b$ and $R = \underline{bc}$ so $p \in R$, so  $(R\cap A) \backslash \{x\} \neq \empty$. But because $R$ does not contain $x$, it contains no points in set $A$ thus $R \cap A = \empty$ which disproves our previous statement.

    2b. $p < x$
    Let $c$ and $d$ be distinct points such that $c <p < d< x$ and the region $R = \underline{cd}$ such that $p \in R$. Based off of this, we know that $(R \cap A) \backslash \{x\} \neq \empty$, but because $R$ does not contain point $x$, it has no elements in its intersection with set $A$ such that $R \cap A = \empty$. Thus our previous statement is false and we have a contradiction. 

**Theorem 3.23: A finite subset $A$ of a continuum $C$ has no limit points.**
A finite subset will contain a region $R$ that is between two points surrounding any point such that the intersection between $R$ and $A$ will be the empty set. Let $A = A_1 \cup A_n$ where they are all subsets of $C$ consisting of one point. Based on *Corollary 3.20: for $p$ to be limit point of the union of sets, it must be a limit point of at least one of the sets*. From this, we can see that $p$ cannot be a limit point of any sets $A_1...A_n$ because they consist only of one element which means none of the sets can have a limit point by *Corollary 3.22*. 

**Corollary 3.24: If $A$ is a finite subset of a continuum $C$ and $x ∈ A$, then there exists a region $R$, containing $x$, such that $A ∩ R = \{x\}$.**

Order $A$ by *theorem 3.5* and let $A = \{a_1...a_n\}$ where some $a_k = x$. Let $A' = \{a_1...a_{k-1}\}$ and let $A'' = \{a_{k+1}...a_n\}$. Because $a_{k-1} < x < a_{k+1}$, let the region $R = \underline{a_{k-1}a_{k+1}}$ which contains $x$ and no other points in $A$. If $x$ is $a_1$ then the region will be $R = \underline{(\textnormal{element of C} < a_1) a_{2}}$ and if $x$ is the last element then the region will be $R = \underline{a_n (\textnormal{element of C} > a_n)}$. Thus $A \cap R = \{x\}$.

**Theorem 3.25: If $p$ is a limit point of $A$ and $R$ is a region containing $p$, then the set $R ∩ A$ is infinite.**
**FIX**

Because $p$ is a limit point of $A$, then by definition, for all regions $R$ where $p \in R$, $R\cap (A\backslash \{p\} \neq \empty)$. For each region $R$, we can say that $A$ is the union of all elements in $A$ also in the region $R$ and all elements of $A$ that aren't in $R$. Since we are given that $p$ is a limit point of $A$, we know that $p$ is a limit point of either $R \cap A$ or $A \backslash R \cap A$. Because $A\backslash (R \cap A)$ contains elements in $A$, but not in $R$, then $R \cap (A \backslash(R \cap A)) = \empty$ which implies that $R \cap (A \backslash (R \cap A)) \backslash \{p\} = \empty$. Therefore $p$ is not a limit point of $(A \backslash (R \cap A))$ and by *theorem 3.19*, $p$ must be a limit point of $R\cap A$. By *theorem 3.20*, we know that finite subsets of continuums have no limit points, so subsets with a limit point must be infinite. Thus, because $p$ is a limit point of $R \cap A$, $R\cap A$ must be infinite.


**Exercise 3.26: Find realizations of a continuum $(C, <)$. That is, find concrete sets $C$ endowed with a relation $<$ satisfying all of the axioms (so far). Are they the same? What does “the same” mean here?**
For every $R$ where $p \in R$, $R \cap A$ is infinite.
By Contradiction we can prove $A \cap R$ is finite.
$S_0 = $A \cap R$ 
$S_1 = \{x \in S_0, x < p\}, x_L$ is last point of $S_1$
If $S_1 = \empty$, then the region $\underline{ax_L}$ that contains $p$ is $\underline{ax_L} \cap A\backslash \{p\} = \empty$ so $p$ is not a limit point.

$S_2 = \{x \in S_0, x > p\} x_F$ is first point of $S_2$
If $S_2 = \empty$ then the region $\underline{x_Lb}$ such that $\underline{x_Lb} \cap A \backslash\{p\} = empty$ so $p$ is not a limit point.

Therefore the region $\underline{x_Lx_F}$ contains $p$, and $\underline{x_Lx_F} \cap A\backslash \{p\} = \empty$, so $p$ is not a limit point of $A$.