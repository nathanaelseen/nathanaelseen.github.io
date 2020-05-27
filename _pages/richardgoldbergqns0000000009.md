---
layout: page
title: Richard Goldberg Exercise 2.4 Q5
description: Discusses the given question, the intuition behind the proof, and the proof itself
---

In this section, I will discuss the given question, the intuition behind the proof, and the
proof itself.

---

_**Question**_

Suppose that $$(s_n)_{n=1}^\infty$$ converges to $$0$$. Prove that $$((-1)^n s_n)_{n=1}^\infty$$
converges to $$0$$.

[//]: # _**Intuition**_

_**Proof**_

Let $$\epsilon > 0$$, be given.

Since, $$(s_n)_{n=1}^\infty$$ converges to $$0$$,
$$\exists N \in \mathbb{N} \ni \lvert s_n - 0 \rvert = \lvert s_n \rvert$$ $$ < \epsilon$$
$$(n \geqslant N)$$.

But, $$\lvert s_n \rvert = \lvert 1 \rvert \cdot \lvert s_n \rvert$$
$$ = \lvert (-1)^n \rvert \cdot \lvert s_n \rvert = \lvert (-1)^n s_n \rvert$$
$$ < \epsilon$$ $$(n \geqslant N)$$.

Thus, $$lim_{n \to \infty} (-1)^n s_n = 0$$. $$\blacksquare$$
