---
layout: page
title: Computability
description: A brief overview of this big Computer Science topic on Computability
---

In this section, I'll do a really high-level overview of Computability, what it means,
and also some problems in Computer Science which are non-Computable. Additionally, we
shall also explore possible (philosophical) ramifications of non-computability.

---

As much as computers can help solve numerous real-world problems, there are actually non-computable problems
and the halting problem is a classic example: we can't write a generalised algorithm to determine if a
program P running on dataset D, will terminate or run indefinitely.

We shall discuss the halting problem in greater details and explore the possible ramifications
of non-computability in general.

In computer science, a decision problem involves a set of valid inputs, where there are only two
possible outputs; yes or no.

Some decision problems are ‘easier’ to solve in that, there exists a polynomial-time algorithm, while
there are others in the NP-hard category which require a very long time (non-polynomial time) for
computers to solve.

However, such decision problems are still decidable, as there exists an algorithm which correctly satisfies
the problem.

On the contrary, there are also undecidable problems,
which are totally non-computable, and the halting problem is a classic example.

The halting problem is non-computable on all (Mathematical) models of computation, even on the most
powerful Turing Machine (TM).

As an interesting aside, the computers we use today are not exactly TMs, but a less powerful variant:
the Finite State Machines (FSM), which unlike TMs, have a finite number of states.

In an FSM, the halting problem is theoretically decidable as a non-terminating program must arrive at the
same state twice (Peter, 2019). However, solving the halting problem in this manner is impractical as a modern computer
with several gigabytes of memory would have at least $$2^{10^{6}}$$ possible states (which is an extremely large number)
(Peter, 2019).

In light of this, all computers could theoretically be modelled as infinite state machines,
and as TMs.

Since this is the case, we conclude that the halting problem is undecidable in all cases.

Now, we also note that non-computability is not due to the limitations in the design of those
Mathematical models of comptuation, but rather, non-computability stems from a limitation in Mathematics.

Gödel’s first incompleteness theorem (Mathematics), states that a mathematical system cannot prove
its own consistency (although it might be able to proof its own
inconsistency).

Together with the use of self-referencing (which is deleterious in this case,
although self-referencing could actually be useful in other aspects of computer science
such as in recursive functions), a glaring Contradiction could be shown (mathematically)
for the halting problem.
    
Furthermore, in the Church-Turing thesis, Alan Turing has already dashed the hope
that everything is computable.

Given the non-computability of certain problems, what are the possible ramifications?

For computer scientists, the halting problem poses an extra burden to write and design correct software
and algorithms which terminate after a finite number of steps.

Although compilers are able to flag out obvious semantical errors which could lead to unreachable statements,
bugs, and infinite loops, they are just but a weak attempt in solving the halting problem.

Here's when a computer scientist need to manually performs algorithm analysis to formally proof that
an algorithm actually terminates. Hence, we note that the burden is on the computer scientist to inspect and
analyse the code (however long and complicated it might be).

Also, we note that we cannot employ the assistance of a computer, as the halting problem tells us
so!

The halting problem, and other non-computable problems reducible to the halting problem impedes the
advancement of computer science.

For example, in research, the halting problem could either lengthen the duration of a research
(due to manual work/verification which cannot be automated), or perhaps render the whole
researched problem non-computable too.

Beyond computer science, non-computable problems highlight the limitations of computers, and more generally,
the TMs. Philosophically, would this lead to the conclusion that human minds are more powerful than machines?
Or could it be that alike non-computable problems, there are limitations of the human mind too? Actually,
what defines limitations, and do definitions have limitations?


_References_

Peter. (2019, February 13). Re: Decidability of the halting problem on finite computers [Online discussion post]. Retrieved from: https://cstheory.stackexchange.com/questions/9907/decidability-of-the-halting-problem-on-finite-computers

