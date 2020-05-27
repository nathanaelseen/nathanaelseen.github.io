---
layout: page
title: Richard Goldberg Exercise 2.4 Q6
description: Discusses the given question, the intuition behind the proof, and the proof itself
---

In this section, I will discuss the given question, the intuition behind the proof, and the
proof itself.

---

_**Question**_

Suppose that $$(s_n)_{n=1}^\infty$$ converges to $$L \ne 0$$. Prove that $$((-1)^n s_n)_{n=1}^\infty$$
oscillates.

[//]: # _**Intuition**_

_**Proof**_

Let $$M > 0$$, be given.

We note that, $$(s_n)_{n=1}^\infty$$ converges to some $$L \ne 0$$.

However, assume the contrary, that instead, $$(s_n)_{n=1}^\infty$$ does not oscillate.

Then, either, it diverges to infinity, or minus infinity, and there are 2 Cases.

Case A: $$((-1)^n s_n)_{n=1}^\infty$$ diverges to infinity

Then, $$\exists N \in \mathbb{N} \ni (-1)^n s_n \geqslant M$$ $$(n \geqslant N)$$.

Here again, there are 2 sub-Cases; $$(-1)^n = -1$$ or $$(-1)^n = 1$$.

Case A1: $$(-1)^n = -1$$

Then, $$-s_n \geqslant M$$ $$ => s_n \leqslant -M$$ $$(n \geqslant N)$$.

Hence, $$(s_n)_{n=1}^\infty$$ diverges to minues infinity.

But, from our hypothesis, it converges to some $$L \ne 0$$. Contradiction.

Case A2: $$(-1)^n = 1$$

Then, $$s_n \geqslant M$$ $$(n \geqslant N)$$.

Thus, $$(s_n)_{n=1}^\infty$$ diverges to infinity

But, from our hypothesis, it converges to some $$L \ne 0$$. Contradiction.

Case B: $$((-1)^n s_n)_{n=1}^\infty$$ diverges to minus infinity

Thus, $$\exists N \in \mathbb{N} \ni (-1)^n s_n \leqslant -M$$ $$(n \geqslant N)$$.

Similarly, as with Case A, there are 2 sub-Cases; $$(-1)^n = -1$$ or $$(-1)^n = 1$$.

Case B1: $$(-1)^n = -1$$

Then, $$-s_n \leqslant -M$$ $$ => s_n \geqslant M$$ $$(n \geqslant N)$$.

Hence, $$(s_n)_{n=1}^\infty$$ diverges to infinity.

But again, from our hypothesis, it converges to some $$L \ne 0$$. Contradiction.

Case B2: $$(-1)^n = 1$$

Then, $$s_n \leqslant -M$$, and $$(s_n)_{n=1}^\infty$$ diverges to minus infinity.

But again, from our hypothesis, it converges to some $$L \ne 0$$. Contradiction.

Since, in all Cases, we arrive at a Contradiction, the theorem is true, and
$$(s_n)_{n=1}^\infty$$ indeed oscillates. $$\blacksquare$$
