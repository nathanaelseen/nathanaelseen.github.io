---
layout: subpage
title: Fields
description: Covers what an algebraic Field in abstract Algebra is, and various operations over a Field
---

In this section, we take a look at what an algebraic Field is, and the various operations
over a Field. Using Fields, we shall also discuss (High School) Algebra but from a more
abstract perpective.

---

In [Algebra](https://en.wikipedia.org/wiki/Algebra), a Field is a [Set](sets),
by which two important operations, namely; **Addition** and **Multiplication**, over the
elements (in the Set) are defined.

_**Definition 1**_. A Field is a 5-tuple, denoted by; $$\langle F, +, \cdot, e, u \rangle$$, where
  - $$F$$ is a [Set](sets) consisting of all the elements
    in the Field
  - $$+$$ is the Additive operator
  - $$\cdot$$ is the Multiplicative operator
  - $$e \in F$$ is the Additive identity
  - $$u \in F$$ is the Multiplicative identity,

with the following Axioms defined:
  1. <a name="axiom1"></a>$$\forall a,b \in F, a + b = b + a$$ (commutativity)
  1. <a name="axiom2"></a>$$\forall a,b \in F, (a + b) + c = a + (b + c)$$ (associativity)
  1. <a name="axiom3"></a>$$\forall a \in F, a + e = a$$ (Additive identity axiom)
  1. <a name="axiom4"></a>$$\forall a \in F, \exists b \in F \ni a + b = e$$ (existence of an Additive inverse)

  1. <a name="axiom5"></a>$$\forall a,b \in F, a \cdot b = b \cdot a$$ (commutativity)
  1. <a name="axiom6"></a>$$\forall a,b \in F, (a \cdot b) \cdot c = a \cdot (b \cdot c)$$ (associativity)
  1. <a name="axiom7"></a>$$\forall a \in F, a \cdot u = a$$ (Multiplicative identity axiom)
  1. $$\forall a \in F$$, $$\exists b \in F \ni a \cdot b = u$$ (existence of an Multiplicative inverse)

  1. <a name="axiom9"></a>$$\forall a,b,c \in F$$, $$a \cdot (b + c) = a \cdot b + a \cdot c$$ (distributivity)

Some common examples of fields include; $$\mathbb{N}$$, $$\mathbb{Q}$$, $$\mathbb{R}$$, and $$\mathbb{C}$$, where in
particular, $$\mathbb{N} \subseteq \mathbb{Q} \subseteq \mathbb{R} \subseteq \mathbb{C}$$.

In the context of $$\mathbb{R}$$, the Additive identity, $$e = 0$$, and the $$u = 1$$.

Just with this simple definition of a Field, we can jump right to proving some common algebraic expressions
we've seen before.

First of all, we want to verify that if $$a + b = a + c$$, then $$b = c$$.

_**Theorem 1**_. $$\forall a, b, c \in F$$, if $$a + b = a + c$$, then $$b = c$$.

_**Proof**_. By _[Axiom 4](#axiom4)_, $$\forall a \in F$$, $$\exists d \in F \ni a + d = e$$.
Thus, $$(a + b) + d = (a + c) + d$$ $$\Longrightarrow (a + d) + b = (a + d) + c$$ (by _[Axiom 1](#axiom1)_ and
_[Axiom 2](#axiom2)_). Hence, $$e + b = e + c$$ $$\Longrightarrow b = c$$ (by _[Axiom 3](#axiom3)_). $$\blacksquare$$

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

_**Theorem 3**_. <a name="theorem3"></a>$$\forall a \in F$$, $$\exists! b \in F \ni a + b = e$$

_**Proof**_. Suppose $$\forall a \in F$$, $$\exists b, b' \in F \ni a + b' = e$$.
Then, by previous Theorem, $$b = b'$$. $$\blacksquare$$

Notationally, $$\forall a \in F$$, we can denote their Additive and Multiplicative inverses by
$$-a$$ and $$a^{-1}$$ respectively.

We thus have $$a + (-a) = e$$ and $$a \cdot a^{-1} = u$$.

In $$\mathbb{R}$$, this would be $$a + (-a) = 0$$ and $$a \cdot a^{-1} = 1$$.

As with inverses, we present here a Theorem on the inverse of a Multiplicative inverse;
$$(a^{-1})^{-1}$$.

_**Theorem 4**_. <a name="theorem4"></a>$$\forall a \in F$$, if $$a \ne e$$ then $$(a^{-1})^{-1} = a$$.

_**Proof**_. We note that $$\forall a \in F$$, $$a^{-1} \cdot (a^{-1})^{-1} = e$$ and
$$a \cdot a^{-1} = e$$. Hence, $$a^{-1} \cdot (a^{-1})^{-1} = e$$ and $$a^{-1} \cdot a = e$$.
Thus, $$(a^{-1})^{-1} = a$$. $$\blacksquare$$

Next, we present a Theorem concerning 'division' of elements (or numbers if you will)
in a Field.

_**Theorem 5**_. <a name="theorem5"></a>$$\forall a, b \in F$$, where $$b \ne e$$,
$$\exists! x \in F \ni a \cdot x = b$$.

_**Proof**_. By _[Theorem 3](#theorem3)_, $$\forall a \in F$$, $$\exists! y \in F \ni a \cdot y = u$$.
Hence, let $$x = y \cdot b$$. Thus, $$a \cdot x = a \cdot (y \cdot b)$$ $$ = (a \cdot y) \cdot b = u \cdot b$$
$$ = b$$ (by _[Axiom 2](#axiom2)_ and _[Axiom 7](#axiom7)_). $$\blacksquare$$

Notationally, we could also denote the $$x$$ satisfying $$a \cdot x = b$$, by $$x = \dfrac{b}{a}$$.

Similarly, we could also denote $$a^{-1}$$, by $$\dfrac{1}{a}$$.

At this juncture, an alert reader might notice that in both _[Theorem 4](#theorem4)_ and _[Theorem 5](#theorem5)_, there are
restrictions on what you can 'divide' by and what can be 'divided'.

We shall tackle them one at a time.

Now, for _[Theorem 4](#theorem4)_, the restriction was on the fact that we couldn't 'divide' anything
by $$e$$ (or equivalently by $$0$$ in $$\mathbb{R}$$).

But is this restriction really necessary? Did the definition of the Field or any Theorems
cause this restriction?

Absolutely not, and we could actually thus remove it!

But suppose we removed it, then in the Proof (of _[Theorem 4](#theorem4)_),
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

Now, as for _[Theorem 5](#theorem5)_, we actually need to keep the restriction there.

For suppose the restriction was removed and $$a \cdot x = b $$ $$ = e$$ $$\Longrightarrow a \cdot x = e$$.
Then either $$a = e$$ or $$x = e$$. But since we're finding an $$x$$, then $$a = e$$.

However, before we prove the Theorem, we first need to prove the following Lemma.

_**Lemma 1**_. <a name="lemma1"></a>$$\forall a \in F$$, $$a \cdot e = e$$.

_**Proof**_. $$\forall a \in F$$, $$a \cdot e = a \cdot (e + e)$$ $$ = a \cdot e + a \cdot e$$
 (by _[Axiom 3](#axiom3)_ and _[Axiom 9](#axiom9)_). Then, $$a \cdot e + e = a \cdot e + a \cdot e$$
$$\Longrightarrow e = a \cdot e$$ (by _[Axiom 3](#axiom3)_). $$\blacksquare$$

_**Theorem 6**_. $$\forall a, b \in F$$, if $$a \cdot b = e$$, then either
$$a = e$$ or $$b = e$$.

_**Proof**_. Assume WLOG (Without Loss of Generality) that $$\forall a, b \in F$$, $$a \ne e$$.
(WTS (Want to Show): $$b = e$$.) Then, $$b = b \cdot u$$ $$= b \cdot (a \cdot a^{-1}) = (b \cdot a) \cdot a ^{-1}$$
$$ = (a \cdot b) \cdot a ^{-1} = e \cdot a$$ $$ = e$$ (by _[Axiom 7](#axiom7)_, _[Theorem
3](#theorem3)_, _[Axiom 5](#axiom5)_, _[Axiom 6](#axiom6)_, and _[Lemma 1](#lemma1)_). $$\blacksquare$$

Now, if that's the case, then by _[Lemma 1](#lemma1)_ again, we run into trouble because anything Multiplied with
$$e$$, would give us back $$e$$.

(Note: $$e$$ seems to be a very special element that has this property, $$u$$
doesn't even have such a property)


Hence we could simply take any $$x \in F$$ to get our desired $$b = e$$, and
the uniqueness as required in _[Theorem 5](#theorem5)_ thus breaks down!

Hence, in this case, we actually need the restriction of $$b \ne e$$ to be present.

With all these seemingly familiar algebraic expressions proved, a reader should be
able to deduce the rest of the common expressions from the abstract definition
of a Field.
