***<h1 style="text-align: center;">Script 4</h1>***
**Theorem 4.2: The sets $\empty$ and C are closed.**

A closed set is a set that contains all of its limit points. Remember for there to be a limit point $p$ of $\empty$, then for every region  $R$ where $p \in R$ this must hold true: $R \cap (\empty \backslash \{p\}) \neq \empty$. However, $\empty$ does not contain any elements in its set, therefore $R \cap \empty$ will always be the empty set therefore there are no limit points, and since $\empty$ has no limit points, then the set trivially contains all of its limit points. 

For the set $C$ which contains all elements of the continuum $C$, recall that limit points $p$ must be in $C$, thus $C$ contains all its limit points based on the definition of a limit point. 


**Theorem 4.3: A subset $C$ containing a finite number of   points is closed.**

According to *theorem 3.23: a finite subset $A$ of a continuum $C$ has no limit points*. Similar to the empty set, when a set contains no limit points, then trivially the set contains all its limit points and is closed.


**Theorem 4.5: $X \sub C$ is closed if and only if $X = \overline{X}$.**

The closure of $X$ is $\overline{X} = X \cup LP(X)$ which is the union of all elements in $X$ and the limit points of $x$. 

First we prove that if $X \sub C$ is closed then $X = \overline{X}$. Suppose we have a set $A = LP(X)$. If $X$ is closed, then that means all limit points $LP(X) \in X$ such that $A \sub X$. Because $X$ contains all elements in $A$, we understand that $X \cup A = X$ because there are no elements in $A$ that are not in $X$. Now we have proved $\overline{X} = X \cup LP(X) = X$.

Now we have to prove that if $X = \overline{X}$ then $X \sub C$ is closed. We know that  $\overline{X} = X \cup LP(X)$, so if $X = \overline{X}$, that means $X =X \cup LP(X)$. Because the set $X$ contains all its limit points, then the set $X$ must be closed.


**Theorem 4.6: Let $X \sub C$. Then $\overline{X}$ is closed. (equivalently, $\overline{X} = \overline{\overline{X}})$**

To prove $\overline{X}$ is closed, we need to show $\overline{X}$ contains all of its limit points. 
We want to show $y \in \overline{X}$, so let $y \in LP(\overline{X})$ so $y\in LP(X \cup LP(X))$ which means based on *theorem 3.19* : 
$y \in LP(X)$ which means $y \in \overline{X}$ based on the definition of closure: $\overline{X} = X \cup LP(X)$.

or 

$y \in LP(LP(x))$ where we let $R_1$ is a region that contains $y$ where $y \in R$ and we want to show $R_1 \cap(X\backslash\{y\} \neq \empty)$. We know that $R_1 \cap(X\backslash\{y\} \neq \empty)$ for all regions $R$ that $y\in R$. Let $Z \in R_1 \cap (LP(X) \backslash \{y\})$ where $z \in LP(X)$which means tha $z \in R_1$ and $z \in LP(X) \backslash\{y\}$. We can then say that $R_1 \cap(X\backslash\{y\} \neq \empty)$. Now, let $a \in R_1 \cap(X\backslash\{y\})$.

case 1: $a \neq y$ which means $R_1 \cap x \backslash \{y\} \neq \empty$. 

case 2: $a = y$ which means $y \in R_1 \cap(x \backslash \{z\})$ and by *theorem 3.21*, $y\in R_2$, $z \in R_3$, and $R_2 \cap R_3 = \empty$.
We can surmise that $z \in R_1 \cap R_3$ such that $(R_1 \cap R_3) \cap (x \backslash \{z\} \neq \empty)$. Let $b \in (R_1 \cap R_3) \cap (x \backslash \{z\}$ which means $b \in R_1 \cap R_3$ and $b\in X$ and $b \in R_1 \cap (x \backslash \{y\})$ such that $y \in LP(X)$ which means $y \in \overline{X}$ and because all $LP(\overline{X} \sub X)$ then $\overline{X}$ is closed.  

**Theorem 4.8: The sets $\empty$ and $C$ are open.**

Recall the definition of an open set: A subset $G$ of $C$ is an open set if its complement $C \setminus G$ is closed.

We want to show that the empty set $\emptyset$ is open by demonstrating that its complement is closed. The complement of $\emptyset$ can be represented as $C \setminus \emptyset$, which is equivalent to $C$.

By Theorem 4.2, we know that the set $C$ contains all elements of the continuum, including its limit points, and is therefore a closed set.
Thus, because the complement of $\emptyset$ (which is $C$) is a closed set, $\emptyset$ is indeed an open set.

Similarly, we want to establish that the entire continuum $C$ is an open set by observing its complement. The complement of $C$ is the empty set, which can be represented by the statement $C \setminus C = \emptyset$.

Again, referring to Theorem 4.2, the empty set is closed because it contains no elements, and it trivially contains its limit points (of which it has none).Therefore, because the complement of $C$ (which is $\emptyset$) is a closed set, we can conclude that $C$ is an open set.

Hence, both the empty set $\emptyset$ and the entire continuum $C$ are open sets.


**Theorem 4.9: Let $G \sub C$. Then $G$ is open if and only if for all $x \in G$, there exists a region $R$ such that $x \in R \sub G$.**

Contrapositive:If for some $x \in G$, all regions $R$ containing $x$ are not subsets of $G$, then $G$ is not open. We know that $R \not\sub G$ which means there some elements of $R$ are in $C\backslash G$. 

Therefore there is some $x$ that is the limit point of $C \backslash G$ for all $R$ containing some $x$, $R \cap (C \backslash G \backslash \{x\}) \neq 0$ where $x \not\in C \backslash G$. Thus the complement of $G$ is not closed because it does not contain all of its limit points, thus we know that 


If for all $x \in G$ there exists a region $R$, such that $x$ is an element of $R$ such that $R \sub G$, then $G$ is open

Contrapositive: If $G$ is not open, then for some $x$ in $G$, for all regions $R$ containing $x$, $R \not\sub G$. If $G$ is not open, by theorem 4.2, then the complement of $G$ is not closed which means the complement does not contain all of its limit points. Let $x \in LP(C \backslash G)$ and $x \in G$. Therefore, there exists for all regions $R$ such that $x \in R$, $R$ contains elements of $C \backslash G$ because $R \cap G\backslash x \neq \empty$. Therefore $R$ is not subset of $G$ because it contains elements not in $G$.


**Corollary 4.10: Every region $R$ is open. Every complement of a region $C\backslash R$, is closed.**

First, we want to prove that every region $R$ is open. For all elements $x$ of the region $R$, $R$ is itself a region such that $x \in R$ and $R \sub R$. By *theorem 4.9 *there exists a region $R$ such that $x \in R \sub G$ and $G \sub C$, $R$ is  open.

Since all $R$ are open, then by definition of an open set, all $C \backslash R$ are closed. 


**Corollary 4.11: Let $G \sub C$. Then $G$ is open if and only if for all $x \in G$, there exists a subset $V \sub G$ such that $x \in V$ and $V$ is open.**

We want to show that iff $G$ is open, then for all elements $x \in G$, there exists a subset $V$ such that $x \in V \sub G$ and $V$ is an open set. 

First, we assume that $G$ is open, then  by *theorem 4.9*, for all $x \in G$ there exists an $R$ such that $x \in R$ and $R \sub G$. Let's set $V = R$ so that $x \in V$ and consequently $V \sub G$. By theorem 4.10, because $R$ is a region and it is open, thus $V$ is also open. We have prove that $V \sub G$, $V$ contains $R$, and $V$ is also open

For all elements $x \in G$, there is a subset $V$ that is open and $x \in V \sub G$. We want to prove that $G$ is open. We know that for all $x$, there exists an $R$ such that $x \in R \in V$ and because $R \sub V$ and $V \sub G$, then $R \sub G$, and it also stands that for all $x \in R$, that $x \in R \sub G$ and by theorem 4.9, $G$ is open. 


**Corollary 4.12: Let $a\in C$. Then the sets $\{x \in C| x < a\}$ and $\{x \in C| a < x\}$ are open.**

Let $a \in C$, so that the sets $\{x \in C| x < a\}$ and $\{x \in C | x >a\}$. Let's let some region $R = \underline{ka}$ where $k$ is an arbitary point on $C$ such that it is less than $x$. $k$ must exist because $C$ does not have a first point. For all $x \in \{x \in C| x < a\}$, the region $R$ both contains $a$ and $R \sub \{x \in C| x < a\}$ thus by theorem 4.9, $\{x \in C| x < a\}$ is open.

For the other region $\{x \in C | x >a\}$, if we let $S= \underline{am}$ where $m$ is a point on $C$, which exists because $C$ doesn't have a last point. For all $\{x \in C | x >a\}$, $S$ contains $x$ and $S \sub \{x \in C | x >a\}$, thus by theorem 4.9, $\{x \in C | x >a\}$ is open. 

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


**Exercise 4.24: Let $C$ be a connected continuum and $a ∈ C$. Prove that $C \backslash \{a\} $is a disconnected continuum.**