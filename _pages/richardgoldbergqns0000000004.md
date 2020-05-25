---
layout: page
title: Richard Goldberg Exercise 2.2 Q2
description: Discusses the given question, the intuition behind the proof, and the proof itself
---

In this section, I will discuss the given question, the intuition behind the proof, and the
proof itself.

---

_**Question**_

If $$L \in \mathbb{R}$$, $$M \in \mathbb{R}$$, and $$L \leqslant M + \epsilon$$ for every
$$\epsilon > 0$$, prove that $$L \leqslant M$$.

[//]: # _**Intuition**_

_**Proof**_

Let $$\epsilon > 0$$, be given.

Suppose the contary, that $$L > M$$.

Then, $$L \leqslant M + \epsilon$$.

Thus, $$M < L \leqslant M + \epsilon$$ $$ => M - \epsilon < L \leqslant M + \epsilon$$
(since $$\epsilon > 0$$) $$ => \lvert L - M \rvert < \epsilon$$ $$(\forall \epsilon > 0)$$.

But, in particular, pick an $$\epsilon_a < \lvert L - M \rvert < \epsilon_a$$.

Thus, $$\epsilon_a < \epsilon_a$$, which is a Contradiction.

Hence, the theorem is true. $$\blacksquare$$
