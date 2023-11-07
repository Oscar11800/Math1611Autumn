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
