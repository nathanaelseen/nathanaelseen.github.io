---
layout: page
title: Richard Goldberg Exercise 2.4 Q3
description: Discusses the given question, the intuition behind the proof, and the proof itself
---

In this section, I will discuss the given question, the intuition behind the proof, and the
proof itself.

---

_**Question**_

Prove that $$\left(\sqrt{n + 1} - \sqrt{n}\right)_{n=1}^\infty$$ is convergent.

(Hint: Recall how to find $$\dfrac{dy}{dx}$$ by the $$\Delta x$$ process when $$y = \sqrt{x}$$.)

[//]: # _**Intuition**_

_**Proof**_

First, note that $$\sqrt{n + 1} - \sqrt{n}$$
$$ = \dfrac{\left(\sqrt{n + 1}\right)\left(\sqrt{n + 1} + \sqrt{n}\right) - \sqrt{n}\left(\sqrt{n + 1} + \sqrt{n}\right)}{\sqrt{n + 1} + \sqrt{n}}$$
$$ = \dfrac{(n + 1) + \sqrt{n(n + 1)} - \sqrt{n(n + 1)} - n}{\sqrt{n + 1} + \sqrt{n}}$$
$$ = \dfrac{1}{\sqrt{n + 1} + \sqrt{n}} \leqslant \dfrac{1}{2 \sqrt{n}}$$.

Now, let, $$\epsilon > 0$$, be given.

Pick, $$N \in \mathbb{N} \ni N > {\left(\dfrac{1}{2\epsilon}\right)}^2$$
$$ <=> {\left(\dfrac{1}{2\epsilon}\right)}^2 < N$$ $$ <=> \dfrac{1}{2\epsilon} < \sqrt{N}$$
$$ <=> 1 < \epsilon \left(2 \sqrt{N}\right)$$ $$ <=> \dfrac{1}{2 \sqrt{N}} < \epsilon$$
$$ <=> \left\lvert \dfrac{1}{2 \sqrt{N}} - 0 \right\rvert < \epsilon$$.

Then, for $$n \geqslant N$$, $$\dfrac{1}{n} \leqslant \dfrac{1}{N}$$
$$ <=> \dfrac{1}{2 \sqrt{n}} \leqslant \dfrac{1}{2 \sqrt{N}}$$
$$ <=> \left\lvert \dfrac{1}{2 \sqrt{n}} - 0 \right\rvert \leqslant \left\lvert \dfrac{1}{2 \sqrt{N}} - 0 \right\rvert < \epsilon$$
$$ => \left\lvert \dfrac{1}{2 \sqrt{n}} - 0 \right\rvert < \epsilon$$
$$ => \left\lvert \left(\sqrt{n + 1} - \sqrt{n}\right) - 0 \right\rvert < \epsilon$$.

Thus, $$\lim\limits_{n \to \infty} \left(\sqrt{n + 1} - \sqrt{n}\right) = 0$$. $$\blacksquare$$
