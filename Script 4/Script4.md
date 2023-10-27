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

case 2: $a = y$ which means $y \in R_1 \cap(x \backslash \{z\}) and by *theorem 3.21*, $y\in R_2$, $z \in R_3$, and $R_2 \cap R_3 = \empty$.
We can surmise that $z \in R_1 \cap R_3$ such that $(R_1 \cap R_3) \cap (x \backslash \{z\} \neq \empty)$. Let $b \in (R_1 \cap R_3) \cap (x \backslash \{z\}$ which means $b \in R_1 \cap R_3$ and $b\in X$ and $b \in R_1 \cap (x \backslash \{y\}) such that $y \in LP(X)$ which means $y \in \overline{X}$ and because all $LP(\overline{X} \sub X) then $\overline{X}$ is closed.  