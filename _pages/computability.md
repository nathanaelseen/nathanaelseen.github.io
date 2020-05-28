---
layout: page
title: The Halting Problem
description: A brief overview of the Halting Problem and its ramifications
---

In this section, I'll do a rather brief overview of the Halting Problem and its
ramifications.

---

As much as computers can help solve numerous real-world problems, there are
actually non-computable problems and the Halting Problem is a classic example.

According to the Halting Problem, we cannot write a (generalised) algorithm to
determine if a program P running on dataset D, will terminate or run
indefinitely.

In computer science, a decision problem involves a set of valid inputs, where there are only two
possible outputs; yes or no.

Some decision problems are ‘easier’ to solve in that, there exists a polynomial-time
algorithm, while there are others in the NP-hard category which require a very long
time (non-polynomial time) for computers to solve.

However, such decision problems are still theoretically decidable, as there exists an
algorithm which correctly satisfies
the problem.

On the contrary, there are also undecidable problems, which are totally non-computable,
and the Halting Problem is a classic example.

The Halting Problem is non-computable on all (Mathematical) models of computation,
even on the most powerful [Turing Machine (TM)](modelsofcomputation/#turingmachine).

As an interesting aside, the computers we use today are not exactly TMs, but a less
powerful variant: the [Finite State Machines (FSM)](modelsofcomputation/#finitestatemachine),
which unlike TMs, have a finite number of states.

In an FSM, the halting problem is theoretically decidable as a non-terminating program
must arrive at the same state twice (Peter, 2019).

However, solving the halting problem in this manner is impractical as a modern computer
with several gigabytes of memory would have at least $$2^{10^{6}}$$ possible
states (which is an extremely large number) (Peter, 2019).

In light of this, all computers could theoretically be modelled as
infinite state machines, and as TMs.

Since this is the case, we conclude that the Halting Problem is undecidable in
all cases.

Now, we also note that non-computability is not due to the limitations in the
design of those Mathematical models of comptuation, but rather, non-computability stems
from a [limitation in Mathematics](modelsofcomputation/#godelincompletenesstheorem).

Gödel’s first incompleteness theorem (Mathematics), states that a mathematical system
cannot prove its own consistency (although it might be able to proof its own
inconsistency).

Together with the use of self-referencing (which is deleterious in this case,
although self-referencing could actually be useful in other aspects of computer science
such as in recursive functions), a glaring Contradiction could be shown (mathematically)
for the halting problem.
    
Furthermore, in the
[Church-Turing thesis](https://en.wikipedia.org/wiki/Church%E2%80%93Turing_thesis),
Alan Turing has already dashed the hope that everything is computable.

Given the non-computability of certain problems, what are the possible ramifications?

For computer scientists, the Halting Problem poses an extra burden to write and
design correct software and algorithms which terminate after a finite number of steps.

Although compilers are able to flag out obvious semantical errors which could lead to
unreachable statements, bugs, and infinite loops, they are just but a weak attempt
in solving the halting problem.

Here's when a computer scientist need to manually performs algorithm analysis
to formally proof that an algorithm actually terminates. Hence, we note that
the burden is on the computer scientist to inspect and analyse the code (however
long and complicated it might be).

Also, we note that we cannot employ the assistance of a computer, as the
Halting Problem tells us so!

The halting problem, and other non-computable problems reducible to the
Halting Problem impedes the advancement of computer science.

For example, in research, the Halting Problem could either lengthen the
duration of a research (due to manual work/verification which cannot be automated),
or perhaps render the whole researched problem non-computable too.

_References_

Peter. (2019, February 13). Re: Decidability of the halting problem on finite computers
[Online discussion post]. Retrieved from:
<https://cstheory.stackexchange.com/questions/9907/decidability-of-the-halting-problem-on-finite-computers>
