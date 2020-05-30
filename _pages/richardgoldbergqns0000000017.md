---
layout: page
title: Richard Goldberg Exercise 2.7 Q4
description: Discusses the given question, the intuition behind the proof, and the proof itself
---

In this section, I will discuss the given question, the intuition behind the proof, and the
proof itself.

---

_**Question**_

Suppose $$(s_n)_{n=1}^\infty$$ is a sequence of positive numbers and $$0 < x$$ $$ < 1$$. If
$$s_{n + 1} < xs_n$$ $$(\forall n \in \mathbb{N})$$, prove $$\lim\limits_{n \to \infty} s_n = 0$$.

[//]: # _**Intuition**_

_**Proof**_

Since, $$s_{n + 1} < xs_n$$ $$ < s_n$$, as $$0 < x < 1$$, and $$s_n > 0$$, the sequence
is monotonically nonincreasing; $$s_1 > s_2$$ $$ > ... > s_k$$ $$ > s_{k + 1} > ...$$.

Also, since the sequence $$(s_n)_{n=1}^\infty$$ only contains positive terms, it is
bounded below.

In particular $$0$$ is a l.b.

Hence, $$(s_n)_{n=1}^\infty$$ converges, to some $$L \in \mathbb{R}$$.

Now, $$s_{n + 1} < xs_n$$, and taking limits;
$$\lim\limits_{n \to \infty} s_{n + 1} \leqslant \lim\limits_{n \to \infty} xs_n$$
$$ = x \lim\limits_{n \to \infty} s_n$$.

Also, $$L \leqslant xL$$, since $$(s_{n + 1})_{n=1}^\infty$$ is a subsequence of
$$(s_n)_{n=1}^\infty$$ $$ => xL - L \geqslant 0$$ $$ => L(x - 1) \geqslant 0$$.

But, since $$0 < x < 1$$, $$L = 0$$. $$\blacksquare$$
