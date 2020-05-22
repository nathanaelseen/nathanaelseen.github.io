---
layout: page
title: Richard Goldberg Exercise 2.10 Q6
description: Discusses the question and the intuition behind the proof, and the solution itself
---

In this section, I will discuss the given question and the intuition behind the proof, and the
solution itself.

---

_**Question**_

Let $$(a_n)_{n=1}^{\infty}$$ be a sequence of real numbers, and, for each $$n \in \mathbb{N}$$, let

$$s_n = a_1 + a_2 + ... + a_n$$,

$$t_n = \mid a_1 \mid + \mid a_2 \mid + ... + \mid a_n \mid$$.

Prove that if $$(t_n)_{n=1}^{\infty}$$ is a Cauchy sequence, then so is $$(s_n)_{n=1}^{\infty}$$.

_**Intuition**_

_**Proof**_

Let $$\epsilon > 0$$, be given.

Since $$(t_n)_{n=1}^{\infty}$$ is Cauchy, $$\exists N \in \mathbb{N} \ni \mid t_m - t_n \mid < \epsilon$$
$$(m,n \geqslant N)$$.

But, we note that, $$\mid s_m - s_n \mid = \mid (a_1 + ... + a_m) - (a_1 + ... + a_n) \mid$$
$$ = \mid a_n + a_{n + 1} +  ... + a_m \mid$$
$$ \leqslant \mid a_n \mid + \mid a_{n + 1} \mid + ... + \mid a_m \mid$$
$$ = t_m - t_n = \mid t_m - t_n \mid$$ $$< \epsilon$$ $$(m, n \geqslant N)$$.

Thus, $$\mid s_m - s_n \mid < \epsilon$$
$$(m, n \geqslant N)$$.

Hence, $$(s_n)_{n=1}^{\infty}$$ is Cauchy. $$\blacksquare$$
