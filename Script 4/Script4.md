***<h1 style="text-align: center;">Script 4</h1>***
**Theorem 4.2: The sets $\empty$ and C are closed.**

To prove that a set is closed, we must show that it contains all of its limit points. By definition a limit point of set $S$ is a point $p$ if for every region $R$ of $C$ containing $p$ such that $p \in R$, the region $R$ intersects with $S$ at some point other than $p$, more formally $R \cap S \backslash \{p\} \neq \empty$.

First let us prove that $\empty$ is closed: 
The set $\empty$ does not contain any elements in its set, therefore $R \cap \empty$ will always be the empty set therefore there are no limit points, and since $\empty$ has no limit points, then the set trivially contains all of its limit points. 

Now let us prove that the set $C$ is closed:
The set $C$ contains all points of the continuum $C$ which means it also includes all limit points $p$. Because all limit points $p$ must be in $C$ for it to be closed, then $C$ is closed by definition of a closed set.


**Theorem 4.3: A subset $C$ containing a finite number of points is closed.**

According to *Theorem 3.23*, a finite subset $A$ of a continuum $C$ has no limit points. We will use this fact to prove that $C$ is closed.

Since $C$ is finite, let's consider any point $p\in R$. There are two possibilities:

$p$ is an element of $C$: Since $C$ is finite, there exists a region $R$ containing $p$ that does not contain any other points of $C$ by *corollay 3.23*. Thus, $p$ is not a limit point of $C$ by definition of a limit point.

$p$ is not an element of $C$: In this case, $p$ cannot be a limit point of $C$ because there exists a region $R$ containing $p$ that does not intersect $C$ at any point other than possibly $p$ itself (if $p$ was in $C$, which it is not).

In both cases, $p$ is not a limit point of $C$. Since $C$ has no limit points, it trivially contains all of its limit points. Therefore, $C$ is closed.

**Theorem 4.5: $X \sub C$ is closed if and only if $X = \overline{X}$.**

The closure of $X$ is $\overline{X} = X \cup LP(X)$ which is the union of all elements in $X$ and the limit points of $x$. 

**(⇒) If \( X \) is closed, then \( X = \overline{X} \):**

Assume \( X \subseteq C \) is closed. By definition, a closed set contains all its limit points. Let \( A = LP(X) \). Since \( X \) is closed, it follows that \( A \sub X \). Therefore, \( X \cup A = X \) because \( A \) does not contain any elements that are not already in \( X \). Hence, \( \overline{X} = X \cup LP(X) = X \), which shows that if \( X \) is closed, then \( X \) is equal to its closure.

**(⇐) If \( X = \overline{X} \), then \( X \) is closed:**

Assume \( X = \overline{X} \). By the definition of closure, \( \overline{X} \) includes \( X \) and all limit points of \( X \), that is, \( \overline{X} = X \cup LP(X) \). If \( X = \overline{X} \), then \( X \) must contain all its limit points because \( \overline{X} \) contains all limit points of \( X \) by definition. Therefore, \( X \) is closed because a set is closed if and only if it contains all its limit points.

Thus, we have shown both directions of the equivalence: \( X \) is closed if and only if \( X = \overline{X} \). 


**Theorem 4.6: Let $X \sub C$. Then $\overline{X}$ is closed. (equivalently, $\overline{X} = \overline{\overline{X}})$**

To prove that \( \overline{X} \) is closed, we must show that it contains all of its limit points. Let \( y \) be a limit point of \( \overline{X} \), so \( y \in LP(\overline{X}) \). By the definition of closure, \( \overline{X} = X \cup LP(X) \). We need to show that \( y \in \overline{X} \).

Since \( y \) is a limit point of \( \overline{X} \), for every region \( R_1 \) containing \( y \) such that $y \in R_1$, the intersection \( R_1 \cap (\overline{X} \setminus \{y\}) \) is non-empty. This means there exists some point \( z \in R_1 \cap (\overline{X} \setminus \{y\}) \). Since \( \overline{X} = X \cup LP(X) \), it follows that \( z \) is either in \( X \) or is a limit point of \( X \).

In either case, \( z \) is in \( \overline{X} \), and since \( z \) is distinct from \( y \), we have shown that every region containing \( y \) intersects \( \overline{X} \) at some point other than \( y \). Therefore, \( y \) must be in \( \overline{X} \), and since \( y \) was an arbitrary limit point of \( \overline{X} \), it follows that \( \overline{X} \) contains all of its limit points.


**Theorem 4.8: The sets $\empty$ and $C$ are open.**

Recall the definition of an open set: A subset \( G \) of \( C \) is an open set if its complement \( C \setminus G \) is closed.

First, consider the empty set \( \emptyset \). The complement of \( \emptyset \) in \( C \) is \( C \setminus \emptyset \), which is simply \( C \). By *Theorem 4.2*, \( C \) is closed because it contains all its limit points, as it is the entire space. Therefore, since the complement of \( \emptyset \) is closed, \( \emptyset \) itself is open.

Next, consider the entire continuum \( C \). The complement of \( C \) within itself is \( C \setminus C \), which is \( \emptyset \). As established above by *Theorem 4.2*, \( \emptyset \) is closed. Hence, the complement of \( C \) is closed, which implies that \( C \) is open.

Thus, we have shown that both \( \emptyset \) and \( C \) are open sets.


**Theorem 4.9: Let $G \sub C$. Then $G$ is open if and only if for all $x \in G$, there exists a region $R$ such that $x \in R \sub G$.**
(class notes)
$=>$ Contrapositive:If for some $x \in G$, all regions $R$ containing $x$ are not subsets of $G$, then $G$ is not open. We know that $R \not\sub G$ which means there some elements of $R$ are in $C\backslash G$. 

Therefore there is some $x$ that is the limit point of $C \backslash G$ for all $R$ containing some $x$, $R \cap (C \backslash G \backslash \{x\}) \neq 0$ where $x \not\in C \backslash G$. Thus the complement of $G$ is not closed because it does not contain all of its limit points. Based on the definition of an open set, we now know that $G$ is open because its complement is closed. We have thus proved if for all $x \in G$ there exists a region $R$, such that $x$ is an element of $R$ such that $R \sub G$, then $G$ is open

$<= $ Contrapositive: If $G$ is not open, then for some element $x$ in $G$, for all regions $R$ containing $x$, $R \not\sub G$. If $G$ is not open, by *theorem 4.2*, then the complement of $G$ is not closed which means the complement does not contain all of its limit points. Let $x \in LP(C \backslash G)$ and $x \in G$. Therefore, there exists for all regions $R$ such that $x \in R$, $R$ contains elements of $C \backslash G$ because $R \cap G\backslash x \neq \empty$. Therefore $R$ is not subset of $G$ because it contains elements not in $G$.


**Corollary 4.10: Every region $R$ is open. Every complement of a region $C\backslash R$, is closed.**

Let \( R \) be a region in \( C \). By the definition of a region, for every point \( x \in R \), there exists an open interval \( (a, b) \) such that \( x \in (a, b) \subseteq R \). This open interval \( (a, b) \) serves as the region required by *Theorem 4.9* to conclude that \( R \) is open. Therefore, every region \( R \) is open.

Now, consider the complement of a region \( C \setminus R \). Since \( R \) is open, its complement \( C \setminus R \) must be closed. This is because the definition of an open set \( R \) is such that its complement \( C \setminus R \) is closed.

Hence, every region \( R \) is open, and every complement of a region \( C \setminus R \) is closed.


**Corollary 4.11: Let $G \sub C$. Then $G$ is open if and only if for all $x \in G$, there exists a subset $V \sub G$ such that $x \in V$ and $V$ is open.**

**(⇒ Direct)** Assume \( G \) is open. By *theorem 4.9*, for every \( x \in G \), there exists a region \( R \) such that \( x \in R \sub G \). Since every region is open by Corollary 4.10, we can choose \( V = R \) such that $V sub G$ is also open and $x\in V$. Hence, for every \( x \in G \), there exists an open subset \( V \sub G \) containing \( x \).

**(⇐ Converse)** Assume that for every \( x \in G \), there exists an open subset \( V \sub G \) such that \( x \in V \). We want to prove that $G$ is open. We know that for all $x$, there exists an $R$ such that $x \in R \in V$ and because $R \sub V$ and $V \sub G$, then $R \sub G$, and it also stands that for all $x \in R$, that $x \in R \sub G$ and by *theorem 4.9*, thus $G$ is open. 


Therefore, \( G \) is open if and only if for every \( x \in G \), there exists an open subset \( V \sub G \) containing \( x \).


**Corollary 4.12: Let $a\in C$. Then the sets $\{x \in C| x < a\}$ and $\{x \in C| a < x\}$ are open.**

Let $a \in C$, so that the sets $\{x \in C| x < a\}$ and $\{x \in C | x >a\}$. Let's let some region $R = \underline{ka}$ where $k$ is an arbitary point on $C$ such that it is less than $x$. $k$ must exist because $C$ does not have a first point. For all $x \in \{x \in C| x < a\}$, the region $R$ both contains $a$ and $R \sub \{x \in C| x < a\}$ thus by theorem 4.9, $\{x \in C| x < a\}$ is open.

For the other region $\{x \in C | x >a\}$, if we let $S= \underline{am}$ where $m$ is a point on $C$, which exists because $C$ doesn't have a last point. For all $\{x \in C | x >a\}$, $S$ contains $x$ and $S \sub \{x \in C | x >a\}$, thus by theorem 4.9, $\{x \in C | x >a\}$ is open.

___

Given the point $a \in C$, consider the set \( L = \{x \in C \mid x < a\} \). Take any point \( x \in L \). Since \( C \) is a continuum without a first point by *axiom 3*, there exists a point \( k \in C \) such that \( k < x \). Similarly, since \( x < a \), we can find a region \( R \) such that \( k < x \) and \( x < a \) are both in \( R \), and \( R \subseteq L \). By *Theorem 4.9*, which states that a set is open if for every point there exists a region contained within the set, \( L \) is open.

Now consider the set \( U = \{x \in C \mid a < x\} \). For any point \( x \in U \), since \( C \) does not have a last point, there exists a point \( m \in C \) such that \( x < m \). We can then find a region \( S \) such that \( a < x \) and \( x < m \) are both in \( S \), and \( S \subseteq U \). Again, by Theorem 4.9, \( U \) is open.

Therefore, both \( \{x \in C \mid x < a\} \) and \( \{x \in C \mid a < x\} \) are open sets.

**Theorem 4.13: Let $G$ be a nonempty open set. Then $G$ is the union of a collection of regions.**

Each point $x$ in $G$ has a region $R_x$ such that $x \in R_x \sub G$ and the regions depends on its respective $x$ by theorem 4.9. $\bigcap_{x \in G}R_x \sub G$ and $G \sub \bigcap_{x \in G}R_x$ because any point $x$ in $G$ is in one of the regions $R_x$ such that $\bigcap_{x \in G}R_x = G$.

**Exercise 4.14: Do there exists subsets $X \sub C$ that are neither open nor closed?**

Yes, there exists a subset $X \sub C$ that is neither open nor closed. Consider the set $X = \{1/x| x \in \N\}$ such that $1/1, 1/2, 1/3$ where $A \sub \mathbb{Q}$. $A$ is not open because there is no region $R$ such that $1/1$ is in $R$ and $R \sub A$. $A$ is not closed because $0$ is a limit point of $A$, but $0$ is not contained in $A$. Thus $A$ is neither open nor closed. 


**Theorem 4.15: Let $\{X_\lambda\}$ be an arbitrary collection of closed subsets of a continuum $C$. Then the intersection $\bigcap_\lambda X_\lambda$ is closed.**



**Theorem 4.16: Let $\{G_\lambda\}$ be an arbitrary collection of open subsets of a continuum $C$. Then the union $\bigcup_\lambda G_\lambda$ is open.**

Let us assign the union of open subsets $\bigcup_\lambda G_\lambda$ as set $G$. Here, we are trying to prove that the set $G$ is open if all open subsets $G_\lambda$ are open and such that for all $x \in G$, $x \in G_\lambda$. 

Remember *theorem 4.11* which stated *that set $G$ is open if and only if for all $x \in G$, there exists a subset $V \sub G$ such that $x \in V$ and $V$ is open.* Because for all elements of $x in \bigcup_\lambda G_\lambda$ the subsets $G_\lambda$ include elements $x$ by definition 1.14 which defined $x$ to be elements of a subset $G_\lambda$ for all $\lambda \in I$ where $I$ is an nonempty set, and subsets $G_\lambda$ are given to be open, then by satisfying all conditions of *theorem 4.11*, the union $\bigcup_\lambda G_\lambda$ is open.


**Theorem 4.17: Let $\{G_1...,G_n\}$ be a finite collection of open subsets of a continuum $C$. Then the intersection $G_1 \cap ... \cap G_n$ is open.**

We want to show that the intersection of the finite open sets is open. The intersection of the open subsets can be represented as $\bigcap_n G_n$ where $n \in \N$. For all $x$ in the intersection, $x \in$ each of the sets $G_n$. Then for all $n$, there exists an individual $R_n$ that contains $x$ such that $x \in R_n \sub G$ by *theorem 4.9*.

*Theorem 3.18:If $n$ regions $R_1,..., R_n$ have a point $x$ in common, then their intersection $R_1 \cup ... \cap R_n$ is a region containing $x$*, therefore there exists a region in the intersection of finite open sets called $R_{inter} = \bigcap_nR_n$. Thus $R_{inter}$ for all $n$, $R_n \sub G_n$, $R_{inter} \sub R_n \sub G_n$. Which means $R_{inter} \sub \bigcap_n G_n$.



**Corollary 4.18: Let $X_1,..., X_n$ be a finite collection of closed subsets of a continuum $C$. Then the union $X_1\cup ... \cup X_n$ is closed.**
We know  that $C \backslash X$ is open for all $i$. By *theorem 4.17* we know that the intersection of $C\backslash X_i$ is open as well so that $\bigcap_n C \backslash X_i$. By *theorem 1.15*, we know that $C \backslash \bigcap_n C \backslash X_i = \bigcup_n C \backslash (C \backslash X_i) = \bigcup_n X_i$ this is because the complement of open is closed.

**OR, bottom is mine**

By *theorem 1.15*, the complement of an intersection of a collection of sets is equal to the union of the complements of each set in the collection represented by $X\backslash (\bigcap_\lambda G_\lambda) = \bigcup_\lambda (X \backslash G_\lambda)$. Remember that the complement of an open set is, by definition, a closed set. Thus, we know that the complement of the finite collection of open subsets which form an open intersection of sets in *theorem 4.17* is the union of closed sets $X_1 \cup... \cup X_n$.

**Exercise 4.19: Is it necessarily the case that the intersection of an infinite number of open sets is open? Is it possible to construct an infinite collection of open sets whose intersection is not open? Equivalently, is it possible to construct an infinite collection of closed sets whose union is not closed?**

1. Yes, it is possible to construct an infinite collection of open sets whose intersection is not open. For example, construct a set $A = \bigcap_n \underline{(- \frac a n)(\frac 1 n)}$ in the continuum $\mathbb{Q}$ where $A \sub Q$ and $n \in N$. It follows that $A = \bigcap_n \underline{(- \frac a n)(\frac 1 n)} = \{0\}$ because $0$ is the only point contained in the intersection of all these regions as $n$ goes towards infinity. For each set $\underline{(- \frac a n)(\frac 1 n)}$ is a region and therefore open by *corollary 4.10* which states regions are open. However, because $A = \{0\}, there exists no region $R$ such that $0 \in R \sub A$. Therefore, $A$ is not open by *theorem 4.9*.

2. Yes, it is possible to construct an infinite collection of closed sets whose union is not closed. Consider set $B = \bigcup_n \{\frac 1 n\}$ where $n \in N$ in the continuum $\mathbb{Q} and $B \sub \mathbb{Q}$. For all $n \in \N$, each set $\{\frac 1 n\} is finite and therefore closed. However, $0$ is not in $B$, and $0$ is a limtit point of $B$. Thus $B$ is not closed due to *definition 4.1*. 

**Corollary 4.20: Let $G \sub C$ be nonempty. Then $G$ is open if and only if $G$ is the union of a collection of regions.**

1. assume $G$ is opeen, then by *theorem 4.9*, for all $x \in G$ there exists a region containing $x$ that is entirely contained by $G$. The union of all such regions contains all $x \in G$ which means that $G \sub \bigcup_n R_n$ where $n \in \N$. So $\bigcup_n R_n \sub G$ which means that $\bigcup_ R_n = G_n$.

2. We can assume that $G = \bigcup_n R_n$ and we want to show that $G$ is open. Since we know that all regions $R_n$ are open by *theorem 4.10*, then because $G$ is a union of open subsets, then it must be open.

**MINE BELOW**

We want to show that if $G$ is a nonempty, open set, then $G$ is the union of a collection of regions. We proved this in *theorem 4.13: $G$ be a nonempty open set. Then $G$ is the union of a collection of regions* because any point $x$ in $G$ is in one of the regions $R_x$ which corresponded to its respective $x$ such that $\bigcap_{x \in G}R_x = G$.

Now, let's show that if $G$ is the union of a collection of regions, then $G$ is open. By *theorem 4.9: $G$ is open if and only if for all $x \in G$, there exists a region $R$ such that $x \in R \sub G$.* Because $G$ is open, then for every $x$ in $G$, there is a region $R_x$ such that $x \in R_x \sub G$. Thus, let's make each region $R_x$, which corresponds to its respective $x$, as a subset $V_x \sub G$ which contains only its respective $x$. By *corollary 4.11: $G$ is open if and only if for all $x \in G$, there exists a subset $V \sub G$ such that $x \in V$ and $V$ is open*, thus $G$ is open because for all $x$ in $G$, there is a $V_x$ such that $x \in V_x$ and $V$ is open.


**Corollary: 4.21: If $\underline{ab}$ is a region of $C$, then ext $\underline{ab}$ is open.**

If $\underline{ab} is a region in continuum $C$, then the ext $\underline{ab} is open. By *theorem 3.14* $C \backslash (\{a\} \cup \underline{ab} \cup \{b\}) = ext \underline{ab}$. If ext $\underline{ab}$ is open, then by *theorem 4.7*, $C \backslash$ ext $\underline{ab} = \{a\} \cup \underline{ab} \cup \{b\}$ is closed.

We want to show that there is no $x$ such that $x$ is a limit point of $\{a\} \cup \underline{ab} \cup \{b\}$ and $x \not\in \{a\} \cup \underline{ab}$.

Suppose there exists some $d$ such that $d$ is a potential limit point of $\underline{ab}$ and $d < a$. Then by *axiom 3 of continuums* there exists a $z$ such that $z < d$. Now suppose there is at least one element $q$ such that $d < q < a$ which means there exists a region $\underline{za}$ such that $\underline{za} \cap (\{a\} \cup \underline{ab} \{b\} \backslash \{d\} = \empty$. Therefore $d$ is not a limit point of $\{a\} \cup \underline{ab} \cup \{b\}.

**YOU CAN USE 4.12 instead**

**Theorem 4.23: Let $C$ be a connected continuum. Let $x$, $y ∈ C$, with $x < y$. Then there exists $z ∈ C$ such that $x < z < y$.**

Let's solve this by contradiction. Assume there does not exist an element $z \in C$ such that $x < z < y$. By *corollary 4.12*, which states that for any element $a \in C$ and $x \in G \sub C$, the sets $\{x\in C| x \leq a\}$ and $\{x \in C| a <x \}$ are open. Therefore, we can represent $C$ as the union of sets $A$ and $B$ where $a\in A \sub C$ and $A = \{a \in C| a <y\}$ and $b \in B \sub C$ and $B = \{b \in C | b > y\}$ (notice we don't use $z$ because it does not exist).

Also, we know that $A$ and $B$ are nonempty because $x \in A$ and $y \in B$.

Moreover, $A$ and $B$ are disjoint: $\overline{A} \cap B = A \cap \overline{B} = \empty$. This is because $x < y$ and every point in $A$ is less than or equal to $x$ and every point in $B$ is greater than or equal to $y$ which is true by *axiom 2* stating that continuums have an ordering $<$, and in this case there is no point in $C$ that is greater than or equal to $y$ and less than or equal to $x$ therefore the sets $A$ and $B$ are disjoint: $A \cap B = \empty$.

The existence of disjoint, nonempty open sets $A$ and $B$ such that $C = A \cup B$ means that $C$ is disconnected by definition which is a contradiction which means our assumption is false. Thus, there must a point $z \in C$ such that $x < z < y$ for $C$ to b a connected continuum.


**Exercise 4.24: Let $C$ be a connected continuum and $a ∈ C$. Prove that $C \backslash \{a\} $is a disconnected continuum.**

We know that the continuum $C\backslash \{a\}$ is a continuum because it fulfills the axioms:
1. it is nonempty
2. it has a well defined ordering
3. it has no first nor last point

To prove that $C\backslash \{a\}$ is disconnected, we want to show that $C \