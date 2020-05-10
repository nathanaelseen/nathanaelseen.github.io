---
title: Order Complete Fields
description: Covers what an algebraic Field is and what it means for a Field to be order complete
---

## Order Complete Fields

In this section, we take a step back and look at (High School) Algebra, but from a more
abstract perspective.

In [Algebra](https://en.wikipedia.org/wiki/Algebra), a Field is a [Set](https://en.wikipedia.org/wiki/Set), by which two important
operations, namely; **Addition** and **Multiplication**, over the elements (in the Set) are defined.

_**Definition 1**_. A Field is a 5-tuple, denoted by; $$\langle F, +, \cdot, e, u \rangle$$, where
  - $$F$$ is a [Set](https://en.wikipedia.org/wiki/Set_(mathematics)) consisting of all the elements
    in the Field
  - $$+$$ is the Additive operator
  - $$\cdot\$$ is the Multiplicative operator
  - $$e \in F$$ is the Additive identity
  - $$u \in F$$ is the Multiplicative identity,

with the following axioms defined:
  1. $$\forall a,b \in F, a + b = b + a$$ (commutativity)
  1. $$\forall a,b \in F, (a + b) + c = a + (b + c)$$ (associativity)
  1. $$\forall a \in F, a + e = a$$ (Additive identity axiom)
  1. $$\forall a \in F, \exists b \in F \ni a + b = e$$ (existence of an Additive inverse)

  1. $$\forall a,b \in F, a \cdot b = b \cdot a$$ (commutativity)
  1. $$\forall a,b \in F, (a \cdot b) \cdot c = a \cdot (b \cdot c)$$ (associativity)
  1. $$\forall a \in F, a \cdot u = a$$ (Multiplicative identity axiom)
  1. $$\forall a \in F, \exists b \in F \ni a \cdot b = u$$ (existence of an Multiplicative inverse)

  1. $$\forall a,b,c \in F, a \cdot (b + c) = a \cdot b + a \cdot c$$ (distributivity)

Some common examples of fields include; $$\mathbb{N}$$, $$\mathbb{Q}$$, $$\mathbb{R}$$, and $$\mathbb{C}$$, where in
particular, $$\mathbb{N} \subseteq \mathbb{Q} \subseteq \mathbb{R} \subseteq \mathbb{C}$$.

In the context of $$\mathbb{R}$$, the Additive identity, $$e = 0$$, and the $$u = 1$$.

Just with this simple definition of a Field, we can jump right to proving some common algebraic expressions
we've seen before.

First of all, we want to verify that if $$a + b = a + c$$, then $$b = c$$.

_**Theorem 1**_. $$\forall a, b, c \in F$$, if $$a + b = a + c$$, then $$b = c$$.

_**Proof**_. By _axiom 4_, $$\exists d \in F$$ where $$a + d = e$$. Thus,
$$(a + b) + d = (a + c) + d$$ $$=> (a + d) + b = (a + d) + c$$ (by _axiom 1 and 2_).
Hence, $$e + b = e + c$$ $$=> b = c$$ (by _axiom 3_). $$\blacksquare$$

Next, we would like to verify that both the Additive and Multiplicative identity ($$e$$ and
$$u$$) are unique.

In the context of $$\mathbb{R}$$, this means there is no such other number; $$0'$$, which has
the same property as $$0$$, where when you add any number $$x$$ with it, you will get back
the same number $$x$$.

We will only prove the uniqueness of the Additive identity, and the proof for the Multiplicative
identity should be similar.

_**Theorem 2**_. $$\exists! e \in F$$, where $$\forall a \in F$$, $$a + e = a$$.

_**Proof**_. Suppose that $$\exists e, e' \in F$$, where $$\forall a \in F$$, $$a + e = a$$ and
$$a + e' = a$$. Then, by previous Theorem, $$e = e'$$. $$\blacksquare$$

Similar to the uniqueness of the identities, we now verify that $$\forall a \in F$$, their Additive
and Multiplicative inverses are also unique.

The proof for this is quite similar to the uniqueness proof above.

_**Theorem 3**_. $$\forall a \in F, \exists! b \in F \ni a + b = e$$

_**Proof**_. Suppose $$\forall a \in F, \exists b, b' \in F \ni a + b' = e$$.
Then, by previous Theorem, $$b = b'$$. $$\blacksquare$$

Notationally, $$\forall a \in F$$, we can denote their Additive and Multiplicative inverses by
$$-a$$ and $$a^{-1}$$ respectively.

We thus have $$a + (-a) = e$$ and $$a \cdot a^{-1} = u$$.

In $$\mathbb{R}$$, this would be $$a + (-a) = 0$$ and $$a \cdot a^{-1} = 1$$.

As with inverses, we present here a Theorem on the inverse of a Multiplicative inverse;
$$(a^{-1})^{-1}$$.

_**Theorem 4**_. $$\forall a \in F$$, if $$a \ne e$$ then $$(a^{-1})^{-1} = a$$.

_**Proof**_. We note that $$\forall a \in F, a^{-1} \cdot (a^{-1})^{-1} = e$$ and
$$a \cdot a^{-1} = e$$. Hence, $$a^{-1} \cdot (a^{-1})^{-1} = e$$ and $$a^{-1} \cdot a = e$$.
Thus, $$(a^{-1})^{-1} = a$$. $$\blacksquare$$

Next, we present a Theorem concerning 'division' of elements (or numbers if you will)
in a Field.

_**Theorem 5**_. $$\forall a, b \in F$$, where $$b \ne e$$, $$\exists! x \in F \ni a \cdot x = b$$.

_**Proof**_. _(to be updated soon)_

Notationally, we could also denote the $$x$$ satisfying $$ax = b$$, by $$x = \dfrac{b}{a}$$.

Similarly, we could also denote $$a^{-1}$$, by $$\dfrac{1}{a}$$.

At this juncture, an alert reader might notice that in both _Theorems 4_ and _5_, there are
restrictions on what you can 'divide' by and what can be 'divided'.

We shall tackle them one at a time.

Now, for _Theorem 4_, the restriction was on the fact that we couldn't 'divide' anything
by $$e$$ (or equivalently by $$0$$ in $$\mathbb{R}$$).

But is this restriction really necessary? Did the definition of the Field or any Theorems
cause this restriction?

Absolutely not, and we could actually thus remove it!

But suppose we removed it, then in the Proof (of _Theorem 4_),
specifically; $$a \cdot a^{-1} = e$$, if $$a = e$$, would that mean $$e^{-1}$$ (or
$$0^{-1}$$) actually exists?

(The gnawing question pops up again.)

The answer is yes it does!

But why then, in High School, do we keep trying to restrict the
expression $$0^{-1}$$ / $$\dfrac{1}{0}$$?

It is because, this expression, although valid does not make sense at all (dividing
something by _nothing_).

Hence to wrap things up, you could theoretically 'divide' by $$0$$, and hence
_Theorem 4_ is valid even with the current restriction on $$a \ne e$$ removed.

Now, as for _Theorem 5_, we actually need to keep the restriction there.

For suppose the restriction was removed and $$a \cdot x = b = e$$ $$=> a \cdot x = e$$.
Then either $$a = e$$ or $$x = e$$. But since we're trying an $$x$$, $$a = e$$.

_**Theorem 6**_. $$\forall a, b \in F$$, if $$a \cdot b = e$$, then either
$$a = e$$ or $$b = e$$.

_**Proof**_. _(to be updated soon)_

Now, if that's the case, then we run into trouble because anything Multiplied with
$$e$$, would give us back $$e$$.

(Note: $$e$$ seems to be a very special element that has this property, $$u$$
doesn't even have such a property)

_**Theorem 7**_. $$\forall a \in F$$, $$a \cdot e = e$$.

_**Proof**_. _(to be updated soon)_

Hence we could simply take any $$x \in F$$ to get our desired $$b = e$$, and
the uniqueness required in _Theorem 5_ thus breaks down!

Hence, in this case, we actually need the restriction of $$b \ne e$$ to be present.

With all these seemingly familiar algebraic expressions proved, a reader should be
able to deduce the rest of the common expressions from the abstract definition
f a Field.
