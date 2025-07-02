---
title: Symposium on Functional and Logic Programming 2024
subtitle: 17th International Symposium on Functional and Logic Programming
layout: page
---

Welcome to the archival website of the 17th International Symposium on
Functional and Logic Programming (FLOPS 2024) May 15-May 17, 2024 in
Kumamoto, Japan.  (The original website of FLOPS 2024 is
[here](https://conf.researchr.org/home/flops-2024).)

FLOPS 2024 is
co-sponsored by Special Interest Group on Programming and Programming
Languages (SIG-PPL), Japan Society for Software Science and Technology
(JSSST), in cooperation with ACM SIGPLAN.

## About FLOPS

FLOPS aims to bring together practitioners, researchers and
implementers of declarative programming, to discuss mutually
interesting results and common problems: theoretical advances, their
implementations in language systems and tools, and applications of
these systems in practice. The scope includes all aspects of the
design, semantics, theory, applications, implementations, and teaching
of declarative programming. FLOPS specifically aims to promote
cross-fertilization between theory and practice and among different
styles of declarative programming.

Previous FLOPS meetings were held at Fuji Susono (1995), Shonan
Village (1996), Kyoto (1998), Tsukuba (1999),
[Tokyo](https://www.ueda.info.waseda.ac.jp/flops2001/) (2001), Aizu
(2002), [Nara](http://www.cs.tsukuba.ac.jp/~kam/flops2004/) (2004),
Fuji Susono (2006),
[Ise](http://www.math.nagoya-u.ac.jp/~garrigue/FLOPS2008/) (2008),
[Sendai](https://web.archive.org/web/20161224011357/http://www.kb.ecei.tohoku.ac.jp/flops2010/wiki/index.php?FrontPage)
(2010), [Kobe](http://www.org.kobe-u.ac.jp/flops2012/) (2012),
[Kanazawa](http://www.jaist.ac.jp/flops2014/) (2014),
[Kochi](http://www.info.kochi-tech.ac.jp/FLOPS2016/#pc) (2016), Nagoya
(2018), [<del>Akita</del>
online](https://www.ipl.riec.tohoku.ac.jp/FLOPS2020/#program) (2020),
and [<del>Kyoto</del>
online](https://conf.researchr.org/home/flops-2022) (2022).

## Papers

The [Proceedings](https://link.springer.com/book/10.1007/978-981-97-2300-3)
are published as Lecture Notes in Computer Science.14659.

-  [Complete Dependency Pair Framework for Almost-Sure Innermost
   Termination of Probabilistic Term Rewriting](https://link.springer.com/chapter/10.1007/978-981-97-2300-3_4)
   <br/>(Jan-Christoph Kassing, Stefan Dollase, Jürgen Giesl)
   
- [An ML-Style Module System for Cross-Stage Type Abstraction in
  Multi-Stage Programming](https://link.springer.com/chapter/10.1007/978-981-97-2300-3_13)
  <br/>(Takashi Suwa, Atsushi Igarashi)
  
- [Declarative Pearl: Rigged Contracts](https://link.springer.com/chapter/10.1007/978-981-97-2300-3_6)
  <br/>(Alexander Vandenbroucke, Tom Schrijvers)
  
- [DeepLLM: Casting Dialog Threads into Logic Programs](https://link.springer.com/chapter/10.1007/978-981-97-2300-3_7)
  <br/>(Paul Tarau)

- [System Description: Grants4Companies: Applying declarative methods for recommending and
  reasoning about business grants in the Austrian public
  administration](https://link.springer.com/chapter/10.1007/978-981-97-2300-3_9)
  <br/>(Bjoern Lellmann, Philipp Marek, Markus Triska)
  
- [Inferring Non-Failure Conditions for Declarative Programs](https://link.springer.com/chapter/10.1007/978-981-97-2300-3_10)
  <br/>(Michael Hanus)

- [Language-parameterized Proofs for Functional Languages with
  Subtyping](https://link.springer.com/chapter/10.1007/978-981-97-2300-3_15)
  <br/>(Seth Galasso, Matteo Cimini)

- [System Description: MetaOCaml: Ten Years Later](https://link.springer.com/chapter/10.1007/978-981-97-2300-3_12)
  <br/>(Oleg Kiselyov)

- [Being Lazy When It Counts](https://link.springer.com/chapter/10.1007/978-981-97-2300-3_11)
  <br/>(Chun Kit Lam, Lionel Parreaux)
  
- [System Description: ACGtk: A Toolkit for Developing and Running
  Abstract Categorial Grammars](https://link.springer.com/chapter/10.1007/978-981-97-2300-3_2)
  <br/>(Maxime Guillaume, Sylvain Pogodalla, Vincent Tourneur)

- [System Description: A theorem-prover for subregular systems: The
  Language Toolkit and its interpreter, plebby](https://link.springer.com/chapter/10.1007/978-981-97-2300-3_16)
  <br/>(Dakotah Lambert)

- [System description: A Constraint-based Mathematical Modeling Library
  in Prolog with Answer Constraint Semantics](https://link.springer.com/chapter/10.1007/978-981-97-2300-3_8)
  <br/>(François Fages)

- System Description: Rhyme: A Data-Centric Multi-Paradigm Query
  Language based on Functional Logic Metaprogramming
  <br/>(Supun Abeysinghe, Tiark Rompf)

- [Tabulation with Zippers](https://link.springer.com/chapter/10.1007/978-981-97-2300-3_5)
  <br/>(Marcos Viera, Alberto Pardo, João Saraiva)

- [Term Evaluation Systems with Refinements: First-Order, Second-Order,
  and Contextual Improvement](https://link.springer.com/chapter/10.1007/978-981-97-2300-3_3)
  <br/>(Koko Muroya, Makoto Hamana)

## Keynotes

### Algebraic Connection between Logic Programming and Machine Learning
#### Katsumi Inoue, NII

There have been attempts to connect machine learning and symbolic
reasoning, providing interfaces between them. This work focuses on our
original approach to integrate machine learning and symbolic
reasoning, in the context of algebraic approaches to logic
programming. We here realize logical reasoning using algebraic
methods, in which algebraic data structures such as matrices and
tensors are used to represent logical formulas. These reasoning
methods are robust against noise, while allowing for high parallelism
and scalable computation. Algebraic logic programming has been applied
to fixpoint computation, abduction, answer set programming and
inductive logic programming.

### Verse: A New Functional Logic Language
#### Lennart Augustsson, Epic Games 

Verse is a new functional-logic language. It has several unusual
features and this talk will give a brief overview of the language and
what makes it different from most other languages. Among other things,
Verse has deterministic choice, and choice is very much a first class
construct. The talk will also show a core calculus for Verse and how
we can use rewrite rules to give a semantics for the language.

### Verification of Refactoring in Answer Set Programming
#### Yuliya Lierler, University of Nebraska

Answer set programming is a declarative programming paradigm for the
development of knowledge intensive applications, especially those that
involve combinatorial search. It is rooted in work on the semantics of
logic programs, so that syntactically answer set programs are
reminiscent of those of Prolog. Yet, the systems that process these
programs, and the art of programming in this style, differ from
classical Prolog. The process of creating an answer set program
involves

1. representing a domain in the language of an answer set solver — a system for processing logic programs,
2. making that representation safe for grounding — a process of eliminating variables of the program by substituting object constants, and
3. tuning the representation to facilitate search efficiency.

The processes involved in making the representation safe and efficient
fall into the so-called refactoring, which is a common software
engineering practice. In this talk, we will discuss answer set
programming and its practices, as well as the proof assistant system
called Anthem, which is designed for the purpose of facilitating
proofs of correctness of the refactoring process. Examples will be
used to illustrate the key concepts of answer set programming the
operation of Anthem, and its logical foundations based on the
relationship between logic programs under the answer set semantics and
the process of converting logic programs into first-order logic
formulas called completion.

### Continuations from Three Angles
#### Youyou Cong, Tokyo Institute of Technology

Continuations represent the rest of the computation. This simple yet
powerful concept attracted me to programming languages research a
decade ago, and since then, I have been studying continuations from
different angles. In this talk, I will present three pieces of my work
on continuations, focusing on applications, theory, and learning,
respectively.

## Program Committee

- Jeremy Gibbons (Co-chair), Department of Computer Science,
  University of Oxford, United Kingdom
- Dale Miller (Co-chair), INRIA Saclay and LIX/Institut Polytechnique
  de Paris, France
- Sandra Alves, University of Porto, Portugal
- Matteo Cimini, University of Massachusetts Lowell, United States
- Maribel Fernandez, King's College London, United Kingdom
- Carsten Fuhs, Birkbeck, University of London, United Kingdom
- Robert Glück, University of Copenhagen, Denmark
- Patricia Johann, Appalachian State University, United States
- Yukiyoshi Kameyama, University of Tsukuba, Japan
- Ekaterina Komendantskaya, Heriot-Watt University and Southampton University, United Kingdom
- Y. Annie Liu, Stony Brook University, United States
- Anil Madhavapeddy, University of Cambridge, United Kingdom
- Aart Middeldorp
- Akimasa Morihata, University of Tokyo, Japan
- Gopalan Nadathur, University of Minnesota, United States
- Carlos Olarte, CNRS; LIPN; Université Sorbonne Paris Nord, France
- Andreas Rossberg, Independent, Germany
- João Saraiva, HASLab/INESC TEC, University of Minho, Portugal
- Alexis Saurin
- Paul Tarau, University of North Texas, United States
- Tachio Terauchi, Waseda University, Japan
- Alwen Tiu
- Kanae Tsushima, National Institute of Informatics, Japan
