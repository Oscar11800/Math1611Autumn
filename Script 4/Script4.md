***<h1 style="text-align: center;">Script 4</h1>***
**Theorem 4.2: The sets $\empty$ and C are closed.**

To prove that a set is closed, we must show that it contains all of its limit points. By definition a limit point of set $S$ is a point $p$ if for every region $R$ of $C$ containing $p$ such that $p \in R$, the region $R$ intersects with $S$ at some point other than $p$, more formally $R \cap S \backslash \{p\} \neq \empty$.

First let us prove that $\empty$ is closed: 
The set $\empty$ does not contain any elements in its set, therefore $R \cap \empty$ will always be the empty set therefore there are no limit points, and since $\empty$ has no limit points, then the set trivially contains all of its limit points. 

Now let us prove that the set $C$ is closed:
The set $C$ contains all points of the continuum $C$ which means it also includes all limit points $p$. Because all limit points $p$ must be in $C$ for it to be closed, then $C$ is closed by definition of a closed set.


**Theorem 4.3: A subset $C$ containing a finite number of points is closed.**

According to *Theorem 3.23*, a finite subset $A$ of a continuum $C$ has no limit points. Since $C$ has no limit points, it trivially contains all of its limit points. Therefore, $C$ is closed.


**Theorem 4.5: $X \sub C$ is closed if and only if $X = \overline{X}$.**

The closure of $X$ is $\overline{X} = X \cup LP(X)$ which is the union of all elements in $X$ and the limit points of $x$.

**(⇒) If \( X \) is closed, then \( X = \overline{X} \):**

Assume \( X \sub C \) is closed. By definition, a closed set contains all its limit points. Let \( A = LP(X) \). Since \( X \) is closed, it follows that \( A \sub X \). Therefore, \( X \cup A = X \) because \( A \) does not contain any elements that are not already in \( X \). Hence, \( \overline{X} = X \cup LP(X) = X \), which shows that if \( X \) is closed, then \( X \) is equal to its closure.

**(⇐) If \( X = \overline{X} \), then \( X \) is closed:**

Assume \( X = \overline{X} \). By the definition of closure, \( \overline{X} \) includes \( X \) and all limit points of \( X \), that is, \( \overline{X} = X \cup LP(X) \). If \( X = \overline{X} \), then \( X \) must contain all its limit points because \( \overline{X} \) contains all limit points of \( X \) by definition. Therefore, \( X \) is closed because a set is closed if and only if it contains all its limit points.

Thus, we have shown both directions of the equivalence: \( X \) is closed if and only if \( X = \overline{X} \). 


**Theorem 4.6: Let $X \sub C$. Then $\overline{X}$ is closed. (equivalently, $\overline{X} = \overline{\overline{X}})$**

Let $x \in LP(\overline{X})$. By *Definition 4.4* $x \in LP(X \cup LP(X))$, and by *Theorem 3.19*, we know that either $x \in LP(X)$ or $x \in LP(LP(X))$

Case 1: $x \in LP(X)$ which implies that $x \in \overline(X)$

Case 2: $x \in LP(LP(X))$
Consider a region $R$ such that for all $R$ containing $x$, $R \cap LP(X)\backslash \{x\} \neq \empty$. Thus, there must exist a $y \in R$, $LP(X)$ such that $y \neq x$. Because $y \in LP(X)$, then all for all $R$ containing $y$, $R\cap X \backslash\{y\} \neq \empty$. Similarly, there must exist $z \in R$, $X$ such that $z \neq y$. Therefore, either $z \neq x$ or $z = x$:

   If $z \neq x$: then for all $R$ containing $x$, $x \in LP(X) $ and $x \in \overline{X}$ because $z \in R$ then $R\cap X \backslash \{x\} \neq \empty$.

   If $z = x$: because $x,y$, and $z$ are distinct pionts, then by *Theorem 3.19*, there exists disjoint regions $x,z \in R_{x,z}$ and $y \in R_y$. Since $y \in LP(X)$ and $y \in R \cap R_y$, then for all $R \cap R_y$, $(R\cap R_y) cap X \backslash \{y\} \neq \empty$. Therefore, there exists some $b \in (R \cap R_y)$, such that $b =y$ because $b \in R_y$, and $R_y \cap R_{x,y}$, then $b \in R_{x,y}$. Thus we know $x \neq b$ and it follows that for all $R_{x,y}$ containing $x, R_{x,y} \cap X \backslash \{x\} \neq \empty$. Therefore $x \in LP(X)$ and $x \in \overline{X}$.

Because for all $x \in \overline{\overline{X}}$, $x \in \overline{X}$, then $\overline{\overline{X}} \sub \overline{X}$, and by *Definition 4.4*, since $\overline{\overline{X}} = \overline{X} \cup LP(\overline{X})$ then $\overline{X} \sub \overline{\overline{X}}$ by *Theorem 1.7*. Therefore we have proven that $\overline{X} = \overline{\overline{X}}$.

Take any \( x \in LP(\overline{X}) \). By *Definition 4.4*, \( x \in LP(X \cup LP(X)) \), and *Theorem 3.19* implies \( x \) is either in \( LP(X) \) or \( LP(LP(X)) \).

- **Case 1**: If \( x \in LP(X) \), then by definition, \( x \in \overline{X} \).

- **Case 2**: If \( x \in LP(LP(X)) \), consider any region \( R \) containing \( x \). There exists \( y \in R \cap LP(X) \) with \( y \neq x \). Since \( y \in LP(X) \), for any region containing \( y \), there exists \( z \in R \) such that \( z \in X \) and \( z \neq y \). This gives us two subcases:

  - If \( z \neq x \), then \( R \cap X \backslash \{x\} \neq \emptyset \), which means \( x \in LP(X) \), and thus \( x \in \overline{X} \).

  - If \( z = x \), distinct regions \( R_{x,z} \) and \( R_y \) exist containing \( x \) and \( y \) respectively, due to *Theorem 3.19*. There must be some \( b \in (R \cap R_y) \) such that \( b = y \), and since \( R_y \cap R_{x,z} \), we have \( b \in R_{x,z} \). Hence, \( x \neq b \), implying \( R_{x,z} \cap X \backslash \{x\} \neq \emptyset \), and \( x \in LP(X) \), resulting in \( x \in \overline{X} \).

Given that every \( x \in \overline{\overline{X}} \) is in \( \overline{X} \), we have \( \overline{\overline{X}} \sub \overline{X} \). Furthermore, \( \overline{X} \sub \overline{\overline{X}} \) by *Theorem 1.7*. Thus, we conclude \( \overline{X} = \overline{\overline{X}} \).


**Theorem 4.8: The sets $\empty$ and $C$ are open.**

Recall the definition of an open set: A subset \( G \) of \( C \) is an open set if its complement \( C \setminus G \) is closed.

First, consider the empty set \( \emptyset \). The complement of \( \emptyset \) in \( C \) is \( C \setminus \emptyset \), which is simply \( C \). By *Theorem 4.2*, \( C \) is closed because it contains all its limit points, as it is the entire space. Since the complement of \( \emptyset \) is closed, \( \emptyset \) itself is open.

Next, consider the entire continuum \( C \). The complement of \( C \) within itself is \( C \setminus C \), which is \( \emptyset \). As established above by *Theorem 4.2*, \( \emptyset \) is closed. Hence, the complement of \( C \) is closed, which implies that \( C \) is open.

Thus, we have shown that both \( \emptyset \) and \( C \) are open sets.


**Theorem 4.9: Let $G \sub C$. Then $G$ is open if and only if for all $x \in G$, there exists a region $R$ such that $x \in R \sub G$.**

(class notes)
$=>$ Contrapositive: If for some $x \in G$, all regions $R$ containing $x$ are not subsets of $G$, then $G$ is not open. We know that $R \not\sub G$ which means there some elements of $R$ are in $C\backslash G$. 

Therefore there is some $x$ that is the limit point of $C \backslash G$ for all $R$ containing some $x$, $R \cap (C \backslash G \backslash \{x\}) \neq 0$ where $x \not\in C \backslash G$. Thus the complement of $G$ is not closed because it does not contain all of its limit points. Based on the definition of an open set, we now know that $G$ is open because its complement is closed. We have thus proved if for all $x \in G$ there exists a region $R$, such that $x$ is an element of $R$ such that $R \sub G$, then $G$ is open

$<= $ Contrapositive: If $G$ is not open, then for some element $x$ in $G$, for all regions $R$ containing $x$, $R \not\sub G$. If $G$ is not open, by *theorem 4.2*, then the complement of $G$ is not closed which means the complement does not contain all of its limit points. Let $x \in LP(C \backslash G)$ and $x \in G$. Therefore, there exists for all regions $R$ such that $x \in R$, $R$ contains elements of $C \backslash G$ because $R \cap G\backslash x \neq \empty$. Therefore $R$ is not subset of $G$ because it contains elements not in $G$.


**Corollary 4.10: Every region $R$ is open. Every complement of a region $C\backslash R$, is closed.**

Let \( R \) be a region in \( C \). By the definition of a region, for every point \( x \in R \), there exists an open interval \( (a, b) \) such that \( x \in (a, b) \sub R \). This open interval \( (a, b) \) serves as the region required by *Theorem 4.9* to conclude that \( R \) is open. Therefore, every region \( R \) is open.

Now, consider the complement of a region \( C \setminus R \). Since \( R \) is open, its complement \( C \setminus R \) must be closed. This is because the definition of an open set \( R \) is such that its complement \( C \setminus R \) is closed. Hence, every region \( R \) is open, and every complement of a region \( C \setminus R \) is closed.


**Corollary 4.11: Let $G \sub C$. Then $G$ is open if and only if for all $x \in G$, there exists a subset $V \sub G$ such that $x \in V$ and $V$ is open.**

**(⇒ Direct)** Assume \( G \) is open. By *theorem 4.9*, for every \( x \in G \), there exists a region \( R \) such that \( x \in R \sub G \). Since every region is open by Corollary 4.10, we can choose \( V = R \) such that $V \sub G$ is also open and $x\in V$. Hence, for every \( x \in G \), there exists an open subset \( V \sub G \) containing \( x \).

**(⇐ Converse)** Assume that for every \( x \in G \), there exists an open subset \( V \sub G \) such that \( x \in V \). We want to prove that $G$ is open. We know that for all $x$, there exists an $R$ such that $x \in R \in V$ and because $R \sub V$ and $V \sub G$, then $R \sub G$, and it also stands that for all $x \in R$, that $x \in R \sub G$ and by *theorem 4.9*, thus $G$ is open. 


Therefore, \( G \) is open if and only if for every \( x \in G \), there exists an open subset \( V \sub G \) containing \( x \).


**Corollary 4.12: Let $a\in C$. Then the sets $\{x \in C| x < a\}$ and $\{x \in C| a < x\}$ are open.**

Given the point $a \in C$, consider the set \( L = \{x \in C \mid x < a\} \). Take any point \( x \in L \). Since \( C \) is a continuum without a first point by *axiom 3*, there exists a point \( k \in C \) such that \( k < x \). Similarly, since \( x < a \), we can find a region \( R \) such that \( k < x \) and \( x < a \) are both in \( R \), and \( R \sub  L \). By *Theorem 4.9*, which states that a set is open if for every point there exists a region contained within the set, \( L \) is open.

Now consider the set \( U = \{x \in C \mid a < x\} \). For any point \( x \in U \), since \( C \) does not have a last point by *axiom 3*, there exists a point \( m \in C \) such that \( x < m \). We can then find a region \( S \) such that \( a < x \) and \( x < m \) are both in \( S \), and \( S \sub U \). Again, by Theorem 4.9, \( U \) is open.

Therefore, both \( \{x \in C \mid x < a\} \) and \( \{x \in C \mid a < x\} \) are open sets.


**Theorem 4.13: Let $G$ be a nonempty open set. Then $G$ is the union of a collection of regions.**

Let \( G \) be a nonempty open set in the continuum \( C \). By Theorem 4.9, for each point \( x \) in \( G \), there exists a region \( R_x \) such that \( x \) is an element of \( R_x \) and \( R_x \) is a subset of \( G \). Consider the collection of all such regions, denoted by \( \{R_x \mid x \in G\} \). We assert that \( G \) is the union of this collection. To establish this claim, we must demonstrate two things: first, that every point in \( G \) is an element of the union of these regions; and second, that this union does not extend beyond \( G \).

For the first part, take any point \( y \) in \( G \). By the definition of an open set, there is a region \( R_y \) containing \( y \), which is also within \( G \). This implies that \( y \) is an element of the union \( \bigcup_{x \in G} R_x \).

For the second part, consider any point \( z \) in the union \( \bigcup_{x \in G} R_x \). By *Corollary 3.20*, \( z \) must be an element of at least one region \( R_x \), where \( x \) is a member of \( G \). Since \( R_x \) is a subset of \( G \), it follows that \( z \) must also be an element of \( G \).

Therefore, we conclude that \( G \) is the union of the regions \( \bigcup_{x \in G} R_x \) which proves that any nonempty open set \( G \) is the union of a collection of regions within the continuum \( C \).

**Exercise 4.14: Do there exists subsets $X \sub C$ that are neither open nor closed?**

Let \( C \) be a continuum of the rationals     , and consider the subset \( X \) defined as \( X = \left\{ \frac{1}{n} \mid n \in \mathbb{N} \right\} \), where \( \mathbb{N} \) denotes the set of natural numbers. We will show that \( X \) is neither open nor closed in \( C \).

To show that \( X \) is not open, we must demonstrate that there exists at least one point in \( X \) that does not have a region entirely contained within \( X \). Take the point \( \frac{1}{1} \in X \). For any region \( R \) containing \( \frac{1}{1} \), there will be points in \( R \) that are not in \( X \) because between any two points in \( X \), there are infinitely many points in \( C \) that are not in \( X \). Hence, no region around \( \frac{1}{1} \) can be entirely contained within \( X \), and therefore \( X \) is not open.

To show that \( X \) is not closed, we need to find a limit point of \( X \) that is not contained in \( X \). Consider the point \( 0 \). For any region \( R \) containing \( 0 \), there are elements of \( X \) within \( R \) because we can always find a natural number \( n \) large enough such that \( \frac{1}{n} \) is in \( R \). However, \( 0 \) itself is not an element of \( X \). Thus, \( 0 \) is a limit point of \( X \) that is not contained in \( X \), and therefore \( X \) is not closed.

In conclusion, the subset \( X = \left\{ \frac{1}{n} \mid n \in \mathbb{N} \right\} \) is an example of a set that is neither open nor closed in the continuum \( C \).


**Theorem 4.15: Let $\{X_\lambda\}$ be an arbitrary collection of closed subsets of a continuum $C$. Then the intersection $\bigcap_\lambda X_\lambda$ is closed.**


Assume \( x \) is a limit point of \( \bigcap_{\lambda \in \Lambda} X_\lambda \). By definition, for every region \( R \) containing \( x \), the intersection \( R \cap \left( \bigcap_{\lambda \in \Lambda} X_\lambda \right) \) is nonempty. This implies that there exists some \( y \) in \( \bigcap_{\lambda \in \Lambda} X_\lambda \) such that \( y \) is also in \( R \). Given that \( y \) is in the intersection, \( y \) must be in each \( X_\lambda \) for all \( \lambda \).

Consequently, for each \( X_\lambda \), the intersection \( R \cap (X_\lambda \setminus \{x\}) \) is nonempty. This means that \( x \) is a limit point of every \( X_\lambda \). Since each \( X_\lambda \) is closed, and closed sets contain all their limit points, \( x \) must be an element of every \( X_\lambda \) for all \( \lambda \).

Therefore, \( x \) is an element of \( \bigcap_{\lambda \in \Lambda} X_\lambda \), proving \( \bigcap_{\lambda \in \Lambda} X_\lambda \), being a set that contains all its limit points, is closed.


**Corollary 4.16: Let $\{G_\lambda\}$ be an arbitrary collection of open subsets of a continuum $C$. Then the union $\bigcup_\lambda G_\lambda$ is open.**

Consider the set \(G = \bigcup_{\lambda \in \Lambda} G_\lambda\), where each \(G_\lambda\) is an open subset of \(C\). To prove that \(G\) is open, we must show that for every point \(x \in G\), there exists a region \(R\) such that \(x \in R \sub G\) (*Theorem 4.9*).

Let \(x\) be an arbitrary point in \(G\). By *Corollary 3.20*, there exists at least one index \(\lambda_0 \in \Lambda\) such that \(x \in G_{\lambda_0}\) if $x$ is in $G$. Since \(G_{\lambda_0}\) is open, by *Theorem 4.11*, there exists a subset \(V \sub G_{\lambda_0}\) such that \(x \in V\) and \(V\) is open.

Now, since \(G_{\lambda_0} \sub G\) and \(V \sub G_{\lambda_0}\), it follows that \(V \sub G\). Hence, for our arbitrary point \(x\), we have found a region \(V\) such that \(x \in V \sub G\), satisfying the condition for \(G\) to be open. Additionally, because for all elements of $x \in \bigcup_\lambda G_\lambda$ the subsets $G_\lambda$ include elements $x$ by *definition 1.14* which defined $x$ to be elements of a subset $G_\lambda$ for all $\lambda \in I$ where $I$ is an nonempty set, and subsets $G_\lambda$ are given to be open, then by satisfying all conditions of *theorem 4.11*, the union $\bigcup_\lambda G_\lambda$ is open.


**Theorem 4.17: Let $\{G_1...,G_n\}$ be a finite collection of open subsets of a continuum $C$. Then the intersection $G_1 \cap ... \cap G_n$ is open.**

To demonstrate that the intersection \(\bigcap_{i=1}^{n} G_i\) is open, we must show that for any point \(x\) in the intersection, there exists a region \(R\) such that \(x \in R \sub \bigcap_{i=1}^{n} G_i\). Let \(x\) be an arbitrary point in \(\bigcap_{i=1}^{n} G_i\). Since \(x\) is in the intersection, it is contained in each \(G_i\), where \(1 \leq i \leq n\). Because each \(G_i\) is open, by *Theorem 4.9*, for each \(i\), there exists a region \(R_i\) such that \(x \in R_i \sub G_i\).

Now, consider the intersection of these regions, \(R_{\text{inter}} = \bigcap_{i=1}^{n} R_i\). *By Theorem 3.18*, the intersection of a finite number of regions containing a common point \(x\) is itself a region containing \(x\). Therefore, \(R_{\text{inter}}\) is a region containing \(x\). Since \(R_i \sub G_i\) for all \(i\), it follows that \(R_{\text{inter}} \sub \bigcap_{i=1}^{n} G_i\). Thus, for our point \(x\), we have found a region \(R_{\text{inter}}\) such that \(x \in R_{\text{inter}} \sub \bigcap_{i=1}^{n} G_i\), which satisfies the definition of an open set by *Theorem 4.9*.

Therefore, the intersection \(\bigcap_{i=1}^{n} G_i\) is open.


**Corollary 4.18: Let $X_1,..., X_n$ be a finite collection of closed subsets of a continuum $C$. Then the union $X_1\cup ... \cup X_n$ is closed.**

To prove that the union of a finite number of closed sets is closed, we will show that the complement of the union is open. By definition, a set is closed if its complement is open. For each closed set \( X_i \), its complement \( C \backslash X_i \) is open. Consider the intersection of these open complements: \( \bigcap_{i=1}^{n} (C \backslash X_i) \). By *Theorem 4.17*, the intersection of a finite number of open sets is open. Therefore, \( \bigcap_{i=1}^{n} (C \backslash X_i) \) is open.

By *Theorem 1.15*, which states that the complement of a union is the intersection of the complements, we have:

\[ C \backslash \left( \bigcup_{i=1}^{n} X_i \right) = \bigcap_{i=1}^{n} (C \backslash X_i) \]

Since the right-hand side of the equation is open, the left-hand side, which is the complement of the union \( \bigcup_{i=1}^{n} X_i \), is also open.

Therefore, the union \( \bigcup_{i=1}^{n} X_i \) is the complement of an open set, which means it is closed.


**Exercise 4.19: Is it necessarily the case that the intersection of an infinite number of open sets is open? Is it possible to construct an infinite collection of open sets whose intersection is not open? Equivalently, is it possible to construct an infinite collection of closed sets whose union is not closed?**

1. Intersection of an Infinite Number of Open Sets:

   Yes, it is possible to construct an infinite collection of open sets whose interseciton is not open. Consider the infinite collection of sets \( A_n = \left\{ x \in \mathbb{Q} \mid -\frac{1}{n} < x < \frac{1}{n} \right\} \) where \( n \) is a natural number in \( \mathbb{N} \). Each set \( A_n \) is open in the continuum \( \mathbb{Q} \) because for each element \( x \) in \( A_n \), there exists a region within \( A_n \) that contains \( x \).

   The intersection of all such sets is:
   \[ A = \bigcap_{n \in \mathbb{N}} A_n \]

   As \( n \) increases, the size of the sets \( A_n \) decreases. The only point that is common to all \( A_n \) is \( 0 \). Therefore, the intersection \( A \) is the singleton set containing only the point \( 0 \), which can be written as \( A = \{0\} \).

   However, there exists no region \( R \) such that \( 0 \in R \sub A \), because any region containing \( 0 \) would necessarily contain other points not in \( A \). Because there is no region $R$ such that $0 \in R \sub A$, by *Theorem 4.9*, \( A \) is not open.

2. Union of an Infinite Number of Closed Sets:

   Yes, it is possible to construct an infinite collection of closed sets whose union is not closed. Consider the infinite collection of singletons \( B_n = \left\{ \frac{1}{n} \right\} \) where \( n \) is a natural number in \( \mathbb{N} \) and \( B_n \sub \mathbb{Q} \). Each singleton \( B_n \) is closed in \( \mathbb{Q} \) because it contains all its limit points because they are finite.

   The union of all such singletons is:
   \[ B = \bigcup_{n \in \mathbb{N}} B_n \]

   The set \( B \) does not include \( 0 \), yet \( 0 \) is a limit point of \( B \) because for every positive integer \( m \), there exists an \( n \) such that \( \frac{1}{n} < \frac{1}{m} \), and thus \( \frac{1}{n} \) is in \( B \) and within \( \frac{1}{m} \) of \( 0 \).

   Since \( B \) does not contain this limit point \( 0 \), it is not closed. This demonstrates that the union of an infinite number of closed sets is not necessarily closed.


**Corollary 4.20: Let $G \sub C$ be nonempty. Then $G$ is open if and only if $G$ is the union of a collection of regions.**

1. If \( G \) is open, then \( G \) is the union of a collection of regions:

   Assume \( G \) is open. By *Theorem 4.9*, for every point \( x \in G \), there exists a region \( R_x \) such that \( x \in R_x \sub G \). The collection of all such regions \( \{R_x \mid x \in G\} \) is entirely contained by \( G \), since every point in \( G \) is contained within at least one region in the collection. Therefore, \( G \) can be expressed as the union of these regions:
   \[ G = \bigcup_{x \in G} R_x \]
   This demonstrates that if \( G \) is open, it is the union of a collection of regions.

2. If \( G \) is the union of a collection of regions, then \( G \) is open:

   Conversely, assume \( G \) is the union of a collection of regions, say \( G = \bigcup_{n \in \mathbb{N}} R_n \), where each \( R_n \) is a region. By *Theorem 4.10*, each region \( R_n \) is open. Since the union of open sets is open, the set \( G \), being a union of the open regions \( R_n \), is also open. Thus, if \( G \) is the union of a collection of regions, it must be open.


**Corollary: 4.21: If $\underline{ab}$ is a region of $C$, then ext $\underline{ab}$ is open.**

Given that \( \underline{ab} \) is a region in the continuum \( C \), we want to show that \( \text{ext} \underline{ab} \), the exterior of \( \underline{ab} \), is open. By *Lemma 3.15*, the complement of \( \underline{ab} \) along with its endpoints in \( C \) is given by:
\[ C \setminus (\{a\} \cup \underline{ab} \cup \{b\}) = \text{ext} \underline{ab} \]

To establish that \( \text{ext} \underline{ab} \) is open, we refer to *Definition 4.6*, which implies that the complement of an open set is closed. Therefore, if \( \text{ext} \underline{ab} \) is open, its complement:
\[ C \setminus \text{ext} \underline{ab} = \{a\} \cup \underline{ab} \cup \{b\} \]
must be closed.

We must show that there are no limit points of \( \{a\} \cup \underline{ab} \cup \{b\} \) that are not contained within the set itself. Assume for contradiction that there exists a point \( d \) that is a limit point of \( \underline{ab} \) and \( d < a \). By the properties of a continuum (specifically, *Axiom 3*), there must exist a point \( z \) such that \( z < d \). If there is a point \( q \) with \( d < q < a \), then there exists a region \( \underline{za} \) that does not intersect with \( \{a\} \cup \underline{ab} \cup \{b\} \) except possibly at \( d \):
\[ \underline{za} \cap (\{a\} \cup \underline{ab} \cup \{b\} \setminus \{d\}) = \emptyset \]
This implies that \( d \) cannot be a limit point of \( \{a\} \cup \underline{ab} \cup \{b\} \), contradicting our assumption.

Therefore, no such limit point \( d \) exists, and the set \( \{a\} \cup \underline{ab} \cup \{b\} \) contains all its limit points, confirming it is closed. Consequently, \( \text{ext} \underline{ab} \), being the complement of a closed set, is open.


**Theorem 4.23: Let $C$ be a connected continuum. Let $x$, $y ∈ C$, with $x < y$. Then there exists $z ∈ C$ such that $x < z < y$.**

Assume for the sake of contradiction that there does not exist an element \( z \in C \) such that \( x < z < y \). By *Corollary 4.12*, for any element \( a \in C \) and \( x \in G \sub C \), the sets \( \{x \in C \mid x \leq a\} \) and \( \{x \in C \mid a < x\} \) are open in the subspace topology of \( C \).

Therefore, under our assumption, \( C \) can be expressed as the union of two sets \( A \) and \( B \), where \( A \sub C \) with \( A = \{a \in C \mid a < y\} \) and \( B \sub C \) with \( B = \{b \in C \mid b > x\} \). We do not include the case where \( a = y \) or \( b = x \) since our assumption negates the existence of such points \( z \) that would satisfy \( x < z < y \). Furthermore, \( A \) and \( B \) are nonempty because \( x \in A \) and \( y \in B \), as given by the conditions of the theorem.

Additionally, \( A \) and \( B \) are disjoint. This follows because, according to the ordering of the continuum (Axiom 2), there can be no element in \( C \) that is both less than \( x \) and greater than \( y\). Consequently, \( \overline{A} \cap B = \emptyset \) and \( A \cap \overline{B} = \emptyset \), which means \( A \cap B = \emptyset \). The existence of these disjoint, nonempty open sets \( A \) and \( B \), such that \( C = A \cup B \), contradicts the premise that \( C \) is connected. This contradiction implies that our initial assumption must be false.

Therefore, there must exist a point \( z \in C \) such that \( x < z < y \).


**Exercise 4.24: Let $C$ be a connected continuum and $a ∈ C$. Prove that $C \backslash \{a\} $is a disconnected continuum.**

We begin by confirming that \( C \backslash \{a\} \) is a continuum by the axioms:
1. It is nonempty, as removing a single point from a continuum leaves other points.
2. It retains the well-defined ordering of \( C \).
3. It has no first or last point, since \( C \) is a continuum and the removal of \( a \) does not create extremal points.

To demonstrate that \( C \backslash \{a\} \) is disconnected, consider two subsets:
- \( S_1 = \{x \in C \backslash \{a\} \mid x > a\} \)
- \( S_2 = \{x \in C \backslash \{a\} \mid x < a\} \)



By *Theorem 4.23*, for any \( x \in S_1 \), there exists a \( z \) such that \( a < z < x \), ensuring that \( z \in S_1 \) and that \( S_1 \) is indeed nonempty and open. A similar argument applies to \( S_2 \), establishing its openness and non-emptiness. Thus, \( S_1 \) and \( S_2 \) are open in \( C \backslash \{a\} \), disjoint, and nonempty, satisfying the conditions of *definition 4.22* for a disconnected space.

Therefore, \( C \backslash \{a\} \) can be expressed as the union of \( S_1 \) and \( S_2 \), which are nonempty, disjoint, open sets proving that \( C \backslash \{a\} \) is disconnected.