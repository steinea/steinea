---
layout: entry
category: commonplace
author: Kevin Hartnett
title: A Short Guide to Hard Problems
publication: Quanta Magazine
link: https://www.quantamagazine.org/a-short-guide-to-hard-problems-20180716/
date: 2024-12-13
---

"Many different complexity classes exist, though in most cases researchers haven’t been able to prove one class is categorically distinct from the others. Proving those types of categorical distinctions is among the hardest and most important open problems in the field."

"In a paper published at the end of May, two computer scientists proved (with a caveat) that [the two complexity classes that represent quantum and classical computers really are different](https://www.quantamagazine.org/finally-a-problem-that-only-quantum-computers-will-ever-be-able-to-solve-20180621/)."

"P

**Stands for:** Polynomial time

**Short version:** All the problems that are easy for a classical (meaning nonquantum) computer to solve.

**Precise version:** Algorithms in P must stop and give the right answer in at most *nc* time where *n* is the length of the input and *c* is some constant."

"NP

**Stands for:** Nondeterministic Polynomial time

**Short version:** All problems that can be quickly verified by a classical computer once a solution is given.

**Precise version:** A problem is in NP if, given a “yes” answer, there is a short proof that establishes the answer is correct."

"PH

**Stands for:** Polynomial Hierarchy

**Short version:** PH is a generalization of NP — it contains all the problems you get if you start with a problem in NP and add additional layers of complexity.

**Precise version:** PH contains problems with some number of alternating “quantifiers” that make the problems more complex."

"This problem is equivalent to the P versus NP problem because if (unexpectedly) P = NP, then all of PH collapses to P (that is, P = PH)."

"PSPACE

**Stands for:** Polynomial Space

**Short version:** PSPACE contains all the problems that can be solved with a reasonable amount of memory.

**Precise version:** In PSPACE you don’t care about time, you care only about the amount of memory required to run an algorithm. Computer scientists have proven that PSPACE contains PH, which contains NP, which contains P."

"Is PSPACE different from P?"

"BQP

**Stands for:** Bounded-error Quantum Polynomial time

**Short version:** All problems that are easy for a quantum computer to solve.

**Precise version:** All problems that can be solved in polynomial time by a quantum computer."

"EXPTIME

**Stands for:** Exponential Time

**Short version:** All the problems that can be solved in an exponential amount of time by a classical computer.

**Precise version:** EXP contains all the previous classes — P, NP, PH, PSPACE and BQP. Researchers have proven that it’s different from P — they have found problems in EXP that are not in P."

"Computer scientists would like to be able to prove that PSPACE does not contain EXP. They believe there are problems that are in EXP that are not in PSPACE, because sometimes in EXP you need a lot of memory to solve the problems."

"BPP

**Stands for:** Bounded-error Probabilistic Polynomial time

**Short version:** Problems that can be quickly solved by algorithms that include an element of randomness.

**Precise version:** BPP is exactly the same as P, but with the difference that the algorithm is allowed to include steps where its decision-making is randomized. Algorithms in BPP are required only to give the right answer with a probability close to 1."
