***<h1 style="text-align: center;">Script 5</h1>***
**Theorem 5.1: The only subsets of a continuum $C$ that are both open and closed are $\empty$ and $C$.**

Let's prove this by contradiction. Assume there exists a non-empty subset $A \sub C$ such that $A$ is both open and closed and $A \neq C$.


Because $A$ is open and closed and nonempty, its complement $C\backslash A$ is open and nonempty by *Definition 4.7* which states that a set is open if its complement is closed. We also know that because they are complements, $A \cap (C \backslash A) = \empty$ which means they are disjoint as they contain no similar elements. This means we have two nonempty, open sets which contradicts the definition of connected set because $C$ can now be represented as the union of two non-empty disjoint open sets, thus making $C$ disconnected which contradicts the fact that $C$ is connected thus our assumption is false and therefore through proof by contradiction the only subsets of continuum $C$ that are open and closed are $\empty$ and $C$.


**Corollary 5.2: Every region is infinite.**

Assume, for the sake of contradiction, that there exists a finite region \( R \) denoted as \( \underline{ab} \), where \( a, b \in C \) and \( a < b \). According to this assumption, the elements in the region can be arranged in a finite sequence, due to *Theorem 3.5*. This sequence is of the form \( a < x_1 < x_2 < \ldots < x_n < b \), with \( n \) elements in total where $n\in \N$.

However, this assumption leads to a contradiction. According to this sequence, there are no elements between \( x_1 \) and \( x_2 \). This directly contradicts *Theorem 4.23*, which states that in a connected continuum (which a continuum must be by *Axiom 4*), for any two elements \( x_1, x_2 \in C \) with \( x_1 < x_2 \), there must exist another element \( z \in C \) that lies between \( x_1 \) and \( x_2 \) such that there are an infinite number of points between any two points which is in direct contrast with the cardinality $n$ specified by *Theorem 3.5* for a finite region. Thus our assumption that $R$ is a  finite region is false, and every region must be infinite.


**Corollary 5.3: Every point of $C$ is a limit point of $C$.**

Assume, for contradiction, that there exists a point \( x \in C \) which is not a limit point of \( C \). This assumption implies that there is a region \( R \) containing \( x \), where \( x \in R \subseteq C \), and \( R \) satisfies the condition: \( R \cap C \setminus \{x\} = \emptyset \). In simpler terms, besides \( x \), the region \( R \) does not contain any other points of \( C \).

However, this assumption leads to a contradiction when we consider *Corollary 5.2*, which we previously proved. *Corollary 5.2* states that every region in \( C \) is infinite. Therefore, it's impossible for the region \( R \) to contain only the point \( x \) if it's a part of \( C \); \( R \) must contain infinitely many points.

Thus, our original assumption, that \( R \) contains only \( x \) and no other points from \( C \), contradicts the fact established in *Corollary 5.2*. Therefore, \( R \cap C \setminus \{x\} \) cannot be empty, implying that \( x \) must be a limit point of \( C \). Consequently, our initial assumption is false, and it follows that every point in \( C \) is indeed a limit point of \( C \).



**Corollary 5.4: Every point of the region $\underline{ab}$ is a limit point of $\underline{ab}$.**

Suppose, for the sake of contradiction, that there exists a point \( x \) in the region \( \underline{ab} \) which is not a limit point of \( \underline{ab} \). This means that we can find a region \( R \) containing \( x \), where \( x \in R \subseteq C \), and this region \( R \) satisfies the condition: \( R \cap \underline{ab} \setminus \{x\} = \emptyset \). In other words, \( R \) does not contain any points from \( \underline{ab} \) other than \( x \).

However, this assumption leads to a contradiction. Note that \( R \cap \underline{ab} \) is itself a region within \( C \). According to *Corollary 5.2*, every region within \( C \) is infinite. This implies that the region \( R \cap \underline{ab} \) must contain infinitely many points.

Thus, if \( R \cap \underline{ab} \) is infinite, then \( R \cap \underline{ab} \setminus \{x\} \) cannot be empty. There must be other points in \( R \cap \underline{ab} \) besides \( x \). This contradicts our initial assumption that \( R \cap \underline{ab} \) contains only \( x \). Therefore, our assumption that \( x \) is not a limit point of \( \underline{ab} \) is false. It follows that every point in the region \( \underline{ab} \) must be a limit point of \( \underline{ab} \).
   c 

**Exercise 5.7: If sup $X$ exists, then it is unique, and similarly for inf $X$.**

Assume that sup $X$ exists and suppose for the sake of contradiction there are at least two distinct least upper bounds, call them $u$ and $u'$ where $u \neq u'$. 

By *definition 5.6*, a supremum $u$ must be an upper bound of $X$ and for any upper bound $u'$ of $X$, $u \leq u'$. This is the same for $u'$ to be a supremum as well, it must be less than or equal to $u$. Thus they both must be upper bounds, more importantly, $u' \leq u$ and $u \leq u$ which means $u = u'$. However, this contradicts our assumption that there are two distinct, equal least upper bounds. Therefore, if sup $X$ exists, then it must be unique.

This same logic can equally be applied to inf $X$ with reverse comparative signage.


**Exercise 5.8: If $X$ has a first point $L$, then inf $X$ exists and equals $L$. Similarly, if $X$ has a last point $U$, then sup $X$ exists and equals $U$.**


Assume that $X$ has a first point $L$ such that $L < x$ where $x$ for all $x \in X$ which means $L$ is a lower bound of $X$ by *definition 5.5*. To show that $L$ is a greatest least bound of $X$, we must show that:
   1. $L$ is a lower bound of $X$ and
   2. If $L'$ is any lower bound of $X$, then $L' \leq L$. 

The first condition is met by $L$ being the first point by *Definition 3.3* as  a first point $L$ of a set X means $L ≤ x$ for all x in X. This satisfies the requirement for L to be a lower bound of X, as it is less than or equal to every element in X. 

As for the second condition, Suppose there exists another lower bound $L'$ of $X$. By the definition of a lower bound, $L' ≤ x$ for all $x \in X$. Since $L$ is the first point of $X$, it is the smallest element in $X$. Therefore, for any lower bound $L'$, it must hold that $L' ≤ L$. This is because $L'$ cannot be greater than the smallest element of $X$ and still be a lower bound. This satisfies the condition that $L$ is greater than or equal to every other lower bound of $X$. Therefore, by satisfying these two conditions, L is the greatest least bound, or the infimum, of X.

Sup $X$ can be proved by *definition 3.3* for the last point in a similar manner.


**Exercise 5.9: For this exercise, we assume that $C = \R$. Find sup $X$ and inf $X$ for each of the following subsets of $\R$, or state that they do not exist. You need not give proofs.**
1. $X = \N $
   1. sup $X$ does not exist because the set of natural numbers has no upper bound as it goes on indefinitely. 
   2. inf $X = 1$ since 1 is the first point of the set of natural numbers, thus it is inf $X$ by *exercise 5.8*.
2. $X = \mathbb{Q}$
   1. neither sup nor inf exist for $X$ because the set of rational numbers extend infinitely in both positive and negative directions such that there is no upper nor lower bound
3. $X = \{\frac 1 n | n ∈ N\}$ 
   1. sup $X$ = 1 because 1 is the upper bound such that there will never be a number in the set $X$ that is greater than 1
   2. inf $X$ is 0, though $0$ is not in the set, it fulfills the requirements because it is a lower bound which the elements of $X$ get close to 0 as $n$ increases.
4. $X = \{x ∈ \R | 0 < x < 1\} $
   1. sup X = $1$, even though 1 is not in the set, no element in the set $X$ is greater than 1 such that $1$ is an upper bound 
   2. inf $X$ = 0, 0 is the greatest lower bound for $X$, even though it's not part of the set since all elements are greater than 0.
5. $X = \{3\} ∪ \{x ∈ \R | −7 ≤ x ≤ −5\}$
   1. sup $X=3$, since 3 is the largest number in the union of the two sets.
   2. inf $⁡X= −7$, because it's the smallest number in the combined set and is included in the set $X$.

**Lemma 5.10: Suppose that $X$ is a nonempty subset of $C$ and $s =$ sup $X$ exists. If $p < s$, then there exists an $x ∈ X$ such that $p < x ≤ s$.**

Assume that \( X \) is a nonempty subset of \( C \) and that \( s = \sup X \) exists. Let \( p \) be any element in $X$ such that \( p < s \). For the sake of contradiction, suppose that there does not exist an \( x \in X \) such that \( p < x \). This means that for all \( x \in X \), \( x \leq p \) or \( x > s \). However, \( x > s \) is impossible because \( s \) is the least upper bound of \( X \).

If \( x \leq p \) for all \( x \in X \), then \( p \) would be an upper bound for \( X \) by *Definition 5.5*, which contradicts the fact that \( s \) is the least upper bound of \( X \) and \( p < s \) by *Definition 5.6*. This contradiction implies that our assumption is false. Therefore, there must exist an \( x \in X \) such that \( p < x \leq s \).


**Theorem 5.11: Let $a < b$. The least upper bound and greatest lower bound of the region $\underline{ab}$ are: sup $\underline{ab}$ = $b$ and inf $\underline{ab}$ = $a$.**

Consider the region \( \underline{ab} \), which is the set of all points \( x \) such that \( a < x < b \). We aim to prove that \( \sup \underline{ab} = b \) and \( \inf \underline{ab} = a \).

We show that \( a \) is a lower bound for \( \underline{ab} \). Since for all \( x \in \underline{ab} \), \( a < x \), \( a \) is less than every element in \( \underline{ab} \) by *Definition 5.5*. To demonstrate that \( a \) is the *greatest* lower bound, suppose there exists some element $l$ such that \( l > a \) that is also a lower bound. Let there be a point $c$ in the region $\underline{al}$ which exists because of *Theorem 4.23* since the continuum is connected, between any two points there exists another point $c$ such that $a < c < l$. Thus $l$ cannot be a lower bound which contradicts our previous asusmption that $q < a$ thus inf$\underline{ab} = $a$. 

Hence, we have proven that \( \sup \underline{ab} = b \) and \( \inf \underline{ab} = a \)

**Theorem 5.12: Let $X$ be a nonempty subset of $C$. Suppose that sup $X$ exists and sup $X /not \in X$. Then sup $X$ is a limit point of $X$. The same holds for inf $X$.**

Let $s =$ sup $X$. Because $S$ is not empty, there exists an element $p$ that is any point in the continuum such that $p < s$. By *Theorem 5.6*, there exists an element $c$ where $c>s$ which exists by *axiom 3* because there is no last point. Therefore, we can create a region where $s \in \underline{pc'}$. There exists an $x$ for any $p$ and $x \neq s$ because $s$ is not in $X$, but $x$ is in $X$ such that $p < x \leq s$ by *Lemma 5.10*. For any region $\underline{pc}$ containing $x$, $\underline{pc} \cup x \backslash\{s\} \neq \empty$ which means that sup $X$ is a limit point of $X$. The same holds for inf $X$. 

**Corollary 5.13: Both $a$ and $b$ are limit points of the region $\underline{ab}$. Let $[a, b]$ denote the closure $\overline{\underline{ab}}$ of the region $\underline{ab}$.**

We know that $a =$ inf $\underline{ab}$ and $b=$ sup $\underline{ab}$ by *Theorem 5.11*, and since $a \not \in \underline{ab}$ and $b \not \in \underline{ab}$, then by *Theorem 5.12*, $a, b \in$ LP$(\underline{ab})$.


**Corollary 5.14: $[a, b] = {x ∈ C | a ≤ x ≤ b}$.**

The set $[a,b]$ is defined as the closure $\overline{\underline{ab}}$ as proven by *Corollary 5.13*. Thus by definition of a closure in *Definition 4.4* which says a closure is the union of the set and its limit points, $[a,b]$ must include both the elements of the region $\underline{ab}$ such that any element $x$ of closure $[a,b]$ must be between $a$ and $b$ where $a < x < b$ by *Definition 3.9* and its limit points which are $a$ and $b$ such that $x$ can also equal $a$ or $b$, once again as described by *Corollary 5.13*. Additionally, we know that there are no other limit poitns outside of the reigon $\underline{ab}$ by *Lemma 3.16* wich states that there is no point of the exterior of a region that can be a limit point of that region; thus, there are no other limit points outside of the closure. This means $[a,b]$ is exactly the set of all points $x$ in $C$ such that $a≤x≤b$.


**Lemma 5.15: Let $X ⊂ C$ and define: $Ψ(X) = \{x ∈ C | x \; \textnormal{is not an upper bound of} \; X\}.$ Then $Ψ(X)$ is open. Define: $Ω(X) = \{x ∈ C | x \;  \textnormal{is not a lower bound of} \; X\}$.Then $Ω(X)$ is open.**

We want to prove that the complement is closed. We can do this by contradiction by letting $x \in LP(C\backslash \Psi (X)$ such that it is a limit point of the set of upper bounds. Suppose $x \not \in C \backslash \Psi (X)$. x is not upperbound, so then there exists a $y \in X$ such that $x < y$. There exists $z$ such that $z < x$ which exists because we are in a continuum that does not have a last point nor first point. Thus $x \in \underline{zy}$, but $\underline{zx} \cap (C \backslash \Psi (X) \backslash \{x\}) = \empty$. This is because no points in the complement of $\Psi (X)$ is smaller than $y$ because all the elements in that set are upper bounds and must be larger than $y$ by definition. Thus, $x$ is in the complement of $\Psi (X)$, thus the complement of $\Psi (X)$ is closed, and by definition of an open set, $\Psi (X)$ is open.

**Alternative**

Take a point $x \in \Psi (X)$ and there exists a point $b \in X$ such that $x < b$ that exists because ... For all $x$ inside of $X$, there exists a region $\underline{ab} \sub \Psi (X)$ this is because $b \in X$ and any element less than $b$ cannot be an upper bound by definition of an upper bound.


**Theorem 5.16 (Least Upper Bound Property): Suppose that $X$ is nonempty and bounded above. Then sup $X$ exists. Similarly, if $X$ is nonempty and bounded below, then inf $X$ exists.**

We will prove this by contradiction. Assume for the sake of contradiction that $X$ is nonempty and bounded above and that the sup$X$ does not exist. We define $A = C \backslash \Psi (X)$ is the set of upper bounds of $X$. Because $X$ is bounded above, then $A \neq \empty$, and since we know that sup$(X)$ does not exist, then for all $y \in A$, we can say that $y$ is not the least upper bound of $X$. Then, we can say there is some $z \in A$ where $z < y$. Because $z \in A$, then $z > x$ for all $x \in X$. then, for any point $a \in C$ where $a > z$, then $a > x$ for all $x \in X$.
   1. For any point $a$ in the continuum where $a > z$, then $a \in A$ because it must be in the upper bounds of $X$ by *Definition 5.5* because it is larger than all $x \in X$. Because the continuum has no last point by *Axiom 3*, then we know that there exists a point $u$ such that $ u > y$. We define the region $\underline{zu}$ such that $z < y < u$ thus $y \in \underline[zu]$. For all points $n \in \underline{zu}$, we know that $n > z$. By line 1, we know that for all $n \in \underline{zu}$ thus $n \in A$. Then $y \in \underline{zu}$ is a subset of $A$. Therfore, $A$ is open by *Theorem 4.9*.
   2. $A$ is nonempty and open. We can say that $\Psi (X)$ is open by *Lemma 5.15*. Because $X$ is nonempty, then we can find some $w \in X$ then there exists some $d < w$ by *Axiom 3* stating that a continuum has no first point. Therefore, $d$ is not an upper bound of $X$. Now, we can state that $\Psi (X)$ is nonempty. 
   3. Since we know that $\Psi (X)$ is nonempty and open, $A = C \backslash \Psi (X)$ then $A \cap \Psi (X) = \empty$, then $A$ and $\Psi (X)$ are disjoint. Because $A$ and $\Psi (X)$ are empty, open, and disjoint, then $C = A \cap \Psi (X)$ and $C$ is the union of nonempty, open, and disjoint sets thus $C$ is disconnected by *Definition 4.22* and this is a contradiction.


For the sake of contradiction assume that the set $X$ is nonempty and bounded above but sup $X$ does not exist. 

**Corollary 5.17: Every nonempty closed and bounded set has a first point and a last point.**

We can prove this by contradiction. Suppose there exists a set $X$ such that $X$ is nonempty, closed, and bounded. Then assume for the sake of contradiction $X$ has no first nor last point. Since $X$ is bounded, then there exists supX and infX by *Theorem 5.16*. The last point is somoe $x \in X$ such that $x /geq a$ where $a \in X$. We know that the sup$x \not \in X$, so if supx $\in X$, then supx $\geq x$ for all $x \in X$. If supx $\not \in X$, then supx $\in$ LP(X) by *Theorem 5.12*. However, this x does not contain all of its limit points, thus $x$ is not closed, causing a contradiction.

**alternative**
Because the set is bounded, the infx exists such that there are 2 cases where the infx is in X or not in X. If it is in x, then infx is the first point, but if its not in X then it is a limit point of X because in 5.12. Applicable to supX as well.

**Exercise 5.18: Is this (Corollary 5.17) true for $\mathbb{Q}$?**

Suppose $\mathbb{Q}$ is the continuum $C$, and suppose the subset $S = \{x \in \mathbb{Q} | x^2 < 2\}$. Consider for every element $x$, there exists an element $y = \frac {(2x+2)} {(x+2)}$ and we want to show that  $y > x$ and $y \in S$ such that $x$ cannot be the last point. Using algebra we have $x^2 + 2x < 2x +2$ such that $x^2 < 2$ which shows that $y > x$. $y^2 = \frac{((2x+2)(2x_2))} {((x+2)(x+2))}$ which simplifies into $\frac {(4x^2+8x+4)} {(x^2+4x+4)} < 2$ which is equal to $4x^2 + 8x + 4 < 2x^ + 8x + 8$ which proves that there exists a $y > x$ and $y^2 < 2$ so *Corollary 5.17* is true for $\mathbb{Q}$.



**Extra Problem 4: Assume that $C$ satisfies Axioms 1,2 and 3. Do not assume that $C$ satisfies Axiom 4. Suppose also that 
(a) every nonempty subset $X$ of $C$ that is bounded above has a supremum 
(b) for any $a, b ∈ C$, there is some $z ∈ C$ with $a < z < b$. Show that $C$ is connected.**

*Axiom 1: A continuum is a nonempty.*
*Axiom 2: A continuum has an ordering $<$.*
*Axiom 3: A continuum has no first or last point.*
*Axiom 4: A continuum is connected*


To show that \( C \) is connected, assume for contradiction that it is not. This means there exist nonempty subsets \( A \) and \( B \) such that \( C = A \cup B \), \( A \cap B = \emptyset \), and both \( A \) and \( B \) are open in \( C \). Next, let \( a \in A \) and \( b \in B \) with \( a < b \) by *Axiom 2*. Consider \( S = \{ x \in C | x < b \} \). Since \( B \) is open, there exists \( c > 0 \) such that \( \underline{cb} \subset B \). Thus, \( S \) is bounded above by \( b \) and has a supremum in \( C \), denoted as \( s \). We know for any \( d > 0 \), the interval \( \underline{ds} \) intersects \( S \). 

   - Case 1: If \( s \in A \), then there exists \( d > 0 \) such that \( \underline{ds} \subset A \). This contradicts the disjoint nature of \( A \) and \( B \).
   - Case 2: If \( s \in B \), elements arbitrarily close to \( s \) and less than $s$ as defined by *Axiom 2)* are in \( S \) (and hence in \( A \)), contradicting the openness of \( B \).

In both cases, we reach a contradiction, which implies our assumption that \( C \) is not connected is false. Therefore, \( C \) must be connected.


