***<h1 style="text-align: center;">Script 5</h1>***
**Theorem 5.1: The only subsets of a continuum $C$ that are both open and closed are $\empty$ and $C$.**

Let's prove this by contradiction. Assume there exists a non-empty subset $A \sub C$ such that $A$ is both open and closed and $A \neq C$.

Because $A$ is open and closed and nonempty, its complement $C\backslash A$ is open and nonempty by definition of an open sets. We also know that because they are complements, $A \cap (C \backslash A) = \empty$ which means they are disjoint. This means we have two nonempty, open sets which contradicts the definition of connected set because $C$ can now be represented as the union of two non-empty disjoint open sets, thus making $C$ disconnected which contradicts the fact that $C$ is connected thus our assumption is false and therefore the only subsets of continuum $C$ that are open and closed are $\empty$ and $C$ and our assumption is false. 


**Corollary 5.2: Every region is infinite.**

**MORE**

Let's prove this by contradiction. Assume the region $R = \underline{ab}$ is finite where $a,b \in C$ and $a < b$ then we can list elements where there are $n$ elements in the region in order by *theorem 3.5* in this format: $a < x_1<x_2<...x_n<b$. Because there are no elements between $x_1$ and $x_2$, then this contradicts our assumption that every region is finite. Thus every region is infinite.



**Corollary 5.3: Every point of $C$ is a limit point of $C$.**

Let's prove this by contradiction. Let us assume there there that for all regions $R$ containing $x\in C$ where $x \in R \sub C$, this will be true: $R \cap C \{x\} = \empty$. But by *corollary 5.2* where we proved all regions are infinite, we know that the previously stated intersection cannot only contain $x$ thus $R \cap C \{x\} \neq \empty$ which contradicts our assumption and proves that every point of the region $\underline{ab}$ is a limit point of $\underline{ab}$.


**Corollary 5.4: Every point of the region $\underline{ab}$ is a limit point of $\underline{ab}$.**

We can prove this by contradiction by assuming that $x$, where $x$ is a limit point of the region $\underline{ab}$, is actually not a limit point of the region $\underline{ab}$. For all $R$ such that $R$ contains $x$ and $x \in R \sub C$ such that $R \cap \underline{ab} \backslash\{x\} = \empty$. We know that $R$ \cap \underline{ab} is also a region and by *corollary 5.2*, we know that all regions are infinite so we know that this the region $R \cap \underline{ab}$ is infinite which means that $R \cap \underline{ab} \backslash \{x\} \neq \empty$ such that $x$ cannot exist which contradicts our assumption which proves that Every point of the region $\underline{ab}$ is a limit point of $\underline{ab}$.

**Exercise 5.7: If sup $X$ exists, then it is unique, and similarly for inf $X$.**

Assume that sup $X$ exists and suppose for the sake of contradiction there are at least two distinct least upper bounds, call them $u$ and $u'$ where $u \neq u'$. 

By *definition 5.6*, a supremum $u$ must be an upper bound of $X$ and for any upper bound $u'$ of $X$, $u \leq u'$. This is the same for $u'$ to be a supremum as well, it must be less than or equal to $u$. Thus they both must be upper bounds, more importantly, $u' \leq u$ and $u \leq u$ which means $u = u'$. However, this contradicts our assumption that there are two distinct, equal least upper bounds. Therefore, if sup $X$ exists, then it must be unique.

This same logic can equally be applied to inf $X$ with reverse comparative signage.


**Exercise 5.8: If $X$ has a first point $L$, then inf $X$ exists and equals $L$. Similarly, if $X$ has a last point $U$, then sup $X$ exists and equals $U$.**

Assume that $X$ has a first point $L$ such that $L < x$ where $x$ for all $x \in X$ which means $L$ is a lower bound of $X$ by *definition 5.5*. To show that $L$ is a greatest least bound of $X$, we must show that:
   1. $L$ is a lower bound of $X$ and
   2. If $L'$ is any lower bound of $X$, then $L' \leq L$.

The first condition is met by $L$ being the first point. As for the second point, suppose there is a point $L'$ that any lower bound for $X$. Since, $L$ is the first point of $X$ then by *definition 3.3* for every point $x$ in $X$, $L \leq x$. The definition of the first point satisfies the second condition for inf $X$, thus $L$ is the greatest least bound of $X'$.

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


**Theorem 5.16: Suppose that $X$ is nonempty and bounded above. Then sup $X$ exists. Similarly, if $X$ is nonempty and bounded below, then inf $X$ exists.**

For the sake of contradiction assume that the set $X$ is nonempty and bounded above but sup $X$ does not exist. 

**Corollary 5.17: Every nonempty closed and bounded set has a first point and a last point.**


**Exercise 5.18: Is this (Corollary 5.17) true for $\mathbb{Q}$?**