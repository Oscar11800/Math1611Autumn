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

Therefore there is some $x$ that is the limit point of $C \backslash G$ for all $R$ containing some $x$, $R \cap (C \backslash G \backslash \{x\}) \neq 0$ where $x \not\in C \backslash G. Thus the complement of $G$ is not closed because it does not contain all of its limit points, thus we know that 


If for all $x \in G$ there exists a region $R$, such that $x$ is an element of $R$ such that $R \sub G$, then $G$ is open

Contrapositive: If $G$ is not open, then for some $x$ in $G$, for all regions $R$ containing $x$, $R \not\sub G$. If $G$ is not open, by theorem 4.2, then the complement of $G$ is not closed which means the complement does not contain all of its limit points. Let $x \in LP(C \backslash G)$ and $x \in G$. Therefore, there exists for all regions $R$ such that $x \in R$, $R$ contains elements of $C \backslash G$ because $R \cap G\backslash x \neq \empty$. Therefore $R$ is not subset of $G$ because it contains elements not in $G$.


**Corollary 4.10: Every region $R$ is open. Every complement of a region $C\backslash R$, is closed.**

First, we want to prove that every region $R$ is open. For all elements $x$ of the region $R$, $R$ is itself a region such that $x \in R$ and $R \sub R$. By *theorem 4.9 *there exists a region $R$ such that $x \in R \sub G$ and $G \sub C$, $R$ is  open.

Since all $R$ are open, then by definition of an open set, all $C \backslash R$ are closed. 


**Corollary 4.11: Let $G \sub C$. Then $G$ is open if and only if for all $x \in G$, there exists a subset $V \sub G$ such that $x \in V$ and $V$ is open.**

We want to show that iff $G$ is open, then for all elements $x \in G$, there exists a subset $V$ such that $x \in V \sub G$ and $V$ is an open set. 

First, we assume that $G$ is open, then  by *theorem 4.9*, for all $x \in G$ there exists an $R$ such that $x \in R$ and $R \sub G$. Let's set $V = R$ so that $x \in V$ and consequently $V \sub G$. By theorem 4.10, because $R$ is a region and it is open, thus $V$ is also open. We have prove that $V \sub G$, $V$ contains $R$, and $V$ is also open

For all elements $x \in G$, there is a subset $V$ that is open and $x \in V \sub G$. We want to prove that $G$ is open. We know that for all $x$, there exists an $R$ such taht $x \in R \in V$ and because $R \sub V$ and $V \sub G$, then $R \sub G$, and it also stands that for all $x \in R$, that $x \in R \sub G$ and by theorem 4.9, $G$ is open. 


**Corollary 4.12: Let $a\in C$. Then the sets $\{x \in C| x < a\}$ and $\{x \in C| a < x\}$ are open.**

Let $a \in C$, so that the sets $\{x \in C| x < a\}$ and $\{x \in C | x >a\}$. Let's let some region $R = \underline{ka}$ wheere $k$ is an arbitary point on $C$ such that it is less than $x$. $k$ must exist because $C$ does not have a first point. For all $x \in \{x \in C| x < a\}$, the region $R$ both contains $a$ and $R \sub \{x \in C| x < a\}$ thus by theorem 4.9, $\{x \in C| x < a\}$ is open.

For the other region $\{x \in C | x >a\}$, if we let $S= \underline{am}$ where $m$ is a point on $C$, which exists because $C$ doesn't have a last point. For all $\{x \in C | x >a\}$, $S$ contains $x$ and $S \sub \{x \in C | x >a\}$, thus by theorem 4.9, $\{x \in C | x >a\}$ is open. 

**Theorem 4.13: Let $G$ be a nonempty open set. Then $G$ is the union of a collection of regions**

Each point $x$ in $G$ has a region $R_x$ such that $x \in R_x \sub G$ and the regions depends on its respective $x$ by theorem 4.9. $\bigcap_{x \in G}R_x \sub G$ and $G \sub \bigcap_{x \in G}R_x$ because any point $x$ in $G$ is in one of the regions $R_x$ such that $\bigcap_{x \in G}R_x = G.

**Exercise 4.14: Do there exists subsets $X \sub C$ that are neither open nor closed?**


**Theorem 4.15: Let $\{X_\lambda\}$ be an arbitrary collection of closed subsets of a continuum $C$. Then the intersection $\bigcap_\lambda X_\lambda$** is closed.

**Additional Problem 1: Prove that if $S \sub C$ then $\overline{S} = \{x \in C| \textnormal{for all} \; R \; \textnormal{ containing} \; x, R \cap S \neq \empty\}$**

We want to prove that if \(S \sub C\), then \(\overline{S} = \{x \in C \,|\, \text{for all } R \text{ containing } x, R \cap S \neq \emptyset\}\).

By Definition 3.12, a limit point in a continuum \(C\) for a subset \(A\) is a point \(p\) in \(A\) such that every region \(R\) containing \(p\) has a non-empty intersection with \(A \setminus \{p\}\). Thus, for every region \(R\) with \(p \in R\), we have \(R \cap (A \setminus \{p\}) \neq \emptyset\).

Now, let's establish the relationship between limit points and the closure of a set \(S\) by considering the definition of closure: \(\overline{S}\) includes all limit points of \(S\) as well as elements of \(S\).

Now, let's prove the desired equality:

 1: \(\overline{S} \sub \{x \in C \,|\, \text{for all } R \text{ containing } x, R \cap S \neq \emptyset\}\)

Suppose \(x \in \overline{S}\). By the definition of closure, \(x\) is either in \(S\) or a limit point of \(S\).

- If \(x\) is in \(S\), then for any region \(R\) containing \(x\), \(R \cap S \neq \emptyset\) because \(x\) is in \(S\).

- If \(x\) is a limit point of \(S\), then for any region \(R\) containing \(x\), \(R \cap (S \setminus \{x\}) \neq \emptyset\) by Definition 3.12. However, \(R \cap (S \setminus \{x\})\) is the same as \(R \cap S\) because removing \(x\) from \(S\) doesn't affect the intersection. Therefore, \(R \cap S \neq \emptyset\).

In both cases, we have shown that for any \(R\) containing \(x\), \(R \cap S \neq \emptyset\).

2: \(\{x \in C \,|\, \text{for all } R \text{ containing } x, R \cap S \neq \emptyset\} \subseteq \overline{S}\)

Now, suppose \(x\) satisfies the property: for all regions \(R\) containing \(x\), \(R \cap S \neq \emptyset\).

We want to show that $x \in \overline{S}$. By the definition of closure, we need to demonstrate that $x$ is either in $S$ or a limit point of $S$.

- If \(x\) is in \(S\), then it's trivially in \(\overline{S}\).

- If \(x\) is not in \(S\), then it must be a limit point of \(S\) because for all regions \(R\) containing \(x\), \(R \cap S \neq \emptyset\). This satisfies the definition of a limit point.

Therefore, we have shown both inclusions, and we can conclude that \(\overline{S} = \{x \in C \,|\, \text{for all } R \text{ containing } x, R \cap S \neq \emptyset\}\).



**Additional Problem 2: Find an example of a continuum $C$ and a subset that is both open and closed, other than $\empty$ and $C$.**

Let \(C\) be the continuum of natural numbers, denoted as \(C = \mathbb{N}\), and consider the set of even natural numbers, \(A = \{x \in \mathbb{N} \,|\, x = 2n\}\).

   We want to show that \(A\) is both open and closed. First, let's address the limit points.

   By Definition 3.12, a limit point in continuum \(C\) for a subset \(A\) is a point \(p\) in \(A\) such that every region \(R\) containing \(p\) has a non-empty intersection with \(A\setminus\{p\}\). Formally, for every region \(R\) with \(p \in R\), we have \(R \cap (A \setminus \{p\}) \neq \emptyset\).

   - Consider a point \(p\) in \(A\). If \(p\) is an even number, it has odd neighbors in \(\mathbb{N}\) that are not in \(A\). These odd neighbors ensure that \(p\) is indeed a limit point of \(A\) because for any region \(R\) containing \(p\), \(R \cap (A \setminus \{p\}) \neq \emptyset\). This is because \(R\) will include both even and odd numbers.

   To establish that \(A\) is both open and closed, we will show that its complement in \(C\), which is the set of odd numbers, is closed, and that \(A\) is open.

   - Closed Set: The set of odd numbers in \(C\) is its complement, denoted as \(A^c = \{x \in \mathbb{N} \,|\, x = 2n + 1\}\). Just as we showed for \(A\), the set of odd numbers is also a closed set because each odd number has even neighbors, making it a limit point of itself. Therefore, \(A^c\) is closed.

   - Open Set: To show that \(A\) is open, we can use the fact that an open set is defined as a set whose complement is closed. Since we have established that \(A^c\) is closed, \(A\) must be open.

Therefore, we have proven that the set of even numbers, \(A\), in the continuum of natural numbers, \(\mathbb{N}\), is both open and closed.