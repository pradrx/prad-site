---
toc: true
order: 5
layout: default
---

# Direct and Semidirect Products and Abelian Groups

## Direct Products

**Definition**: The **direct product** $G_1 \times G_2 \times \dots$ for groups $G_1, G_2, \dots$ with operations $\star_1, \star_2, \dots$, respectively, is the set of $n$-tuples $(g_1, \dots, g_n)$ (if finite) or sequences (if infinite) with the operation defined componentwise.

**Proposition 1**: If $G_1, \dots, G_n$ are groups, their direct product is a group of order $\prod \vert G_i \vert$ (if any $G_i$ is infinite, so is the direct product).

*Proof*: Trivial.

**Proposition 2**: Let $G_1, \dots, G_n$ be groups and $G$ their direct product.
1. $G_i \cong \lbrace (1, \dots, 1, g_i, 1, \dots, 1) \mid g_i \in G_i \rbrace$ and $G_i \trianglelefteq G$ with

$$
G/G_i \cong G_1 \times \dots \times G_{i - 1} \times G_{i + 1} \times \dots \times G_n
$$

2. For each fixed $i$ one can define $\pi_i: G \to G_i$ by $\pi_i(g_1, \dots, g_n)) = g_i$, which is a surjective homomorphism with kernel $G/G_i$.
3. If $x \in G_i$ and $y \in G_j$ for $i \neq j$, then $xy = yx$.

*Proof*: $(1)$ The map for the first isomorphism is given by $g_i \mapsto (1, \dots, 1, g_i, 1, \dots, 1)$. For the second part, note that 

$$
\varphi: G \to G_1 \times \dots \times G_{i  -1} \times G_{i + 1} \times \dots \times G_n
$$

defined by $(\varphi(g_1, \dots, g_n)) = (g_1, \dots, g_{i - 1}, g_{i + 1}, \dots, g_n)$ is a homomorphism with kernel $G_i$.

$(2)$ It is clear that this map is a surjective homomorphism: to see the kernel note that $G/G_i \cong \lbrace (g_1, \dots, g_{i - 1}, 1, g_{i + 1}, \dots, g_n) \mid g_j \in G_j \forall j \neq i \rbrace$.

$(3)$ Trivial.

$\blacksquare$

## The Fundamental Theorem of Finitely Generated Abelian Groups

**Definition**: $G$ is **finitely generated** if there exists a finite $X \subseteq G$ such that $G = \langle X \rangle$.

**Definition**: Let $r \in \mathbb Z_{\geq 0}$. Then $\mathbb Z^r = \mathbb Z \times \dots \times \mathbb Z$ ($r$ times) is the **free Abelian group of rank $r$**. When $r = 0$, $\mathbb Z^0 = 1$.

**Examples**:
1. $\mathbb Z$ is finitely generated by $\lbrace 1 \rbrace$
2. $\mathbb Z^n$ is finitely generated by $\lbrace (1, 0, \dots, 0), (0, 1, 0, \dots, 0), \dots, (0, 0, \dots, 0, 1) \rbrace$.

**Theorem 3 (Fundamental Theorem of Finitely Generated Abelian Groups, Invariant Form)**: Let $G$ be a finitely generated Abelian group. Then
1. $G \cong \mathbb Z^r \times Z_{n_1} \times \dots \times Z_{n_s}$ for some $r \geq 0$ and $n_j \geq 2$. such that $n_j \mid n_{j - 1} \mid \dots \mid n_2 \mid n_1$
2. The decomopsition in $(1)$ is unique and called the **invariant decomposition of $G$**. That is, if also $G \cong \mathbb Z^t \times Z_{m _1} \times \dots \times Z_{m_k}$ with the same constraints, then $r = t$ and $k = s$, and $m_j = n_j$, for all $j$.

*Proof*: Ring theory. $\blacksquare$

**Definition**: The exponent $r$ in the $\mathbb Z^r$ term of the invariant decomposition is called the **Betti number of $G$** or the **free rank of $G$**, and $n_1, \dots, n_s$ are the **invariants of $G$**.

**Remarks**:
1. If $G$ is **Abelian** , then $T(G) = \lbrace g \in G : \vert g \vert \lt \infty \rbrace \leq G$ is the **torsion component** of $G$. Also, $T(G) \cong Z_{n_1} \times \dots \times Z_{n_s}$.
2. $G$ is a Abelian group if its free rank is 0.
3. Suppose $G$ is a finite abelian group with $\vert G \vert = n$. Then $n = \prod n_i$. Let $p$ be prime. Then if $p \mid n$ then $p \mid n_1$.

**Corollary 4**: If $n$ is the product of distinct primes, h

**Remark**: $G$ is an Abelian group if its free rank is 0.

*Proof*: 

**Example**: $T(G)$ isn't necessarily a subgroup of $G$ isn't Abelian.

**Note**: 