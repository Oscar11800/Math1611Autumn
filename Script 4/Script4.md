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

Recall the definition of a open set: *a subset $G$ of $C$ is a open set if its complement $C\backslash G$ is clsoed.*

Looking at $\empty$, we can determine if it is open by seeing it its complement is closed. The complement of the $\empty$ can be represented by $C \backslash \empty$ which is equal to $C$. 

According to *theorem 4.2*, the set $C$ contains all elements of the continuum thus it contains all of its limit points and is a closed set. Thus, because its complement is a closed set, then the set $\empty$ is an open set. 

As for the set $C$, we can determine if it is open by observing its complement. The complement of $C$ is the set $\empty$ which can be represented by the statement $C\backslash C = \empty$. 

According to *theorem 4.2*, the empty set is closed because it contains no elements such that it trivially contains its limit points (of which it has none). Thus because its complement, the empty set, is a clsoed set, then the set $C$ is an open set. 

**Theorem 4.9: Let $G \sub C$. Then $G$ is open if and only if for all $x \in G$, there exists a region $R$ such that $x \in R \sub G$.**

**FIX**
First, we can prove that if $G$ is open, then for all $x \in G$, there exists a region $R$ such that $x \in R \sub G$. To do this, we prove by contradiction. Let's assume that $G$ is an open set, but for any arbitrary element $x$ in $G$ there is no region $R$ such that $x \in R \sub G$.

If $G$ is an open set, that means its complement, $C \backslash G$ is a closed set by definition of an open set. Let's assign this closed complement set as $F$. 
**MORE**

Now, we want to prove that if there exists a region $R$ such that $x \in R \sub G$, then $G$ is open. We can also prove this by contradiction by assuming that for some element $x$m there is some region $R$ such that $x \in R \sub G$, but $G is not an open set. If $G$ is not an open set, then it must be a closed set as it is a binary distinction.



**Corollary 4.10: Every region $R$ is open. Every complement of a region $C\backslash R$, is closed.**

**FIX**

We know that from *theorem 4.9*, there exists a region $R$ such that $x \in R \sub G$ and $G \sub C$

To prove that every complement of a region $C\backslash R$ is closed, we can simply look at the definition of an open set: *a subset $G$ of continuum $C$ is open if its complement $C \backslash G* is closed. 

Because we have proven every region $R$ is open, then we know by definition that every complement of the region $R$ is closed.


**Corollary 4.11: Let $G \sub C$. Then $G$ is open if and only if for all $x \in G$, there exists a subset $V \sub G$ such that $x \in V$ and $V$ is open.**


**Corollary 4.12: Let $a\in C$. Then the sets $\{x \in C| x < a\}$ and $\{x \in C| a < x\} are open.**

**Theorem 4.13: Let $G$ be a nonempty set. Then $G$ is the union of a collection of regions**

**Exercise 4.14: Do there exists subsets $X \sub C$ that are neither open nor closed?**


**Theorem 4.15: Let $\{X_\lambda\}$ be an arbitrary collection of closed subsets of a continuum $C$. Then the intersection $\bigcap_\lambda X_\lambda$** is closed.

**Additional Problem 1: Prove that if $S \sub C$ then $\overline{S} = \{x \in C| \textnormal{for all} \; R \; \textnormal{ containing} \; x, R \cap S \neq \empty\}$**

Remember that the closure of $S$ is $\overline{S} = S \cup LP(S)$ which is the union of all elements in $X$ and the limit points of $x$. Let's prove this by contradiction. Assume that if $S \sub C$ then the closure of S is all elements $x \in C$ where for some $R$ containing $x$, $R\cap S = \empty$. 

**Additional Problem 2: Find an example of a continuum $C$ and a subset that is both open and closed, other than $\empty$ and $C$.**

Here is an example: In the continuum of rationals, consider the subset of rationals from $[0,1]$ as the set $A$. We can prove that $A$ is a closed set if it contains all of its limit points. For there to be a limit point $p$ of $A$, then for every region  $R$ where $p \in R$ this must hold true: $R \cap ([0,1] \backslash \{p\}) \neq \empty$.

Here is an example: Let our continuum be the set of natural numbers $\N$, and our subset is set of even natural numbers $\{x\in \N|2n\}$. In this discrete set, the set is closed because as an infinite set, there will be even numbers surrounding