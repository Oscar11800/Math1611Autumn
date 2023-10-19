***<h1 style="text-align: center;">Script 3</h1>***
**Lemma 3.4: If $A$ is a nonempty, finite subset of a continuum $C$, then $A$ has a first and last point.**
We can prove that $A$ has a first and last point through induction.

Suppose our base case $n=1$ , then $A = \{a_1\}$ where $A$ is a set with a single element thus that single element is both the first and last case (according to *definition 3.3*). Now for the inductive hypothesis, we can assume when $n = k$, where $k$ is a positive integer. $A$ has a first element $a_i$ and the last point is $a_k$ such that $a_1 < a_k$. Finally, our inductive step proves our assumption holds for when $A$ contains $n=k+1$ elements. There are three possible cases : 
1. $a_{k+1} < a_1 < a_k $
2. $a_1 < a_{k+1} < a_k$
3. $a_1 < a_k < a_{k+1}$

All these are true for the inductive step and maintain the existence of the first and last element, therefore any finite subset $A$ of a continuum $C$, it has a first and last point.

**Theorem 3.5: Suppose that $A$ is a set of $n$ distinct points in a continuum $C$, or, in other words, $A \sub C$ has cardinality $n$. Then symbols $a_1,...a_n$ may be assigned to each point of $A$ so that $a_1, a_2, <... < a_n, \; ie. \; a_i < a_{i+1} \; for \; 1 \leq i \leq n-1$.**
Suppose we have a set $X$ with elements $\{a_1, a_2, < ... < a_n\}$. We can essentially assign the elements of set $X$ to the first point in $A$ according to *Lemma 3.4* which says that $A$ which is a subset of $C$ has a first and last point. Thus as we move through set $X$, we can assign and remove element $a_1$ from set $A$ so that each element in $A$ will be assigned to symbols $a_1,...a_n$ in set $X$.

**Corollary 3.7: Of three distinct points in a continuum, one must be between the two other.**
Consider *Theorem 3.5* where we proved each point in a subset of a continuum $C$ to a symbol $a_1, a_2,...,a_n$ in ascending order. In this case, points assigned to index $i$ would be less than points $i+1$. 

**Exercise 3.8**: 
**a**. We define a relation $<$ on $\Z$ by $m < n $ if $n = m + c$ for some $c \in \N$. Show that, $\Z$, with the ordering $<$, satisfies *Axion 1-3*. 

Let us be reminded of *Axioms 1-3*.
*Axiom 1. A continuum is a nonempty set $C$.* 
First, let us identify $\Z$ as a continuum because it's a nonempty set . Next, we can identify $m$ and $n$ as distinct points in $\Z$ and $c$ as a positive integer. For *Axiom 1* to prove true, an ordering on the set represented by $\Z \times \Z$ with elements $(m,n)$ written as $m < n$ must satisfy these conditions according to *definition 3.1* . Trichotomy, where for all $m,n \in \Z$ one of the following holds: $m < n, m = n, \; \textnormal{or} \; m > n $. Because we defined $m < n$ if $n = m + c$, then trichotomy is satisfied as one of the above held true.

Next we must prove transitivity for all $m,n,l \in \Z$ so if  $m < n$ and $n < l$ then $m < l$.      

*Axiom 2. A continuum $C$ has an ordering $<$*



*Axiom 3. A continuum $C$ has no first or last point*

**b.** Show that, for any $p = \{\frac a b\} \in \mathbb{Q}$, there is some $(a_1, b_1) \in p$ with $0 < b_1$. 

**c.** We define a relation $<_\mathbb{Q}$ on $\mathbb{Q}$ as follows. For $p, q \in \mathbb{Q}$, let $(a_1,b_1) \in p$ be such that $0 < b_1$, and let $(a_2, b_2) \in q$ be such that $0 < b_2$. Then we define $p <_\mathbb{Q} q$ if $a_1b_2 < a_2b_1$. Show that $<_\mathbb{Q}$ is a well-defined relation on $\mathbb{Q}$. 

**d.** Show that $\mathbb{Q}$, with the ordering $<_\mathbb{Q}$, satisfies *Axioms 1-3*. 
**