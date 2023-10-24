***<h1 style="text-align: center;">Script 3</h1>***
**Lemma 3.4: If $A$ is a nonempty, finite subset of a continuum $C$, then $A$ has a first and last point.**
We can prove that $A$ has a first and last point through induction.

Suppose our base case $n=1$ , then $A = \{a_1\}$ where $A$ is a set with a single element thus that single element is both the first and last element (according to *definition 3.3*). Now for the inductive hypothesis, we can assume when $n = k$, where $k$ is a positive integer. $A$ has a first element $a_i$ and the last point is $a_k$ such that $a_1 < a_k$. Finally, our inductive step proves our assumption holds for when $A$ contains $n=k+1$ elements. There are three possible cases : 
1. $a_{k+1} < a_1 < a_k $
2. $a_1 < a_{k+1} < a_k$
3. $a_1 < a_k < a_{k+1}$

All these are true for the inductive step and maintain the existence of the first and last element, therefore any finite subset $A$ of a continuum $C$, it has a first and last point.

**Theorem 3.5: Suppose that $A$ is a set of $n$ distinct points in a continuum $C$, or, in other words, $A \sub C$ has cardinality $n$. Then symbols $a_1,...a_n$ may be assigned to each point of $A$ so that $a_1, a_2, <... < a_n, \; ie. \; a_i < a_{i+1} \; for \; 1 \leq i \leq n-1$.**
Suppose we have a set $X$ with elements $\{a_1, a_2, < ... < a_n\}$. We can essentially assign the elements of set $X$ to the first point in $A$ according to *Lemma 3.4* which says that $A$ which is a subset of $C$ has a first and last point. Thus as we move through set $X$, we can assign and remove element $a_1$ from set $A$ so that each element in $A$ will be assigned to symbols $a_1,...a_n$ in set $X$.

**Corollary 3.7: Of three distinct points in a continuum, one must be between the two other.**
Consider *Theorem 3.5* where we proved each point in a subset of a continuum $C$ to a symbol $a_1, a_2,...,a_n$ in ascending order. In this case, points assigned to index $i$ would be less than points $i+1$. 
**MORE**

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

As we have observed in *Exercise 2.6: $[\frac a b] = [\frac {a_1} {b_1}] = (a,b)$ ~ $(a_1, b_1)$*. Thus, we may find an equivalent fraction for any rational number $p$ such that $[\frac a b] = [\frac {a_1} {b_1}]$ by dividing both $a,b$ by their greatest common divisor (GCD). We know based on the equivalence relation established in *Exercise 2.2* that $[\frac a b] = (a,b)$ and conversely $[\frac {a_1} {b_1}]  = (a_1, b_1)$. Thus since $(a,b) \in p$ and $(a,b)$ ~ $(a_1, b_1)$, then $(a_1, b_1) \in p$. Note that by dividing $b$ by a GCD and because $p$ is a rational number and fractions cannot have $0$ in their denominator, $b$ must be a positive integer and thus $b > 0$. 

**c. We define a relation $<_\mathbb{Q}$ on $\mathbb{Q}$ as follows. For $p, q \in \mathbb{Q}$, let $(a_1,b_1) \in p$ be such that $0 < b_1$, and let $(a_2, b_2) \in q$ be such that $0 < b_2$. Then we define $p <_\mathbb{Q} q$ if $a_1b_2 < a_2b_1$. Show that $<_\mathbb{Q}$ is a well-defined relation on $\mathbb{Q}$.** 



**d. Show that $\mathbb{Q}$, with the ordering $<_\mathbb{Q}$, satisfies *Axioms 1-3*.**

Let us be reminded of *Axioms 1-3*.
*Axiom 1. A continuum is a nonempty set $C$.* 
First, let us identify $\mathbb{Q}$ as a continuum because it's a nonempty (infinite) set of rational numbers (fractions). For example, the set $\mathbb{Q}$ contains elements such as $\{(\frac 0 1), (\frac 1 1), (\frac {-1} 1), (\frac {1} 2)\}$ and so on. This means $\mathbb{Q}$ fulfills *axiom 1*.


*Axiom 2. A continuum $C$ has an ordering $<$*
We can identify $p$ and $q$ as distinct points in $\mathbb{Q}$ and define a point $x \in \mathbb{Q}$ and let $(a_3, b_3) \in x$ be such that $0 < b_3>$ and let's make $x$ so $q = p +_\mathbb{Q} x$. For *Axiom 2* to prove true, an ordering on the set represented by $\mathbb{Q} \times \mathbb{Q}$ with elements $p,q$ written as $p <_\mathbb{Q} q$ must satisfy these conditions according to *definition 3.1*: 

**CONTINUE HERE**
Trichotomy, where for all $p,q \in \mathbb{Q}$ one of the following holds: $p <_\mathbb{Q} q, p =_\mathbb{Q} q, \; \textnormal{or} \; p >_\mathbb{Q} q $. Because we defined $p <_\mathbb{Q} q$ if $a_1b_2 < a_2b_1$, then trichotomy is satisfied as one of the above held true. This is also because when $n=m+c$ and $c \in \N$ and $c = n-m$, $m \neq n$ because $c$ would have to equal $0$, and $m \ngeq n$ because $c$ would have to be negative, both of which are not within the set $\N$ thus, $m < n$ is the only case and trichotomy is true in the continuum $Z$.

Transistivity: where for all $m,n,l \in \Z$, if $m < n$ and $n < l$ then $m < l$. Let's suppose $n = m + a$, $l = n + b$, and $l = m + c$ where $a,b,c \in \N$. From this, we can deduce $n > m$ because $a = m - n$. We can substitute $m+a$ for $n$ to get $l = m + a + b$. If $a,b$ are both positive integers more than $0$, then $l$ must be greater than $m$ which proves that if $n > m$ and $l > n$, then $l > m$. Therefore, the transistivity property is true for an ordering $<$ of continuum $\Z$.

With both Trichotomy and Transistivty satisfied, we can conclude that the continuum $\Z$ has an ordering $<$.

*Axiom 3. A continuum $C$ has no first or last point*

This is true, as $\mathbb{Q}$ has no first nor last point. This is because $\mathbb{Q}$ is a dense infinite set thus there is no $a_1 \in \mathbb{Q}$ and $a_i \in \mathbb{Q}$ where $a_i$ is any element of $\mathbb{Q}$ and $a_1 < a_i$ for all $i$ nor is there any element $a_n$ that represents the last element of $\mathbb{Q}$ because $\mathbb{Q}$ is an infinite set where between any two distinct rational numbers, there is another rational number. Thus $\mathbb{Q}$ has no first nor last element.

Therefore, $\Z$ with the ordering $<$, satisfies axioms 1-3.

**Theorem 3.11: If $x$ is a point of a continuum $C$, then there exists a region $\underline{ab}$ such that $x \in \underline{ab}$ .**

Let us remember *Definition 3.9: If $a, b ∈ C$ and $a < b$, then the set of points between $a$ and $b$ is called a region, denoted by $\underline{ab}$.*
Let us mimic this region by creating a subset of $C$ called $A$ of points between $a$ and $b$ where $a$ is the first point and $b$ is the last point. This is possible through *Lemma 3.4* which defines the first and last points of subset $A$ and *Corollary 3.5* which indexes each point point in the subset in ascending order. Because $A$ can be arranged in ascending order $(a_1, a_2, a_3,...a_n)$ where $a_1 = a$ and $a_n = b$ where $n$ is the cardinality of $A$, there must be an $a_i = x$ where $i \in \N$ and is between $1$ and $n$. Therefore, $x$ must be a point existing within the region $\underline{ab}$.


**Theorem 3.13: If $p$ is a limit point of $A$ and $A \sub B$, then $p$ is a limit point of $B$.**

Let us be reminded of *Definition 3.12: a limit point is a point $p$ of continuum $C$ in subset $A$ if every region $R$ containing $p$ has nonempty intersection with $A\backslash \{p\}$ which means for every region $R$ with $p \in R$, we have $R \cap (A \backslash \{p\}) \neq \empty$*. 

Since $p$ is a limit point of $A$, then for all regions $R$ containing $p$,  $R \cap (A \backslash \{p\}) \neq \empty$*. Let $q \in A$ be an intersection point with $R \cap (A \backslash \{p\}) \neq \empty$, and since $A \sub B$, then $q \in B$. Thus, given an $R$ containing $p$, there is a $q \in R \cap B \backslash \{p\}$.  


**Lemma: 3.15: If $\underline{ab}$ is a region in a continuum $C$, then,  ext $\underline{ab} = \{x \in C | x < a \} \cup \{x \in C| b < x\}$**

**FIX**
Consider *Definition 3.14: If $\underline{ab}$ is a region of continuum $C$, then $C \backslash (\{a\} \cup \underline{ab} \cup \{b\})$. is called the exterior of $\underline{ab}$ denoted by ext $\underline{ab}$.*

We want to show ext $\underline{ab} = \{x \in C | x < a \} \cup \{x \in C| b < x\}$. We know that:

if $x \nleq a$, then $x \geq a$
if $x \ngeq b$, then $x \leq b$

We can formulate the equation: $C\backslash (\{a\} \cup \underline{ab} \cup \{b\}) = \{x \in C | x < a\} \cup \{x \in C | b< x\}$. We can simplify the LHS to $C\backslash( x\geq a \cap x \leq b)$ which equals to the RHS $\{x \in C| C\backslash(x \geq a) \cup C\backslash (x \leq b)\}$ . 




**Lemma 3.16: No point in the exterior of a region is a limit point of that region. No point of a region is a limit point of the exterior of that region.**

**FIX**

Proof by contradiction: Consider the set $E = ext \; \underline{ab}$ where $E \cap R \neq \empty$. Let $e \in E$ where $e$ is a limit point of $\underline{ab}$. If $a$ and $b$ are in the continuum $C$, then $e < a$ where $a'$ is an element such that $a' < e < a$ because the continuum has no first or last point. Or $e > b$ such that there is a $b'$ where $b < e < b'$ because the continuum has no first or last point. Because $\underline{a'a} \cap  \underline{ab} \backslash e = \empty$ or $\underline{bb'} \cap \underline{ab} \backslash e = \empty$ and since $e \in \underline{ab}$, then $a < e < b$ and $a' < a$ which means that $\underline{ab} \cap \underline{a'a} \backslash \{e\} = \empty$. And thus $b < b'$ which means that $\underline ab \cap \underline{bb'} \backslash \{e\} = \empty$ or $\underline{ab} \cap E \backslash \{e\} = \empty$.

**Theorem 3.17: If two regions have a point $x$ in common, their intersection is the region containing $x$.**

**FIX**
Let $x \in \underline{ab}$ and $x \in \underline{cd}$, which means $a,b,c,d \in C$ and $a < b$ and $c < d$. We can infer that $a < x$ and $x < b$ and $c < x$ and $x < d$. If $x \in \underline{ab} \cap \underline{cd}$, then $x$ is in a region, $R$, that is between the least value (whether $a$ or $c$) and the greatest value $b$ or $d$. Let $a$ be the smallest, then $c < b$. 

Be aware of our four cases: $a< c < b< d$, $c < a < b< d$, $a < c <d <c$, $c < a < d < b$

Because $R$ encompasses both $\underline{ab}$ and $\underline{cd}$, then $x \in (\underline{ab} \cap \underline{cd})$.

**Corollary 3.18: If $n$ regions $R_1,..., R_n$ have a point $x$ in common, then their intersection $R_1 \cup ... \cap R_n$ is a region containing $x$.**

**FIX**

Proof by induction: If a region $R$, $R_n$ $x$, then the intersection $R$ 

Base case $(n=1)$, $R_1$ contains $x$ without intersection
Inductive hypothesis, we assume $n = k$, so if $R_1... R_k$ all contains $x$, then $R_1 \cap R_k$ contains $x$.
Inductive step, we can show it holds for $(n = k+1)$. Let $K = R_1 \cap R_n \cap R_n$ based on our hypothesis. We know that $K$ is a region containing $x$. Thus $R_1 \cap R_2 $, $R_k \cap R_{k+1} = K \cap R_{k+1}$. The intersection of 2 regions containing $x$. By *theorem 3.17 *, we have $K \cap R_{k+1}$ is a region containing $x$.

**Theorem 3.19: Let $A$, $B$ be subsets of a continuum $C$. Then $p$ is a limit point of $A ∪ B$ if, and only if, $p$ is a limit point of at least one of $A$ or $B$.**

We can prove this this by contradiction. Let us assume that there exists a $p$ which is a limit point of $A \cup B$ but not a limit point of either $A$ nor $B$. This means $p$ must satisfy 3 conditions:

$p$ is a limit point of $A \cup B$: For $p$ to be a limit point, then for every region $R$ containing $p$ with $p \in R$, $R \cap (A \cup B \backslash \{p\}) \neq \empty$. This means that there must be elements of either $A$ or $B$ for any region $R$ excluding $p$. This means that there must be an element $x \neq p \in A\cup B$ for regions $R$ containing $p$.

$p$ is not a limit point of $A$: If $p$ is not a limit point of $A$, then for every region $R$ containing $p$ with $p \in R, R \cap (A \backslash \{p\}) = \empty$. This means that there is no element $x \neq p$ in $A$ for any region $R$ containing $p$. 

$p$ is not a limit point of $B$:If $p$ is not a limit point of $B$, then for every region $R$ containing $p$ with $p \in R, R \cap ( B \backslash \{p\}) = \empty$. This means that there is no element $x \neq p$ in $B$ for any region $R$ containing $p$. 

This is contradictory because if $x \notin A$ and $x \notin B$, then $x \notin A\cup B$ which contradicts our assumption that there is an element  $x \in A\cup B$ for regions $R$ containing $p$. Therefore, the limit point $p$ is a limit point of $A ∪ B$ if, and only if, $p$ is a limit point of at least one of $A$ or $B$.

**Corollary 3.20: Let $A_1, . . . , A_n$ be $n$ subsets of a continuum $C$. Then $p$ is a limit point of $A_1 ∪ · · · ∪ A_n$ if, and only if, $p$ is a limit point of at least one of the sets $A_k$.**

Let us be reminded of *Theorem 3.19: Let $A$, $B$ be subsets of a continuum $C$. Then $p$ is a limit point of $A ∪ B$ if, and only if, $p$ is a limit point of at least one of $A$ or $B$.* Now, let's solve this with mathematical induction: 

Base case$(n=1)$: We can prove that $p$ is a limit point for a single set $A_1$ if and only if $p$ is a limit point of $A_1$ which is inherently true.

Inductive hypothesis $(n=k)$: We assume that the statement is true when $n=k$ such that for any subsets $A_1, A_2, ...,  A_k$ of a continuum $C$, $p$ is a limit point of $A_1 \cup A_2, ..., \cup A_k$ if and only if $p$ is a limit point of at least one of the sets $A_i$. 

Inductive step $(n=k+1)$: 

To prove that our hypothesis holds for $(n = k+1)$, we must show that for subsets $A_1, A_2, ..., A_{k+1}$ of continuum $C$, $p$ is a limit point of $A_1 \cup A_2, ..., \cup A_{k+1}$ if and only if $p$ is a limit point of at least one of the sets $A_i$.

Let's first consider the forward direction, where $p$ is a limit point of $A_1 \cup A_2, ..., \cup A_{k+1}$. By the induction hypothesis, we know that if $p$ is a limit point of the union of the first $k$ sets $A_1, A_2, ..., A_k$, then it must be a limit point of at least one of them.

Now, we check the reverse direction. If $p$ is a limit point of at least one of the sets $A_i$, we want to show that it is indeed a limit point of $A_1 \cup A_2, ..., \cup A_{k+1}$.

Consider the case where $p$ is a limit point of $A_k+1$. By *Theorem 3.19*, we can state that the limit point of a set is also a limit point of the union between that set and another. Thus, if $p$ is a limit point of $A_{k+1}$, it is also a limit point of the union $A_1 \cup A_2, ..., \cup A_k \cup A_{k+1}$.

We have now proven both directions of the statement, ensuring that $p$ is a limit point of $A_1 \cup A_2, ..., \cup A_{k+1}$ if and only if $p$ is a limit point of at least one of the sets $A_i$. 


**Theorem 3.21: If $p$ and $q$ are distinct points of a continuum $C$, then there exist disjoint regions $R$ and $S$ containing $p$ and $q$, respectively.**

Let's say that region $R$ is defined as $\underline {a_1b_1}$ and region $S$ is defined as $\underline {a_2b_2}$. Because the regions are disjoint, overlap would contradict the assumption. Let's examine multiple scenarios where overlap does not occur:

case 1: $p > q$
In this case, region $R$ must be such that $a_1 < p < b_1$ and region $S$ must be such that $a_2 < q < b_2$. For the regions to be disjoint, $b_2 < a_1$ must be true.

case 2: $p < q$ 
In this case, region $R$ must be such that $a_1 < p < b_1$ and region $S$ must be such that $a_2 < q < b_2$. For the regions to be disjoint, $b_1 < >_2$ must be true.

case 3: $p = q$
This case cannot be true because we are given that $p$ and $q$ are distinct points.

In all possible cases, the regions $R$, $S$ are disjoint with no overlap and contain point $p$ and $q$ respectively. 

**Corollary 3.22. A subset of a continuum C consisting of one point has no limit points.**

Let us be reminded of the definition of a limit point: *Let $A$ be a subset of a continuum $C$. A point $p$ of $C$ is called a limit point of $A$ if every region $R$ containing $p$ has nonempty intersection with $A \backslash \{p\}$. This means for every region $R$ with $p \in R$, we have $R \cap (A \backslash \{p\}) \neq \empty$ .*

Let us prove by contradiction: 

Assume that a subset $A$ of continuum $C$ consists of one point and has a limit point $p$, and because $A$ has only one point, we can assume the set $A = \{p\}$. For a region $R$ to contain a limit point $p$ of $A$, then $A$ must contain elements other than $p$ else  $R \cap (A \backslash \{p\}) \neq \empty$ would be false. Because $A$ contains no other elements than $p$, the intersection would be $\empty$ which indicates that $A$ does not have a limit point. Thus we have proved by contradiction that a subset of a continuum C consisting of one point has no limit points.

**Theorem 3.23: A finite subset $A$ of a continuum $C$ has no limit points.**
A finite subset will contain a region $R$ that is between two points surrounding any point such that the intersection between $R$ and $A$ will be the empty set.


**Corollary 3.24: If $A$ is a finite subset of a continuum $C$ and $x ∈ A$, then there exists a region $R$, containing $x$, such that $A ∩ R = \{x\}$.**
