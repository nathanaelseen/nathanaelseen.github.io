---
layout: page
title: Richard Goldberg Exercise 2.1 Q5
description: Discusses the given question, the intuition behind the proof, and the proof itself
---

In this section, I will discuss the given question, the intuition behind the proof, and the
proof itself.

---

_**Question**_

Let $$S$$ be a sequence. Prove that every subsequence of a subsequence of S is itself a subsequence
of S.

_**Intuition**_

_**Proof**_

Let S be a sequence in the set $$A$$.

We note that, it is given by the function; $$f: \mathbb{N} \rightarrow A$$.

Now, consider an (arbitary) subsequence $$S'$$ of $$S$$,which has the form $$f \circ g$$,
where $$h: \mathbb{N} \rightarrow \mathbb{N}$$, satisfies $$h(n) < h(n + 1)$$,
for all $$n$$.

A subsequence $$S''$$ of $$S'$$ has the form $$(f \circ g) \circ h$$, where
$$h: \mathbb{N} \rightarrow \mathbb{N}$$.

(Claim: $$(g \circ h)(n) < (g \circ h)(n + 1)$$, $$\forall n \in \mathbb{N}$$)

We note that $$h(n) < h(n + 1)$$, and $$g(n) < g(n + 1)$$.

Now, let $$b = h(n)$$, and $$c = h(n + 1)$$.

Now, $$b < c$$, since $$h(n) < h(n + 1)$$.

Thus, $$b < b + 1 \leqslant c$$ (due to composite function $$g(h(n))$$)
$$ => g(b) < g(b + 1) \leqslant g(c)$$ $$ => g(b) < g(c)$$ $$ => g(h(n)) < g(h(n + 1))$$,
as needed. $$\blacksquare$$
