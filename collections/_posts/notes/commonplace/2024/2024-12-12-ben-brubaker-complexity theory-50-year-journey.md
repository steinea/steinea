---
layout: entry
category: commonplace
author: Ben Brubaker
title: Complexity Theory’s 50-Year Journey
publication: Quanta Magazine
link: https://www.quantamagazine.org/complexity-theorys-50-year-journey-to-the-limits-of-knowledge-20230817/
date: 2024-12-12
---

"the professor posed a simple question that would change the course of his life: How do you know math actually works?"

"“That made me sit up and pay attention,” recalled [Carmosino](https://marco.ntime.org/), now a theoretical computer scientist at IBM."

"the central open question in theoretical computer science, known as the P versus NP problem."

"At stake is nothing less than the nature of what’s knowable."

"Despite decades of effort by researchers in the field of computational complexity theory — the study of such questions about the intrinsic difficulty of different problems — a resolution to the P versus NP question has remained elusive. And it’s not even clear where a would-be proof should start."

"“There’s no road map,” said [Michael Sipser](https://math.mit.edu/~sipser/), a veteran complexity theorist at the Massachusetts Institute of Technology who spent years grappling with the problem in the 1980s. “It’s like you’re going into the wilderness.”"

"Carmosino and other researchers in the subfield of meta-complexity reformulate questions like this as computational problems, propelling the field forward by turning the lens of complexity theory back on itself."

"researchers have learned that the hardness of proving computational hardness is intimately tied to fundamental questions that may at first seem unrelated. How hard is it to spot hidden patterns in apparently random data? And if truly hard problems do exist, how often are they hard?"

"The P versus NP problem owes its lackluster name to complexity theorists’ habit of sorting computational problems into broad “[complexity classes](https://www.quantamagazine.org/a-short-guide-to-hard-problems-20180716/)”"

"The challenge for complexity theorists is to turn these hints into rigorous theorems about the relationships between complexity classes."

"David Hilbert proposed a research program for grounding mathematics in absolute certainty. He hoped to start from a few simple assumptions, called axioms, and derive a unified mathematical theory that met three key criteria."

"Hilbert’s first condition, consistency, was the essential requirement that mathematics be free of contradictions: If two contradictory statements could be proved starting from the same axioms, the whole theory would be unsalvageable."

"Hilbert’s second condition, completeness: the requirement that all mathematical statements be either provably true or provably false."

"His third criterion, decidability, demanded an unambiguous mechanical procedure for determining whether any mathematical statement was true or false."

"Addressing a conference in 1930, Hilbert declared: “Our slogan shall be ‘We must know, we will know.’”"

"Just a year later, Gödel delivered the first blow to Hilbert’s dream."

"He [proved](https://www.quantamagazine.org/how-godels-incompleteness-theorems-work-20200714/) that a self-defeating statement like “this statement is unprovable” could be derived from any appropriate set of axioms."

"Gödel also proved that no mathematical theory could ever prove its own consistency."

"Then in 1936, a 23-year-old graduate student named Alan Turing rephrased Hilbert’s decidability condition in the then-unfamiliar language of computation and dealt it a fatal blow."

"Turing formulated a mathematical model — now known as the [Turing machine](https://www.quantamagazine.org/alan-turings-most-important-machine-was-never-built-20230503/) — that could represent all possible algorithms, and showed that if Hilbert’s procedure existed, it would fit within this model. He then used self-referential methods like Gödel’s to [prove](https://londmathsoc.onlinelibrary.wiley.com/doi/abs/10.1112/plms/s2-42.1.230) the existence of undecidable statements — or, equivalently, uncomputable problems that no algorithm could solve."

"What if the question wasn’t just whether problems are solvable, but how hard they are to solve?"

"At first, complexity classes seemed like convenient categories for sorting problems that were similar but not directly related — nobody suspected that finding Hamiltonian paths had anything to do with other hard computational problems."

"Then in 1971, within a year of relocating to the University of Toronto after being denied tenure in the United States, the complexity theorist [Stephen Cook](http://www.cs.toronto.edu/~sacook/) published an [extraordinary result](https://dl.acm.org/doi/10.1145/800157.805047). He identified a particular NP problem with a strange feature: If there’s a polynomial algorithm that can solve that problem, it can also solve every other problem in NP. Cook’s “universal” problem, it seemed, was a lone column propping up the class of apparently hard problems, separating them from the easy problems below. Crack that one problem, and the rest of NP will come crashing down."

"Around the same time, a graduate student in the Soviet Union named [Leonid Levin](https://www.cs.bu.edu/fac/lnd/) proved a [similar result](https://www.mathnet.ru/php/archive.phtml?wshow=paper&jrnid=ppi&paperid=914&option_lang=eng), except that he identified several different universal problems."

"In addition, the American complexity theorist [Richard Karp](https://www2.eecs.berkeley.edu/Faculty/Homepages/karp.html) [proved](https://link.springer.com/chapter/10.1007/978-1-4684-2001-2_9) that the universality property identified by Cook (and Levin, though Karp and Cook didn’t know of Levin’s work until years later) was itself all but universal."

"Nearly every NP problem without a known polynomial algorithm — that is, nearly every easily checkable problem that seemed hard — had the same property, which became known as NP-completeness."

"This means all NP-complete problems — the Hamiltonian path problem, sudoku, and [thousands](https://www.quantamagazine.org/edit-distance-reveals-hard-computational-problems-20150929/) [of others](https://www.quantamagazine.org/computer-scientists-break-traveling-salesperson-record-20201008/) — are in a precise sense equivalent. “You have all these different natural tasks, and they all magically turn out to be the same task,” Ilango said. “And we still don’t know whether that same task is possible or not.”"

"Carmosino’s main goal, at first, was to better understand a [landmark paper](https://dl.acm.org/doi/10.1145/195058.195134) from two decades earlier that had captured his imagination. That paper, by the complexity theorists [Alexander Razborov](https://people.cs.uchicago.edu/~razborov/) and [Steven Rudich](https://csd.cmu.edu/people/faculty/steven-rudich), had shown that a certain “natural” strategy for proving P ≠ NP would almost certainly fail, because success would come at a steep cost — the complete breakdown of cryptography — that researchers regarded as very unlikely."

"he and three colleagues proved a surprising result by examining the natural proofs barrier from the perspective of meta-complexity."

"At first, researchers tried to prove P ≠ NP — that is, prove that some NP problems aren’t solvable by any possible polynomial algorithm — using variations on the techniques Turing had used to prove that some problems aren’t solvable by any algorithm whatsoever."

"they began to look for another approach, and they soon found one in the work of Turing’s contemporary [Claude Shannon](https://www.quantamagazine.org/how-claude-shannons-information-theory-invented-the-future-20201222/)."

"Shannon’s work suggested a new way for theorists to think about the difficulty of computational problems, called “circuit complexity,” even though the circuits in question are just mathematical abstractions."

"instead of computational problems and the algorithms that solve them, researchers consider Boolean functions and the circuits that compute them."

"like an algorithm, a circuit describes a procedure for producing an output given any input."

"Does the minimum number of gates needed to compute a Boolean function grow polynomially or exponentially as the number of input variables increases? Researchers call these two categories of functions “easy to compute” and “hard to compute,” respectively."

"attempts to prove P ≠ NP had a self-defeating character reminiscent of Gödel’s famous proposition “this statement is unprovable”"

"The tension at the heart of the natural proofs barrier is that the task of distinguishing high-complexity functions from low-complexity ones is similar to the task of distinguishing true randomness from the pseudorandomness used to encrypt messages. We’d like to show that high-complexity functions are categorically different from low-complexity functions, to prove P ≠ NP. But we’d also like for pseudorandomness to be indistinguishable from randomness, to be confident in the security of cryptography. Maybe we can’t have it both ways."

"A natural proof of P ≠ NP would require a very comprehensive understanding of how easy-to-compute and hard-to-compute functions differ, and that knowledge could also fuel a fast algorithm for spotting easy-to-compute functions even if they’re superficially complicated."

"“If you believe in hardness, then you should believe that it’s hard to prove hardness,” Kabanets said."

"The difficulty of understanding circuit complexity acts like a barrier to any known strategy for proving the NP-completeness of MCSP — a problem that’s itself about the difficulty of understanding circuit complexity. The twisted, self-defeating logic of the natural proofs barrier seemed inescapable."

"Meta-complexity research slowed to a trickle. It would flourish again 16 years later, when researchers discovered a surprising connection to another fundamental question: How hard is it to solve problems if you only care about getting the right answer most of the time?"

"For everyday problems, answers that work most of the time are often good enough. We plan our commutes for typical traffic patterns, for instance, not for worst-case scenarios."

"Most complexity theorists are harder to satisfy: They’re only content to declare a problem easy if they can find a fast algorithm that gets the right answer on every possible input."

"The distinction matters to cryptographers."

"Impagliazzo coined whimsical names for [five worlds](https://www.quantamagazine.org/which-computational-universe-do-we-live-in-20220418/) distinguished by different degrees of computational hardness and different cryptographic capabilities. We live in one of these worlds, but we don’t know which."

"In a [2016 paper](https://dl.acm.org/doi/10.5555/2982445.2982455), the four researchers proved that a certain kind of average-case MCSP algorithm could be used to construct a worst-case algorithm for identifying patterns hidden in random-looking strings of digits — a task that computer scientists refer to as “learning.”"

"Those four researchers had found a connection between the average-case complexity of one problem — MCSP — and the worst-case complexity of another — Boolean learning."

"Hirahara developed their techniques further to [derive](https://ieeexplore.ieee.org/document/8555110) a worst-case to average-case reduction for MCSP."

"His result implies that a hypothetical average-case MCSP algorithm like the one Carmosino and his colleagues had considered would actually be powerful enough to solve a slightly different version of MCSP without making any mistakes."

"Impediments remain to proving NP-completeness for the full version of MCSP. But none are the sort of barriers that suggest an entirely new toolkit is needed — it may just be a matter of finding the right way to combine known techniques."
