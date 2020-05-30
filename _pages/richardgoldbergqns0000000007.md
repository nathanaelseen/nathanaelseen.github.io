---
layout: page
title: Richard Goldberg Exercise 2.3 Q5
description: Discusses the given question, the intuition behind the proof, and the proof itself
---

In this section, I will discuss the given question, the intuition behind the proof, and the
proof itself.

---

_**Question**_

If $$(s_n)_{n=1}^\infty$$ is a sequence of real numbers and if $$\lim\limits_{m \to \infty} s_{2m} = L$$,
$$\lim\limits_{m \to \infty} s_{2m - 1} = L$$, prove that $$s_n \to L$$ as $$n \to \infty$$.

(That is, if the subsequence of $$(s_n)_{n=1}^\infty$$ of terms with even subscripts converges to
$$L$$, as well as the subsequence with odd subscripts, then $$(s_n)_{n=1}^\infty$$ converges to
$$L$$ also.)

[//]: # _**Intuition**_

_**Proof**_

Let $$\varepsilon > 0$$, be given.

Since, $$\lim\limits_{m \to \infty} s_{2m} = L$$,
$$\exists N_1 \in \mathbb{N} \ni \lvert s_{2m} - L \rvert < \varepsilon$$ $$(2m \geqslant N_1)$$.

Similarly, since, $$\lim\limits_{m \to \infty} s_{2m - 1} = L$$,
$$\exists N_2 \in \mathbb{N} \ni \lvert s_{2m - 1} - L \rvert < \varepsilon$$ $$(2m - 1 \geqslant N_2)$$.

Set $$N = \max\{N_1, N_2\}$$, then, in both cases, where $$m$$ is odd or even,
$$\exists N \in \mathbb{N} \ni \lvert s_m - L \rvert < \varepsilon$$ $$(m \geqslant N)$$.

Hence, $$\lim\limits_{m \to \infty} s_m = L$$, as needed. $$\blacksquare$$
