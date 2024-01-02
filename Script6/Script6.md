***<h1 style="text-align: center;">Script 6</h1>***

**Lemma 6.2: Let $A$ be a Dedekind cut and $x ∈ Q$. Then $x \not \in A$ if, and only if, $x$ is an upper bound for $A$.**

First we will prove that if $x$ is an upperbound of $A$, then $x \not \in A$. For all $a \in A$, $a \leq x$ by *Axiom 3*. By *Definition 6.1 (c)*, we know there does not exist an $a \in A$ where $a = x$ thus, $a \neq x$ which means $x \not \in A$ because $x$ is not a last point and it's an upper bound, which is given. 

Next we will prove that if $x \not \in A$, then $x$ is an upper bound of $A$ where $A$ is a Dedekind cut. We will prove this by contradiction where we assume for the sake of contradiction such that if $x$ is not an upper bound, then $x \in A$. Then this means there exists an $a \in A$ such that $x < a$ and $x \in \mathbb{Q}$ and $x < a$, then $x \in A$ by *Definition 6.1 (b)*. 

**Exercise 6.3:
(a) Prove that, for any $q ∈ \mathbb{Q}, {x ∈ \mathbb{Q} | x < q}$ is a Dedekind cut. We then define $0 = {x ∈ \mathbb{Q} | x < 0}$. 
(b) Prove that ${x ∈ \mathbb{Q} | x ≤ 0}$ is not a Dedekind cut.
 (c) Prove that ${x ∈ \mathbb{Q} | x < 0} ∪ {x ∈ \mathbb{Q} | x^2 < 2}$ is a Dedekind cut.**

(a)
$A = \{x \in \mathbb{Q} | x < q\}$ then $A$ is nonempty. If $r$ is in the set $A$ and $s < r$ then $s \in A$ this is because $s < r < q$ which implies $s < q$ by transitivity thus $s \in A$. There is no last point because $r < \frac {r+q} 2 < q$ and $r$ canoot be the last point because there exists an $x \in A$ that is greater.    

(b)
$\{x \in \mathbb{Q} | x \leq 0\}$ has a last point because zero is the last point. 

(c)
Use *Theorem 5.18* which means there is no last point. 

**Exercise 6.5: Show that $\R$ satisfies Axioms 1,2 and 3.**
*Axiom 1: A continuum is a nonempty.*
*Axiom 2: A continuum has an ordering $<$.*
*Axiom 3: A continuum has no first or last point.*
**Fix Trichotomy, more on transistivity, more on 3**

1. Choose any element in $\R$ such as 0 from *Theorem 6.3* such that it is an Dedekind cut < 0, which proves $\R$ is not empty.
2. For the continuum to have an ordering, it must satisfy 2 conditions:
   1. Trichotomy: between two elements $X,Y \in \R$ that are Dedekind cuts (subsets of $\mathbb{Q}$) must have a relation either <, >, or =. We can prove this by contradiction. Suppose that $X \not \sub Y$ and $Y \not \sub X$. Then there exists an $x \in X$ such that $x \not \in Y$ and there exists a $y \in Y$ such that $y \not \in X$. Assume that $x < y$, and we know that $x \in \mathbb{Q}$ satisfies $x < y$ and $x \not \in Y$. Therefore, we can say that $Y$ is not a Dedekind cut by *Theorem 6.1*, because $x<y$ and does not exist in the set $Y$ which contradicts the definition of a Dedekind. This means it is not true that two. Then for any Dedekind cuts $X,Y$, eithher $X \sub Y$, $Y \sub X$, or $Y\sub X$ and $X \sub Y$ such that $X = Y$ which proves trichotomy.
   2. Transitivity: If $A < B$, $B < C$, then $A < C$ where $A,B,C$ are Dedekind cuts. By *Definition 6.4*, this is equivalent to saying $A \sub B$, $B \sub C$, and supposedly $A \sub C$. This is proven by *Theorem*
3. There exists a point $c$ that is not an element of $L$. By *Theorem 6.2*, $c$ must be an upperbound of $L$ such that we can define a Dedekind cut such that $L<C$ which contradicts our assumption that there can be no greatest cut $L$.

**Lemma 6.6: A nonempty subset of $\R$ that is bounded above has a supremum.**
Let us define $A = \bigcup _{B\in X}B$ where every $B$ is a Dedekind cut such that $A$ is the union of all Dedekind cuts in $\R$. We want to prove that $A$ itself is also a Dedekind cut. Since $X$ is nonempty, then it must contain some $B \in X$ such that $B \neq \empty$. Therefore,  there exists some $b \in B$ since $B$ is nonempty, and because $B \sub A$ (prove this), then $b \in A$ such that $A$ is also nonempty. We also know that $X$ is bounded above, so for all all $B \sub A$, there must exist some Dedekind cut $ Y \in \R$ where $Y \geq B$ such that $Y$ is the upperbound of $X$. Because $R$ has no last point by *Axiom 3* there must exist some $Z \in \R$ such that $Z > Y$, and by transitivity, for all $B$, $B < Z$.

Therefore there must exist some $z \in Z$ such that $z \in \mathbb{Q}$ and $z \not \in B$ for all $B$. Thus, $z \not \in A$ which means $A \neq \mathbb{Q}$.

Let $b \in A$ and because $A$ is the union of all $B$, then $b$ must exist in some $B$. If $q <  b$ where $q \in \mathbb{Q}$, then $q \in B$ and because $B \sub A$, then $q \in A$.

In order for $A$ to be a Dedekind cut, it cannot have a last point. For some $b \in B$, there exists some $s \in B$ such that $ s > b$ because $B$ is a Dedekind cut. Since $B \sub A$, then $s \in A$. Then for all $B \in A$, the $ b < s$. Thus $A$ is a Dedekind cut.

We want to show $A$ is the upper bound of $X$. For all $B \in X$ that are also in $A$, then $X \sub A$ by *Lemma 3.4* $B \leq A$ for all $B \in X$ which is the definition of a an upper bound by *Definition 5.5*. Thus $A$ is an upper bound of $X$. Assume for the sake of contradiction that there exists some $U$ where $U$ is an upper bound of $X$ and $U < A$. If $ u \in U$ and $U < A$, then $u \in B$ therefore $u \in A$ so $U \in A$ thus $U \sub A$ but $A \not \sub U$ such that $ U < A$ so $U$ cannot be an upper bound of $X$.
**MORE**


**Exercise 6.7: Show that $\R$ satisfies *Axiom 4***

We will prove this by contradiction and suppose that $\R$ is disconnected. This means that there exists $A,B$ which are Dedekind cuts that are subsets of $R$ which are disjoint, nonempty, and open such that $A \cap B = \empty$ and $A \cup B = \R$. Suppose without loss of generality that $a in A$, $b \in B$, and $a < b$. Then $A$ is bounded above and by *Lemma 6.6*, we know that sup $A$ exists which we can set equal to $u$.
Case 1: $u \in A$: Since $A$ is open, by *Theorem 4.9*, $u \in R \sub A$. Then we know that there exists an $x \in R$ and $u < x$ thus $u$ cannot be the sup$A$ because it is not even an upper bound. This proves that $u \not \in A$.
Case 2: $u \in B$: Since $B$ is open, by *Theorem 4.9*, there exists a region $u \in R_2 \in B$ and there exists a $y \in R_2$ such that $y < u$, but there cannot be an element less than $u$ because $u$ would no longer be the sup$A$ because there exists a elements in $R_2$ which are upper bounds. Thus $u \not \in B. 


**Lemma 6.9: A subset $X ⊂ C$ is dense in $C$ if, and only if, $\overline{X} = C$.**

First, let us prove that $\overline{X}$ = $C$ given that $X$ is dense in $C$. $X$ is dense in $C$ if every $p$ in $C$ is a limit point of $X$. Remember that the closure of $X$ is $\overline{X} = LP(X) \cup X$, and because density essentially states that $C = LP(X)$ because $C \sub LP(X)$ and $LP(X) \sub C$, then $\overline{X} = C \cup X$, but because no elements of a set $X$ can be outside of its continuum $C$ such that $X \sub C$, then $\overline{X} = C$.



Now, let us prove the reverse direction: given $\overline{X} = C$, we need to prove that $X$ is dense in $C$ such that every $p$ in $C$ is a limit point of $X$. Density states that $C = LP(X)$, and we know that $\overline{X} = LP(X) \cup X$, so $\overline{X} = C \cup X$, and similar to our first proof, $X \sub C$, so $C \cup X = C$ such that $\overline{X} = C$.

**Second part needs revision**

**Lemma 6.10: Given $A, B \in R$, there exists $p \in \mathbb{Q}$ such that $A < i(p) < B$.**

$A << B$ implies $A \sub B$ by *Theorem 6.4*.   

**Theorem 6.11: $i(\mathbb{Q})$ is dense in $\R$**
To prove that $i(\mathbb{Q})$ is dense in $\R$, we can equivalently prove that $\overline {i(\mathbb{Q})} = \R$ as shown in *Lemma 6.9*. Remember that the closure of a set is the union of the set and its limit points

To prove that \( i(\mathbb{Q}) \), the image of the rationals under the image \( i \) in \( \R \), is dense in \( \R \), we need to demonstrate that every real number is either a rational number or a limit point of the rationals.

1. **Closure of \( i(\mathbb{Q}) \) Includes \( i(\mathbb{Q}) \):**
   - By definition, the closure of a set includes the set itself. Therefore, \( \overline{i(\mathbb{Q})} \) includes \( i(\mathbb{Q}) \).

2. **Limit Points of \( i(\mathbb{Q}) \) are in \( \overline{i(\mathbb{Q})} \):**
   - From *Lemma 6.10*, for any two elements \( A, B \in \R \) with \( A < B \), there exists a rational \( p \in \mathbb{Q} \) such that \( A < i(p) < B \). This implies that for every region in \( \R \), there is a rational number in \( \mathbb{Q} \) whose image under \( i \) lies within that interval. 
   - Therefore, for any real number \( r \in \R \), and for any region \( R \) containing \( r \), there is always a rational number \( q \) in \( \mathbb{Q} \) such that \( i(q) \) lies in \( R \). This makes every real number \( r \) a limit point of \( i(\mathbb{Q}) \).

3. **Every Point in \( \R \) is Either in \( i(\mathbb{Q}) \) or a Limit Point of \( i(\mathbb{Q}) \):**
   - Since \( \mathbb{Q} \) is dense in \( \R \), every real number is arbitrarily close to some rational number. Thus, every real number is either in \( i(\mathbb{Q}) \) or a limit point of \( i(\mathbb{Q}) \) because there will always exist at least another element in the intersection such that: $i(p) \cup R \backslash \{r\} \neq \empty$ which means every $r$ is a limit point of $i(\mathbb{Q})
  
4. **Closure Equals \( \R \):**
   - Combining the above points, since every real number is either in \( i(\mathbb{Q}) \) or a limit point of \( i(\mathbb{Q}) \), the closure of \( i(\mathbb{Q}) \) must be the entire set of real numbers, \( \R \).

5. **Conclusion:**
   - Therefore, \( \overline{i(\mathbb{Q})} = \R \), confirming that \( i(\mathbb{Q}) \) is dense in \( \R \).