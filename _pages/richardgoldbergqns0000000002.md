---
layout: page
title: Richard Goldberg Exercise 2.1 Q6
description: Discusses the given question, the intuition behind the proof, and the proof itself
---

In this section, I will discuss the given question, the intuition behind the proof, and the
proof itself.

---

_**Question**_

If $$(s_{n_k})_{k=1}^{\infty}$$ is a subsequence of $$(s_n)_{n=1}^{\infty}$$, prove that
$$n_k \geqslant k$$ $$(k \in N)$$.

[//]: # _**Intuition**_

_**Proof**_

We note that a subsequence of $$S$$ has the form; $$S \circ N$$, where
$$N: \mathbb{N} \to \mathbb{N}$$, and that $$N(k) < N(k + 1)$$,
$$\forall k \in \mathbb{N}$$.

Also, $$N(k) = n_k$$. Thus, $$n_k < n_{k + 1}$$.

(Claim: $$n_k \geqslant k$$)

Base Case: $$k = 1$$

Then, it is obvious, that $$n_1 \geqslant 1$$.

Inducitve Step:

Assume that, $$n_k \geqslant k$$. (WTS: $$n_{k + 1} \geqslant k + 1$$)

Consider, $$n_{k + 1}$$.

Since, $$n_k < n_{k + 1}$$, then $$k \leqslant n_k < n_{k + 1} + 1$$
$$ => k + 1 < n_{k + 1} < n_{k + 1} + 1$$ $$ => k + 1 < n_{k + 1}$$.

Thus, by Induction, $$n_k \geqslant k$$ $$(\forall k \in \mathbb{N})$$, and the
Theorem is proved. $$\blacksquare$$
