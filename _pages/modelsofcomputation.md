---
layout: page
title: Models of Computation
description: Provides a really brief overview over the various mathematical models of Computation
---

In this article, we will provide a really brief overview about the various mathematical
models of Computation, used in the study of Computability.

---

As we know, there are problems in Computer Science which are non-computable despite being given
an given infinite amount of (computing) resources.

In the Theory of Computability (ToC), various Mathematical models are used by
Computer Scientists to study Computability.

Notionally, these Mathematical models of Computation could be perceived as abstract
forms of Computers.

Some examples include (from the least to most powerful):
 - Combinational Logic (includes basic digital circuitry, designed using Boolean Algebra)
 - Push-down Automata
 - <a name="finitestatemachine"></a> Finite State Machines (FSM):
   - (Examples include PCs, Laptops, Mobile Phones. These devices have (finite) RAM slots,
      hence States, and when all slots are used, the Computer would need to free up some
      slots and therefore reuse those slots, or States. Hence the term Finite State
      Machines.)
 - Context-Free Grammer/Languages
 - <a name="turingmachine"></a> Turing Machine (most powerful model, invented
   by [Alan Turing](https://en.wikipedia.org/wiki/Alan_Turing) himself)

Despite these powerful and potentially ‘infinite’ ‘computers’, the Halting Problem
(more details discussed in another article), is an example of a non-computable problem.

You might be wondering then; is this non-computability due to the (limited) design?

<a name="godelincompletenesstheorem"></a> Actually nope, it stems from a limitation
in Mathematics (Godel’s Incompleteness Theorem).

This Theorem states that a formal Mathematical system cannot prove it’s own consistency.

It is not hard to see that given a Mathematical system with a bunch of axioms, one might
not be able to prove those axioms (irreducible assertions).

While we note that a formal system cannot prove its own consistency, it might however
be able to prove its own inconsistency.

Perhaps you are taken aback that Mathematics which seem like such a powerful tool used in many
disciplines, also has its own limitations.

However, it is precisely this limitation which caused a limitation in the
Computability of the Halting Problem.

The Halting Problem is a classic non-computable problem, and to prove a problem is
non-computable, one only needs to show it is
[reducible](https://en.wikipedia.org/wiki/Reduction_(complexity)) to the Halting Problem.

