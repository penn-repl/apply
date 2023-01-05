---
layout: page
title:
permalink: /plclub+/
---

<img align="center" width="100%" src="/images/plclub+.png">

## PLClub+
PLClub+ is an undergraduate supplement to PLClub, the weekly meeting of Penn's programming language research group. REPL students will participate in PLClub+ in addition to their research with PLClub. It consists of 4 activities:
- **Software Foundations Mini-Course.** Condensed version of [CIS 5000](https://www.seas.upenn.edu/~cis5000/current/index.html), covers essential prerequisites for programming languages research. Taught by a PLClub PhD student twice a week.
- **Reading Club.** Covers classic papers in programming languages. Led by a PLClub PhD student once a week.
- **Seminar.** An undergraduate friendly seminar series, covering a variety of research happening in and outside of PLClub. Happens once a week.
- **PhD Application Workshop.** A two-week workshop at the end of REPL. Covers the fundamentals of preparing a strong PhD application.

See below for more details about each activity in PLClub+.

---

## Software Foundations Mini-Course

[Software Foundations](https://softwarefoundations.cis.upenn.edu) is a book series which began in PLClub and is now used internationally as an introduction to formal proofs about the properties of programs and programming languages. This mini-course covers a condensed version of the material from [CIS 5000](https://www.seas.upenn.edu/~cis5000/current/index.html), Penn's graduate programming languages course. Below we outline the curriculum, with brief synopses of topics we cover.

#### <a href="https://softwarefoundations.cis.upenn.edu/lf-current/index.html">Volume 1: Logical Foundations</a>

- **Week 1: Functional Programming in Coq, Proof by Induction.** Coq lets you write programs and prove them correct in the same language. These lessons introduce students to simple programs and simple proofs of their correctness.

- **Week 2: Working with Structured Data, Polymorphism and Higher-Order Functions.** Building on the introduction to functional programming, these sections introduce new programming constructs. These let us write more interesting programs and more interesting proofs e.g. list processing programs.

- **Week 3: More Basic Tactics, Logic in Coq.** Introduces more proof techniques, called tactics, to help you write proofs in Coq. Exercises these proof skills by proving logical propositions involving conjunction, disjunction, negation, and more.

- **Week 4: Inductively Defined Propositions, Total and Partial Maps.** To write more interesting propositions, we often use inductively defined propositions. For example, whether a natural number is even can be defined as an inductive proposition. These sections demonstrate how to construct and prove correct propositions involving inductively defined propositions and total/partial maps.

- **Week 5: The Curry-Howard Correspondence, Induction Principles.** These sections zoom out. Both illuminate details that were somewhat implicit up to this point. The Curry-Howard correspondence relates programming and proving in a deep way. Induction principles let us prove things about inductive data like lists and trees.

- **Week 6: Properties of Relations, Simple Imperative Programs.** Constructing and proving properties of relations. Applying all the techniques up to this point to construct and reason about simple imperative programs.

#### <a href="https://softwarefoundations.cis.upenn.edu/plf-current/index.html">Volume 2: Programming Language Foundations</a>

- **Week 7: Program Equivalence, Hoare Logic I.** Shows how to demonstrate the equivalence of two programs using variable assignment and loops. Moreover, introduces Hoare Logic: a tool for proving the correctness of such programs.

- **Week 8: Hoare Logic II, Small-Step Operational Semantics.** A continuation of asserting program behavior through Hoare Logic. Introduction to operational semantics, a way of giving meaning to a program by defining how it "steps" from the initial program to the final result.

- **Week 9: Type Systems, The Simply Typed-Lambda Calculus (STLC).** Introduction to type theory and the model organism of programming languages, the simply-typed lambda calculus. A useful precursor to more advanced types, more advanced languages.

- **Week 10: Properties of STLC, A Typechecker for STLC.** Considering which properties hold of the STLC and proving them. Additionally, how to build a correct typechecker for the language. Both lessons generalize to languages with more advanced types and features.


## Reading Club

Programming languages a rich history of deep intellectual contributions to computer science. Reading club helps REPL students digest these insights, each week discussing papers like those below. A PLClub PhD student leads discussions, both helping students interpret and develop reading strategies for making sense of papers.

- **The next 700 programming languages (Peter Landin, 1969).** This paper pioneers the move to consider powerful “core” languages in designing programming languages. Instead of everyone inventing their own language, they ought to first ask if it can be encoded in an existing “core” language. Landin proposes his own core language, ISWIM, based on the lambda calculus. Today, most functional programming languages build off an expressive lambda calculus “core” as suggested by Landin.

- **An axiomatic basis for computer programming (Peter Landin, 1969).** Introduces Hoare logic: a means to assert that computations behave in specific ways. You assert preconditions (what must be true before running the computation) and postconditions (what must be true after running the computation). Then the logic gives you rules for determining if the postcondition follows from both the precondition and “evidence” provided by the computation. Today, a cottage industry of Hoare-style logics exist and continue to develop for increasingly diverse programming languages.

- **Towards a theory of type structure (John Reynolds, 1974).** Introduces polymorphism into programming languages, greatly expanding the space of functions that typed programming languages could write. Precedes his work on parametricity, formalizing what it means to have polymorphism in a language. Today, all popular typed functional programming languages include polymorphism.

- **On the expressive power of programming languages (Matthias Felleisen, 1991).** What is meant when someone claims one language is more expressive than another? Surely it can’t just be about whether it’s Turing-complete or not. Because we often claim differences in expressiveness across Turing-complete languages. This paper clarifies the intuitive sense in which we claim the expressive power of a programming language. Today, we continue to use this approach to compare languages which add/remove different features.

- **More on advice on structuring compilers and proving them correct (Thatcher et al., 1981).** A follow-up, refinement to a paper proposing a unified view of compiler correctness. Namely, that correct compilers must preserve or refine the meaning of the original program. Frames the problem algebraically. Today, most compiler correctness theorems still take this form.


## Seminar

To complement the PhD-oriented PLClub seminar, we organize an undergraduate-oriented PLClub+ seminar. Only REPL students will be allowed to attend and a generous amount of discussion time available for discussion and questions. Below are example topics that REPL students can expect to see at seminar.

- **Seeing the world through Lenses (Li-Yao Xia).** Lenses are the prototypical bidirectional transformations, programs which may be run in one direction to view data as a fragment (e.g., a row) of some source (e.g., a database), and in another direction to synchronize the source after updating the visible fragment. Perhaps because of their simplicity, lenses arise in domains seemingly unrelated to bidirectional programming. Records in programming languages, subtyping, interactive systems, machine learning, laziness... Is it merely a coincidence? Or could lenses be a fundamental particle of PL? Discovering lenses in the wild may forever change how you see the world.

- **Reflecting on Random Generation (Harrison Goldstein).** Frameworks like QuickCheck provide domain specific languages (DSLs) for writing generators, programs that randomly generate program inputs that are useful for testing. Generators provide lots of utility for testers, enabling thorough testing of functions with hard-to-satisfy preconditions, but it turns out that there is even more potential utility hiding in plain sight. In this talk, I'll present reflective generators, a modified DSL for random generation that builds on ideas from bidirectional programming to improve workflows throughout the testing process. Reflective generators can do more than just sample input values: they can validate their own correctness, adapt their distributions based on user-specified examples, and even mutate test inputs while maintaining invariants. These new capabilities come at a relatively low cost and unlock state-of-the-art testing strategies that normally require entirely separate testing infrastructure.

- **One Quantum Algorithm, Inexpertly Explained (Lucas Silver).** This Friday, I will be presenting One Quantum Algorithm, Inexpertly Explained. As quantum computers continue to become bigger and more reliable, quantum computing promises to become very impactful on the field of computer science. In this talk, I hope to be able to bring someone from 0 quantum computing knowledge to understanding Simon's Algorithm, the first algorithm known to be exponentially faster than any known classical or probabilistic algorithm. It will be an informal chalkboard talk. Fair warning, my knowledge of quantum computing is new and still very limited. Still, I hope that this talk can still be very informative, as most of us have very limited knowledge about quantum mechanics.

- **Modal Logic & Type Theory (Lef Ioannidis).** Modal logics are contextual logics -- they allow us to qualify intuitionistic formulas as holding in a certain way, e.g. ‘necessarily’, ‘in the future’, ‘everywhere’, ‘probably’, ‘as everyone knows’, or ‘normally’. As pure functional programs need monads to interact with their environment, intuitionistic logic  needs modalities to prove things with respect to the environment. This Friday I will introduce Modal logics and Modal Type Theory in the way of Pfenning and Reed. Moreover, I will introduce some common modal logics (S4, LTL, Epistemic, Location, Lax, Authentication logic), in addition to models for structural modal logics (Kripke models, Bool-algebras with operators, coalgebras).

## PhD Application Workshop

On weeks 9 and 10 students will attend a workshop led by Joey on how to prepare competitive PhD applications. The workshop will hone in on the following topics.

- **Personal Statements.** How important are personal statements in an application? How personal should they be? What to include and not to include? How to format and outline them?

- **Letters of Recommendation.** How important are letters of recommendation in an application? What’s a good letter of recommendation? How can I strengthen my letters of recommendation? How to select letter writers? How to help your letter writers?

- **A Good Fit.** When is a program a good fit? How to find programs that are good fits? When is an adviser a good fit? How to find advisers that are good fits?


