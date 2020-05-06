## Order Complete Fields & l.u.b axiom

In [Algebra](https://en.wikipedia.org/wiki/Algebra), a Field is a 5-tuple,
denoted by; $$\langle F, +, \cdot, e, u \rangle$$, where
  - $$F$$ is a [Set](https://en.wikipedia.org/wiki/Set_(mathematics)) consisting of all the elements
    in the Field
  - $$+$$ is the additive operator
  - $$\cdot\$$ is the multiplicative operator
  - $$e$$ is the additive identity
  - $$u$$ is the multiplicative identity

Some common examples of fields include; $$\mathbb{N}$$, $$\mathbb{R}$$, and $$\mathbb{C}$$, where in
particular, $$\mathbb{N} \subseteq \mathbb{R} \subseteq	\mathbb{C}$$.

Now, having defined the componenets of a Field, a Field has to follow some axioms.

With regards to the additive operator, the following axioms are defined:
  - $$\forall a,b \in F, a + b = b + a$$ (commutativity)
  - $$\forall a,b \in F, (a + b) + c = a + (b + c)$$ (associativity)
  - $$\forall a \in F, a + e = a$$ (this justifies the use of 'identity' on $$e$$)
  - $$\forall a \in F, \exists b \ni a + b = e$$ (existence of an additive inverse)

Similarly (and symmetrically), for the multiplicative operator, the following axioms hold:
  - $$\forall a,b \in F, a \cdot b = b \cdot a$$ (commutativity)
  - $$\forall a,b \in F, (a \cdot b) \cdot c = a \cdot (b \cdot c)$$ (associativity)
  - $$\forall a \in F, a \cdot e = a$$ (this justifies the use of 'identity' on $$e$$)
  - $$\forall a \in F, \exists b \ni a \cdot b = e$$ (existence of an additive inverse)

Finally, there is an axiom which involves (and associates) both the additive and multiplicative
operators together:
  - $$\forall a,b,c \in F, a \cdot (b + c) = a \cdot b + a \cdot c$$ (distributivity)
