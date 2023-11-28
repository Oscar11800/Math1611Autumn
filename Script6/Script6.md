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



**Exercise 6.6: A nonempty subset of R that is bounded above has a supremum.**



**Exercise 6.7: Show that $R$ satisfies *Axiom 4***

**Lemma 6.9**