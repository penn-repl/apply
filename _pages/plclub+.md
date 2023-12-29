---
layout: page
title:
permalink: /plclub+/
---

<img align="center" width="100%" src="/images/plclub+.png">

## PLClub+
In addition to their research, REPL students will participate in PLClub+, an undergraduate-level supplement to the usual weekly PLClub seminar. PLClub+ consists of 5 activities:
- **Software Foundations Bootcamp.** Based on [CIS 5000](https://www.seas.upenn.edu/~cis5000/current/index.html), covers the basics of using the Coq proof assistant. Taught every day for the first week of the program.
- **Types and Programming Languages.**  An introduction to type theory and programming languages. Taught once a week beginning the second week.
- **Reading Club.** Covers classic papers in programming languages. Discussions moderated by a PLClub PhD student, once a week.
- **Seminar.** An undergraduate friendly seminar series, covering a variety of research happening in and outside of PLClub. Happens once a week.
- **PhD Application Workshop.** A two-week workshop at the end of REPL. Covers the fundamentals of preparing a strong PhD application.

See below for more details about each activity in PLClub+.

---

## Software Foundations Bootcamp

[Software Foundations](https://softwarefoundations.cis.upenn.edu) is a series of
books which began in PLClub, and are now used internationally as a standard
introduction to formal proofs about the properties of programs and programming
languages.  This bootcamp condenses material in Penn's graduate programming
languages course, [CIS 5000](https://www.seas.upenn.edu/~cis5000/current/index.html),
which uses Software Foundations as its textbook. Below are a sample of covered topics.

- **Functional Programming in Coq, Proof by Induction.** Coq lets you write programs and prove them correct in the same language. These lessons introduce students to writing functional programs and building proofs of their correctness.

- **Working with Structured Data, Polymorphism and Higher-Order Functions.** Building on the introduction to functional programming, these sections introduce new programming constructs, which let us write more interesting programs and more interesting proofs.

- **More Basic Tactics, Logic in Coq.** Introduces more proof techniques, called tactics, to help you write proofs in Coq. Exercises these proof skills by proving logical propositions involving conjunction, disjunction, negation, and more.

- **Inductively Defined Propositions, Total and Partial Maps.** These sections demonstrate how to construct and prove theorems involving inductively defined propositions, which are a much broader class of propositions than the ones to this point.
As a case study using the tools learned so far, this section also investigates the theory of total/partial maps.

- **The Curry-Howard Correspondence, Induction Principles.** These sections zoom out and illuminate details that were somewhat
implicit up to this point. The Curry-Howard correspondence relates programming and proving in a deep way, while induction principles let us
prove things about inductive data like lists and trees.

## Types and Programming Languages

A weekly lecture introduces students to type theory and programming languages, based on material from Benjamin Pierce's [Types and Programming Languages](https://www.cis.upenn.edu/~bcpierce/tapl/). Students will learn about various lambda calculi and how to prove properties about them. Below are a sample of covered topics.

- **Untyped lambda calculus.** The untyped lambda calculus is a "simple" programming language. It's a programming language with only a handful of moving parts. Despite this simplicity it's incredibly expressive, it's a Turing-complete programming language. In this section we explore how to formally define a lambda calculus, and how to represent various programs.

- **Simply typed lambda calculus.** The simply typed lambda calculus introduces types to the lambda calculus. With simple types, we've made a dramatic shift from the untyped lambda calculus. We lose some expressive power but we can now statically determine properties of programs, without running them. In this section we explore how to define a type system and how to prove that it's "correct."

- **Polymorphically typed lambda calculus.** The polymorphic lambda calculus introduces stronger types to the lambda calculus. This helps it recover some of the expressive power lost by simple types while also showcasing how types can statically enforce strong properties of programs like parametricity. In this section we explore how to introduce polymorphism into a lambda calculus and how to prove that it's "correct."

- **Strong normalization.** So far the course has defined correctness of a type system in terms of type safety: well typed programs can always take a step of computation. We now introduce a stronger notion of correctness called strong normalization: well typed programs always terminate. In this section we explore how to prove strong normalization with logical relations.

## Reading Club

Programming language theory has a rich history of deep intellectual contributions to
computer science. Each week, REPL students will digest these insights by reading
and discussing papers like the ones below.  A PLClub PhD student will lead
discussions, helping students to both understand the text, and to develop
reading strategies for making sense of future papers.

- **The next 700 programming languages (Peter Landin, 1966).** This paper pioneers the move to consider powerful “core” languages in designing programming languages. Instead of everyone inventing their own language, they ought to first ask if it can be encoded in an existing “core” language. Landin proposes his own core language, ISWIM, based on the lambda calculus. Today, most functional programming languages build off an expressive lambda calculus “core” as suggested by Landin.

- **An axiomatic basis for computer programming (Tony Hoare, 1969).** Introduces Hoare logic: a means to assert that computations behave in specific ways. You assert preconditions (what must be true before running the computation) and postconditions (what must be true after running the computation). Then the logic gives you rules for determining if the postcondition follows from both the precondition and “evidence” provided by the computation. Today, a cottage industry of Hoare-style logics exists, and researchers continue to develop them for increasingly diverse and complex languages.

- **Towards a theory of type structure (John Reynolds, 1974).** Introduces polymorphism into programming languages, greatly expanding the space of functions that typed programming languages could write. Precedes Reynolds' work on parametricity, which characterizes the expressivness of polymorphic functions. Today, all popular typed functional programming languages include polymorphism.

- **On the expressive power of programming languages (Matthias Felleisen, 1991).** What is meant when someone claims one language is more expressive than another? This paper formalizes the intuitive sense in which we claim the expressive power of a programming language. Today, we continue to use this approach to compare languages which add/remove different features.

- **More on advice on structuring compilers and proving them correct (Thatcher et al., 1981).** A follow-up, refinement to a paper proposing a unified view of compiler correctness. Namely, that correct compilers must preserve or refine the meaning of the original program. Frames the problem algebraically. Today, most compiler correctness theorems still take this form.


## Seminar

To complement the PhD-student-oriented PLClub seminar, REPL students will also attend an undergraduate-oriented PLClub+ seminar. *Only* REPL students will be allowed to attend, and a generous amount of discussion time available for discussion and questions. Below are example topics that REPL students can expect to see at the PLClub+ seminar.

- **Seeing the world through Lenses (Li-Yao Xia).** Lenses are the prototypical bidirectional transformations, programs which may be run in one direction to view data as a fragment (e.g., a row) of some source (e.g., a database), and in another direction to synchronize the source after updating the visible fragment. Perhaps because of their simplicity, lenses arise in domains seemingly unrelated to bidirectional programming. Records in programming languages, subtyping, interactive systems, machine learning, laziness... Is it merely a coincidence? Or could lenses be a fundamental particle of PL? Discovering lenses in the wild may forever change how you see the world.

- **Reflecting on Random Generation (Harrison Goldstein).** Frameworks like QuickCheck provide domain specific languages (DSLs) for writing generators, programs that randomly generate program inputs that are useful for testing. Generators provide lots of utility for testers, enabling thorough testing of functions with hard-to-satisfy preconditions, but it turns out that there is even more potential utility hiding in plain sight. In this talk, I'll present reflective generators, a modified DSL for random generation that builds on ideas from bidirectional programming to improve workflows throughout the testing process. Reflective generators can do more than just sample input values: they can validate their own correctness, adapt their distributions based on user-specified examples, and even mutate test inputs while maintaining invariants. These new capabilities come at a relatively low cost and unlock state-of-the-art testing strategies that normally require entirely separate testing infrastructure.

- **One Quantum Algorithm, Inexpertly Explained (Lucas Silver).** This Friday, I will be presenting One Quantum Algorithm, Inexpertly Explained. As quantum computers continue to become bigger and more reliable, quantum computing promises to become very impactful on the field of computer science. In this talk, I hope to be able to bring someone from 0 quantum computing knowledge to understanding Simon's Algorithm, the first algorithm known to be exponentially faster than any known classical or probabilistic algorithm. It will be an informal chalkboard talk. Fair warning, my knowledge of quantum computing is new and still very limited. Still, I hope that this talk can still be very informative, as most of us have very limited knowledge about quantum mechanics.

- **Modal Logic & Type Theory (Lef Ioannidis).** Modal logics are contextual logics -- they allow us to qualify intuitionistic formulas as holding in a certain way, e.g. ‘necessarily’, ‘in the future’, ‘everywhere’, ‘probably’, ‘as everyone knows’, or ‘normally’. As pure functional programs need monads to interact with their environment, intuitionistic logic  needs modalities to prove things with respect to the environment. This Friday I will introduce Modal logics and Modal Type Theory in the way of Pfenning and Reed. Moreover, I will introduce some common modal logics (S4, LTL, Epistemic, Location, Lax, Authentication logic), in addition to models for structural modal logics (Kripke models, Bool-algebras with operators, coalgebras).

## PhD Application Workshop

On weeks 9 and 10 students will attend a workshop led by Joey on how to prepare competitive PhD applications. The workshop will hone in on the following topics.

- **Personal Statements.** How important are personal statements in an application? How personal should they be? What to include and not to include? How to format and outline them?

- **Letters of Recommendation.** How important are letters of recommendation in an application? What’s a good letter of recommendation? How can I strengthen my letters of recommendation? How to select letter writers? How to help your letter writers?

- **A Good Fit.** When is a program a good fit? How to find programs that are good fits? When is an adviser a good fit? How to find advisers that are good fits?


