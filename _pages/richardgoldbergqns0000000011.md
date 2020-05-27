---
layout: page
title: Richard Goldberg Exercise 2.5 Q3
description: Discusses the given question, the intuition behind the proof, and the proof itself
---

In this section, I will discuss the given question, the intuition behind the proof, and the
proof itself.

---

_**Question**_

Prove that if $$lim_{n \to \infty} \dfrac{s_n}{n} = L \ne 0$$, then $$(s_n)_{n=1}^\infty$$
is not bounded.

[//]: # _**Intuition**_

_**Proof**_

Let $$\epsilon > 0$$, be given.

Also, assume the contrary, that $$(s_n)_{n=1}^\infty$$ is bounded.

Then, $$\exists M \in \mathbb{R} \ni \lvert s_{n_1} \rvert \leqslant M$$
$$(\forall n_1 \in \mathbb{N})$$.

(In particular, let's claim that $$lim_{n \to \infty} \left(\dfrac{s_n}{n}\right) = 0$$.)

Pick, $$N \in \mathbb{N} \ni N > \dfrac{M}{\epsilon}$$ $$ <=> N\epsilon > M$$
$$ <=> N\epsilon > s_{n_1}$$ $$ <=> s_{n_1} < N\epsilon$$
$$ <=> \dfrac{s_{n_1}}{N} < \epsilon$$
$$ <=> \left\lvert \dfrac{s_{n_1}}{N} \right\rvert < \epsilon$$ $$(\forall n_1 \in \mathbb{N})$$

Thus, for $$n \geqslant N$$,
$$\left\lvert \dfrac{1}{n} \right\rvert \leqslant \left\lvert \dfrac{1}{N} \right\rvert$$
$$ => \left\lvert \dfrac{s_{n_1}}{n} \right\rvert \leqslant \left\lvert \dfrac{s_{n_1}}{N} \right\rvert$$
$$ < \epsilon$$ $$(\forall n_1 \in \mathbb{N})$$.

Hence, we have found an $$N$$, where, $$\left\lvert \dfrac{s_{n_1}}{n} - 0 \right\rvert < \epsilon$$
$$(n \geqslant N$$, and $$\forall n_1 \in \mathbb{N})$$.

Thus, $$lim_{n \to \infty} \dfrac{s_n}{n} = 0$$, as needed. $$\blacksquare$$
