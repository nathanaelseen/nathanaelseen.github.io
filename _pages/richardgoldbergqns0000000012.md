---
layout: page
title: Richard Goldberg Exercise 2.5 Q4
description: Discusses the given question, the intuition behind the proof, and the proof itself
---

In this section, I will discuss the given question, the intuition behind the proof, and the
proof itself.

---

_**Question**_

If the sequence $$(s_n)_{n=1}^\infty$$ is bounded, prove that for any $$\epsilon > 0$$ there is a
closed interval $$J \subset \mathbb{R}$$ of length $$\epsilon$$ such that $$s_n \in J$$ for
infinitely many values of $$n$$.

[//]: # _**Intuition**_

_**Proof**_

Let $$\epsilon > 0$$, be given.

Since, the sequence $$(s_n)_{n=1}^\infty$$ is bounded,
$$\exists M \in \mathbb{R} \ni \left\lvert s_n \right\rvert \leqslant M$$
$$(\forall n \in \mathbb{N})$$ $$ => -M \leqslant s_n \leqslant M$$
$$(\forall n \in \mathbb{N})$$.

Now, we note that within the closed interval $$[-M, M]$$, the number of terms in
$$(s_n)_{n=1}^\infty$$ is (countably) infinite.

Also, the closed interval has length $$2M > 0$$.

Now, we could divide this interval into $$2$$ parts of length; $$2M - \epsilon$$ and
$$\epsilon$$ respectively, such that each part has $$N_1$$ and $$N_2$$ terms and the total
number of terms is $$N = N_1 + N_2$$.

(Here, we note that $$\epsilon < 2M$$.)

Since $$N$$ is countably infinite, we can infer that either both $$N_1$$ and $$N_2$$ are
countably infinite, or that one of them is.

In either case, one of them is (guaranteed) to be countably infinite, and hence
we obtain a set $$J \subseteq \mathbb{R}$$ of finite arbitrary length, which
contains infinite elements.

Now, for the case of any $$\epsilon \geqslant 2M$$, we can always box our closed interval $$[-M, M]$$,
with that $$\epsilon > 0$$.

Thus, for that $$\epsilon$$, all infinite elements of the sequence $$(s_n)_{n=1}^\infty$$
is present there. $$\blacksquare$$
