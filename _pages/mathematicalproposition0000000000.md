---
layout: page
title: Mathematical Proposition
description: Discusses the given proposition, the intuition behind the proof, and the proof itself
---

In this section, I will discuss the given proposition, the intuition behind the proof, and the
proof itself.

---

_**Question**_

Let $$A$$ and $$B$$ be nonempty subsets of $$\mathbb{R}$$ that are  both bounded above.

Define, $$A + B = \{a + b: a \in A, b \in B\}$$.

Show that $$A + B$$ is bounded above, and that, $$sup(A + B) = sup A + sup B$$

_**Intuition**_

_**Proof**_

Since $$A$$ and $$B$$ are bounded above, then,

$$a \leqslant sup A$$, $$\forall a \in A$$, and,

$$b \leqslant sup B$$, $$\forall b \in B$$.

Hence, $$a + b \leqslant sup A + sup B$$, $$\forall (a + b) \in A + B$$.

Thus, $$A + B$$ is bounded above.

(Claim: $$sup A + sup B = sup (A + B)$$)

Suppose the contrary, that $$sup A + sup B \ne sup (A + B)$$.

Then $$\exists x \in \mathbb{R} \ni a + b \leqslant x < sup A + sup B$$
$$(\forall a \in A, b \in B)$$

Hence, $$x < sup A + sup B => x - sup A < sup B$$.

(Claim: $$x - sup A < b$$, $$\forall b \in b$$)

Suppose to the contrary, that $$x - sup A \geqslant b$$, instead.

Then, $$b \leqslant x - sup A$$, and $$x - sup A$$ is an u.b of $$B$$.

Also, we have, $$b \leqslant sup B$$.

Hence, $$b \leqslant sup B \leqslant x - sup A$$, which contradicts,
$$x - sup A < sup B$$.

Thus, $$x - sup A < b => x - b < sup A$$.

(Claim: $$x - b < a$$)

Suppose to the contrary, that $$x - b \geqslant a$$, instead.

Then, $$a \leqslant x - b$$, and $$x - b$$ is an u.b of $$a$$.

Also, $$a \leqslant sup A$$.

Hence, $$a \leqslant sup A \leqslant x - b$$, which contradicts $$x - b < sup A$$.

Thus, $$x - b < a => x < a + b$$, $$\forall (a + b) \in A + B$$, which contradicts,
$$a + b \leqslant x$$.

Thus, $$sup A + sup B = sup (A + B)$$, as needed. $$\blacksquare$$
