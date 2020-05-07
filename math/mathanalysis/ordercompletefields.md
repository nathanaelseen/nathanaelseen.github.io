---
title: Order Complete Fields
description: Covers what an algebraic Field is and what it means for a Field to be order complete
---

## Order Complete Fields

In [Algebra](https://en.wikipedia.org/wiki/Algebra), a Field is a [Set](https://en.wikipedia.org/wiki/Set), by which two important
operations, namely; **Addition** and **Multiplication**, over the elements (in the Set) are defined.

_**Definition**_:
A Field is a 5-tuple, denoted by; $$\langle F, +, \cdot, e, u \rangle$$, where
  - $$F$$ is a [Set](https://en.wikipedia.org/wiki/Set_(mathematics)) consisting of all the elements
    in the Field
  - $$+$$ is the Additive operator
  - $$\cdot\$$ is the Multiplicative operator
  - $$e$$ is the Additive identity
  - $$u$$ is the Multiplicative identity,

with the following axioms defined:
  1. $$\forall a,b \in F, a + b = b + a$$ (commutativity)
  1. $$\forall a,b \in F, (a + b) + c = a + (b + c)$$ (associativity)
  1. $$\forall a \in F, a + e = a$$ (Additive identity axiom)
  1. $$\forall a \in F, \exists b \ni a + b = e$$ (existence of an Additive inverse)

  1. $$\forall a,b \in F, a \cdot b = b \cdot a$$ (commutativity)
  1. $$\forall a,b \in F, (a \cdot b) \cdot c = a \cdot (b \cdot c)$$ (associativity)
  1. $$\forall a \in F, a \cdot u = a$$ (Multiplicative identity axiom)
  1. $$\forall a \in F, \exists b \ni a \cdot b = u$$ (existence of an Multiplicative inverse)

  1. $$\forall a,b,c \in F, a \cdot (b + c) = a \cdot b + a \cdot c$$ (distributivity)

Some common examples of fields include; $$\mathbb{N}$$, $$\mathbb{Q}$$, $$\mathbb{R}$$, and $$\mathbb{C}$$, where in
particular, $$\mathbb{N} \subseteq \mathbb{Q} \subseteq \mathbb{R} \subseteq \mathbb{C}$$.

The Additive and Multiplicative identity $$e$$ and $$u$$, are merely 'special' elements in the Set
$$F$$, where when you 'add'/'multiply' any element; $$x \in F$$, you will get back the same x.

Also, we note that in $$\mathbb{R}$$, the Additive identity, $$e$$ is the _symbol_ $$0$$, and the
Multiplicative identity $$u$$ is the _symbol_ $$1$$.

Just with the simple definition of a Field (as given above), we can jump right to proving some
common algebraic expressions we've seen before.

First of all, we want to verify that if $$a + b = a + c$$, then $$b = c$$.

_**Theorem**_: $$\forall a, b, c \in F$$, if $$a + b = a + c$$, then $$b = c$$.

_**Proof**_: By the existence of Additive inverse axiom, $$\exists d \in F$$ where $$a + d = e$$. Thus,
$$(a + b) + d = (a + c) + d$$ $$=> (a + d) + b = (a + d) + c$$ (by the commutativity and associativity
axiom). Hence, $$e + b = e + c$$ $$=> b = c$$ (by the Additive identity axiom). $$\blacksquare$$

Next, we would like to verify that both the Additive and Multiplicative identity are unique, i.e,
there is only one such identity (in the whole Field).

In $$\mathbb{R}$$, this means that $$0$$, the Additive identity is unique, and there is no other
such number; $$0'$$, which has the same property as $$0$$, where when you add a number $$x$$
with it, you will get back the same number $$x$$.

We will only prove the uniqueness of the Additive identity, and the proof of the Multiplicative
identity should be similar.

_Theorem_:
$$\exists! e \in F$$, where $$\forall a \in F$$, $$a + e = a$$.

_Proof_: Suppose that $$\exists e, e' \in F$$, where $$\forall a \in F$$, $$a + e = a$$ and
$$a + e' = a$$. Then, by previous Theorem, $$e = e'$$.
