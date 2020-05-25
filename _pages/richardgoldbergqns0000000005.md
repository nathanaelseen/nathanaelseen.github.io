---
layout: page
title: Richard Goldberg Exercise 2.2 Q4(b)
description: Discusses the given question, the intuition behind the proof, and the proof itself
---

In this section, I will discuss the given question, the intuition behind the proof, and the
proof itself.

---

_**Question**_

Prove $$lim_{n \to \infty} \dfrac{2n}{n + 3} = 2$$.

[//]: # _**Intuition**_

_**Proof**_

Let $$\epsilon > 0$$, be given.

(WTS: $$lim_{n \to \infty} \dfrac{2n}{n + 3} = 2$$)

Pick, $$N \in \mathbb{N} \ni N \geqslant \dfrac{6}{\epsilon} - 3$$
$$ <=> N \geqslant \dfrac{6 - 3\epsilon}{\epsilon}$$
$$ <=> N\epsilon \geqslant 6 - 3\epsilon$$ $$ <=> N\epsilon + 3\epsilon \geqslant 6$$
$$ <=> \epsilon(N + 3) \geqslant 6$$ $$ <=> 6 \leqslant \epsilon(N + 3)$$
$$ <=> \dfrac{6}{N + 3} \leqslant \epsilon$$
$$ <=> \left\lvert \dfrac{2N - 2(N + 3)}{N + 3} \right\rvert \leqslant \epsilon$$
$$ <=> \left\lvert \dfrac{2N}{N + 3} - 2 \right\rvert < \epsilon$$.

Then, $$\left\lvert \dfrac{1}{n} \right\rvert \leqslant \left\lvert \dfrac{1}{N} \right\rvert$$
$$ => \left\lvert \dfrac{1}{n + 3} \right\rvert \leqslant \left\lvert \dfrac{1}{N + 3} \right\rvert$$
$$ => \left\lvert \dfrac{2n}{n + 3} \right\rvert \leqslant \left\lvert \dfrac{2N}{N + 3} \right\rvert$$
$$ => \left\lvert \dfrac{2n}{n + 3} - 2 \right\rvert \leqslant \left\lvert \dfrac{2N}{N + 3} - 2 \right\rvert$$
$$ < \epsilon$$.

Hence, we have found an $$N$$, where, $$\left\lvert \dfrac{2n}{n + 3} - 2 \right\rvert < \epsilon$$
$$(n \geqslant N)$$.

This proves, $$lim_{n \to \infty} \dfrac{2n}{n + 3} = 2$$, as needed. $$\blacksquare$$
