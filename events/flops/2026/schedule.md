---
title: Symposium on Functional and Logic Programming 2026 - Schedule
subtitle: 18th International Symposium on Functional and Logic Programming - Schedule
layout: page
---

Note: This schedule is preliminary and subject to change!

## Tuesday, May 26

#### 9:30 Opening
#### 9:40 Invited talk: Gabriele Keller

<details>
<summary>
Accelerate – past, present and future
</summary>

<p>
Accelerate, a purely functional embedded parallel array language was
designed to give Haskell programmers an easy, high-level way to
exploit parallel hardware. It has been around for many years, and it
has seen signiﬁcant changes, some on the user level, but mostly in its
implementation behind the scene.
</p>

<p>
This talk brieﬂy introduces the language, and the concept of
functional parallel array languages in general. It also explores
upcoming changes now available in an experimental release - that
rethink fusion, scheduling, and code generation.
</p>

<p>
Fusion optimizations typically focus on merging producer-consumer
pairs to reduce intermediate structures and memory accesses. However,
many approaches struggle with multiple inputs and often fail to fuse
computations whose combination would be producing multiple outputs,
therefor missing optimizations opportunities. Accelerate’s new
strategy can deal with this situation. Yet, more powerful fusion
strategies complicate ﬁnding optimal solutions, as this is an
NP-complete problem, so this poses additional challenges.
</p>

<p>
The new scheduling strategy, which we present, enables mixing data and
task parallelism while preserving loop parallelism. In this respect,
it is unlike most approaches that convert all parallelism to
tasks. Preserving data-parallelism avoids task-parallel overhead and
supports selfscheduling for loops, o!ering full ﬂexibility: thread
counts and distribution need not be ﬁxed before execution.
</p>

<p>
Finally, a new backend-aware intermediate language enables
architecturedependent optimizations. Together, these innovations
promise to improve performance, and broaden Accelerate’s applicability
to modern hardware.
</p>

</details>

#### 11:00-12:30 Talks: Functional Programming

<details>
<summary>
Miyazawa, O., Nishizaki, S.: Matrix Coeffect: A Coeffect Calculus for Handling Interdependent Information
</summary>

Coeffects capture requirements that the environment imposes on
programs. Petricek’s structural coeffect calculus extends the simply
typed lambda calculus with a type-and-coeffect system. In this
framework, requirements such as variable reuse counts and the number
of past values needed in dataflow languages are represented by scalars
drawn from algebraic structures that relax some semiring axioms
(coeffect algebras). However, existing scalar- and vector-based
coeffect domains combine annotations componentwise and therefore do
not naturally capture constraints between interacting contextual
quantities, such as travel times between airports and departure times
at airports. To address this limitation, we introduce <i>Matrix Coeffect
Algebra</i>, a matrixvalued coeffect domain whose composition propagates
requirements across contextual components, enabling constraints
between interdependent quantities. We embed Matrix Coeffect Algebra
into Petricek’s structural coeffect calculus and prove its type safety
via his translational semantics. A flight-timetable case study
demonstrates that matrix-based coeffects enable dependency-aware
static checking in a coeffect type system. Our technical contribution
is a new matrix-valued coeffect algebra, used as an instantiation of
Petricek’s structural (schematic) coeffect calculus.

</details>

<details>
<summary>
Cabo, Q., Scholz, S.: Finding Programming Faults Even When Large Parts of the Code have Disappeared
</summary>

This paper proposes a debugging technique for functional programming
languages that enables debugging of highly optimised code even if the
code that actually is executed is very different from its original
specification. We suggest a combination of virtual shadow stacks,
uniqueness types, as well as pre- and post conditions for
functions. Using this combination, we can trace bugs through function
calls that may no longer exist at runtime at all. We describe how this
approach is realised in the functional array language SaC and we
demonstrate how we can enrich virtual stack traces with partial
argument information such as array dimensionality or shape.
</details>

<details>
<summary>
Arntzenius, M., Willsey, M.: Finite Functional Programming or, LAMBDA: the Ultimate Predicate
</summary>

We unify functional and logic programming by treating predicates as
functions equipped with their support: the set of inputs whose output
is nonzero. Datalog, for instance, is a language of finitely supported
boolean functions. Finite support allows representing functions as
input-output tables. Generalizing from boolean functions to other
pointed sets neatly handles aggregation and weighted logic
programming. We refer to the combination of finitely supported
functions, represented as data, with higher order functions,
represented as code, as <i>finite functional programming</i>. We give a
simple type system to check finite support, using graded effects to
check variable grounding and relevance types to model pointed sets.

</details>


#### 12:30-14:00 Lunch

#### 14:00-15:00 Talks: Logic Programming

<details>
<summary>
Li, F., Gupta, G.: Computing Supported Models via Transformation to Stable Models
</summary>

Supported models offer a semantics for logic programs that relaxes the
minimality constraint of stable models while maintaining logical
consistency through a support condition. Despite their theoretical
significance since 1988, supported models lack practical computational
tools integrated with modern Answer Set Programming (ASP)
infrastructure. We present a transformation-based method that enables
computation of supported models using standard stable model
solvers. Our approach transforms any ground logic program into an
equivalent program whose stable models correspond exactly to the
supported models of the original program. We implement this
transformation as a preprocessor for Clingo and demonstrate
applications in software verification, medical diagnosis, and planning
where supported models enable valuable exploratory reasoning beyond
stable models.
</details>

<details>
<summary>
Bohrer, R.: Demonic Dynamic Logic Programming **(Distinguished Paper)**
</summary>

This paper introduces a logic programming language called Demonic
Dynamic Logic Programming. It is based on the ground, Demonic fragment
of propositional dynamic logic, a well-studied program logic. Syntax,
operational semantics and proof-theoretic semantics are presented. The
theoretical foundations are validated by proving theorems such as
soundness and existence of uniform proofs. Applications to twoplayer
mathematical games are discussed and a pursuit-evasion game on a graph
is presented as a concrete example. By bringing program logic and
logic programming together, we hope to improve reasoning about
imperative programs within logic programs. Future work is discussed,
including extensions to game logic which hold the potential to
generate winning strategies of games.
</details>

#### 15:20-16:20 Talks: Logic Programming

<details>
<summary>
Zhou, N., Jiang, C., Bierlee, H., Stuckey, P.: Dynamic Programming and Tabled Logic Programming for Encoding Single-Constant Multiplication into SAT (Declarative Pearl) **Distinguished Paper**
</summary>

Encoding single-constant multiplication (SCM) constraints into SAT is
essential for solving a wide range of combinatorial problems involving
integer arithmetic. Although optimal SAT encodings for SCM are known,
they are often prohibitively expensive to generate for large
constants. This paper introduces a dynamic programming (DP) approach
that offers a practical balance between encoding quality and encoding
time. The proposed method recursively decomposes the binary
representation of the target constant into chunks and eliminates
common subexpressions across the chunks and their one’s
complements. The objective is either to minimize the number of
additions (the <i>min-k</i> objective) or to minimize the number of half/full
adders (the <i>min-a</i> objective). The DP algorithm is naturally expressed
and efficiently implemented using mode-directed tabling in
Picat. Although the approach does not guarantee optimality,
experimental results show that it produces high-quality encodings
while substantially reducing encoding time. This makes SAT-based
techniques considerably more practical for applications involving SCM
constraints. The full implementation is publicly available at:
<a href="https://github.com/nfzhou/Picat/blob/master/scm.pi"><code>https://github.com/nfzhou/Picat/blob/master/scm.pi</code></a>.

</details>

<details>
<summary>
Maieli, R., Acclavio, M.: Probabilistic Linear Logic Programming with an application to Bayesian Networks computations
</summary>

Bayesian networks are a canonical formalism for representing
probabilistic dependencies, yet their integration within logic
programming frameworks remains a nontrivial challenge, mainly due to
the complex structure of these networks.

In this paper, we propose <i>probLO (probabilistic Linear Objects)</i> an
extension of Andreoli and Pareschi’s LO language which embeds Bayesian
network representation and computation within the framework of
multiplicative additive linear logic programming. The key novelty is
the use of multi-head Prolog-like methods to reconstruct network
structures, which are not necessarily trees, and the operation of
slicing, standard in the literature of linear logic, enabling internal
numerical probability computations without relying on external
semantic interpretation.

</details>

#### 16:40-18:00 Student Research Competition and Posters

## Wednesday, May 27

#### 9:30 Invited talk: Kazunori Ueda

<details>
<summary>
Hierarchical Port Hypergraphs: Two Decades Toward a Unifying Structure for Declarative Languages
</summary>

<p>
Declarative languages take diverse forms with respect to data
structures and control structures. They encompass a broad range of
notions and paradigms, ranging from higher-order terms with binders to
concurrent processes with various forms of communication.
</p>

<p>
A natural but challenging question is whether many, if not all, of
these frameworks can be uniﬁed within a simple yet expressive
formalism, rather than merely combined into a larger formalism. Graphs
and graph rewriting provide a promising framework, since higher-order
terms can be represented as tree structures augmented with edges
encoding binding structures, while networks of processes can be
represented as graph nodes and edges representing processes and their
interconnection, respectively.
</p>

<p>
This perspective motivated us to design and implement LMNtal, a
graph rewriting language for modeling and programming. LMNtal was
conceived as an attempt to unify constraint-based concurrency
(a.k.a. concurrent constraint programming) and Constraint
Handling Rules [1], two extensions of concurrent logic programming,
within a simple setting consisting of <i>relations</i> and <i>zero-assignment
logical variables</i> that connect relations (i.e., without
function/constant symbols). This ‘degeneration’ naturally allows
computation to be interpreted in terms of graphs and graph
rewriting. Here, graphs are more accurately described as <i>port graphs</i>
(when each variable connects exactly two ports of graph nodes) or <i>port
hypergraphs</i> (when each variable may connect more than two ports), to
distinguish them from ordinary graphs in graph theory.
</p>

<p>
Programming languages for graphs remain largely under-explored,
presumably because graphs have poor aﬃnity with standard PL-style
inductive deﬁnitions. LMNtal addresses this issue by allowing graphs
to be represented as terms modulo structural congruence, which serves
as a PL counterpart of graph isomorphism.
</p>
</details>

#### 10:50-12:20 Tutorial

<details>
<summary>
Alama, J.: TypeScript, meet Lean!
</summary>

In this tutorial we'll get our hands dirty with Lean, a
dependently-typed functional language and proof assistant that mixes
proving and programming, including metaprogramming. Bring your laptop
and get your hands dirty as we see how we can embed TypeScript inside
Lean, with Lean checking our work as we go.
</details>

#### 12:20-13:30 Lunch

#### 13:30- Excursion 

#### 18:00- Banquet

## Thursday, May 28

#### 9:30 Invited talk: Fritz Henglein

<details>
<summary>
Mining algebra for power and performance
</summary>

<p> 

What do query processing, deep learning and quantum computing have in
common?  They can be formulated and generalized as dealing with linear
operators over spaces such as free (semi)modules and Hilbert spaces,
with associated classical algebras such as Boolean, associative and
tensor algebras.  The algebras have universal equational properties
that can be exploited at run time by judicious simplification.  Part
of the trick is resisting the temptation to normalize data to a normal
form, but employing symbolic operators that not only delay evaluation
(as in lazy evaluation), but act differently depending on the context
in which they occur at run time.  The challenge then is when and how
much to simplify, which data structures to use, and how to analyze the
algorithmic consequences.
</p>

<p>
We illustrate this methodology by applying it to 
</p>

<ul>
<li> relational first-order logic based query evaluation, where we show
  that it is easy to program worst-case optimal joins on in-memory
  data that are secure against algorithmic complexity attacks, require
  few lines of code in Python or Haskell and perform quite well
  compared to even highly advanced and mature query compilers and
  database systems;
</li>
<li>
  automatic differentiation (AD), where it leads to a DSL for
  compactly representing linear operators and computing their adjoints
  for reverse-mode AD.
</li>
</ul>

<p>
We will hint at other applications that we have developed in this
fashion, from quantum circuit simulation to greenwashing-proof virtual
energy sourcing. And we will encourage participants to think of more
cases where this may be a (potentially revisionist) way of formulating
their underlying methodology.
</p>

</details>

#### 11:00-12:30 Talks

<details>
<summary>
Pfingsten, B., Hemann, J.: A Fine-Grained Small-Step Semantics for Interleaving Search
</summary>

We present a deterministic small-step operational semantics for
miniKanren that explicitly represents the evolving search tree during
execution. This semantics models interleaving and goal scheduling with
fine granularity, exposing each evaluation step—goal activation,
suspension, resumption, and success. This approach supports reasoning
about miniKanren’s interleaving search behavior, helping users
understand surprising answer orders and operational effects. A
reference implementation undergirds an interactive visualizer that
renders the search tree as it develops and lets users step through
execution; we treat this tool as a consumer and demonstration of the
semantics. Our semantics and tool are illustrated by example and
validated through property-based testing.
</details>

<details>
<summary>
Tudor, A., Arias, J., Gupta, G.: Automatic Knowledge Gap Detection and Plan Validation Using Counterfactual Justifications
</summary>

Given the increased importance of physical AI, reliable planning in
dynamic environments remains a critical function of embodied
systems. In particular, care must be taken in how they interact with
situations outside the boundaries of their training. While planning
languages such as PDDL or STRIPS tend to be highly problem-dependent,
LLMs can be applied to broader and more general tasks in dynamic
environments, but remain prone to hallucinations. Logic-based systems,
in contrast, provide frameworks for a wide variety of problems and
offer justifications for complete and correct plans, but offer no
explanation when they cannot generate a plan. For example, VECSR, a
planning system based on the s(CASP) answer set programming system,
can create plans for unseen tasks by generalizing from a small number
of training tasks. However, this generalization is limited to tasks
achievable with actions learned during training. To address this
limitation, we propose and build the <i>Counterfactual Generation Module</i>,
which exploits the justification framework of s(CASP) to identify
counterfactuals for unachievable tasks. These counterfactuals allow us
to detect missing actions that should be incorporated into VECSR’s
knowledge base to enable task completion. We validate our proposal by
asking VECSR to generate action plans for 55 tasks outside the 10 it
was trained on. For 16 tasks, VECSR could not produce plans, and the
counterfactuals “identified” the actions that need to be learned to
complete 13 of them. Next, we evaluated 56 plans generated by GPT-4o,
observing that the module’s assessment of plan correctness
corresponded to human evaluation, supporting that the module itself is
correct.
</details>

<details>
<summary>
Coltharp, N., Libby, S., Israel, L., Li, Y.: Unifying Hindsight and Foresight: Lazy Cost Analysis as Functional Logic Programming
</summary>

Clairvoyance semantics and demand semantics are both pure and
time-cost equivalent to lazy evaluation, oﬀering alternatives to the
stateful natural semantics of lazy evaluation for analyzing
computation cost. Unfortunately, clairvoyance semantics is simple but
hard to execute, and demand semantics is executable but
complicated. In this paper, we propose a novel approach for unifying
these two semantics using functional logic programming. We propose (1)
a logical clairvoyance translation, which translates lazy functional
programs to functional logic programs where the computation cost is
reiﬁed, and (2) a logical demand translation, which is a simple
extension to the logical clairvoyance translation. We prove that these
two translations correctly implement clairvoyance and demand semantics
respectively using Agda. We also conduct case studies on examples
including insertion sort and Okasaki’s banker’s queue using
Curry/KiCS2 to show how these translations can be used in practice.
</details>

#### 12:30-14:00 Lunch

#### 14:00-15:00 Talks: Functional Programming

<details>
<summary>
Kiselyov, O.: More Fun with Monoids (Declarative Pearl)
</summary>

Playing with monoids and discovering for oneself how frequently they
turn up in various guises and how much is expressed by them is a
delight. Not only it brightens the day of important but frankly boring
data analytics. Not only it challenges to discover efficient (with the
constant time and space operation) monoids, which demands
ingenuity. In the words of Guy Steele, inventing efficient associative
combining operators is a <i>very big deal</i>. An efficient monoid opens up
parallel implementations – not just parallel but embarrassingly
parallel: The input sequence arbitrarily partitioned among workers,
all running in parallel with no races, dependencies or even memory
bank conflicts. This is the ideal for multi-core, GPU or distributed
processing.

In this paper we show why monoids are a big deal, and also a big fun
even more than expected. Horner rule and Boyer-Moore majority voting –
commonly regarded as prototypically inherently sequential – turn out
monoids, and hence embarrassingly parallelizable. As we generalize
monoids to observable monoids, we discover a new, vertical way to
combine them, enabling efficient iterated grouping and aggregation
directly on raw deserialized (big) data, on multicore or
multi-processor.
</details>

<details>
<summary>
Lam, C.: Optimizing Mesh Booleans by Being Lazy (System Description)
</summary>

Mesh Boolean operations (union, difference, intersection) enable the
combination of simpler shapes into complex forms, and are essential in
modeling software such as OpenSCAD, a popular functional programming
language in the Maker community. Although these operations are
intuitive to users, existing implementations often suffer from
performance or robustness issues. Manifold is a new open source
library designed for robust and efficient mesh Boolean operations. It
is up to hundreds of times faster than traditional methods using exact
arithmetic, and more robust than conventional float-based
techniques. In this paper, we describe a crucial design decision that
enabled this level of performance while maintaining a simple
user-facing API: implementing a functional and lazy API design,
coupled with expression tree rewriting before evaluation. Manifold has
recently been integrated into projects such as OpenSCAD (nightly
builds), Blender, and has bindings for various languages.
</details>

#### 15:20-16:20 Talks: Testing

<details>
<summary>
Morihata, A.: Test Your Polymorphic Functions with Boolean Values
</summary>

Testing of parametrically polymorphic functions is nontrivial because
an inappropriate type instantiation may lead to overlooking
bugs. Several studies have discussed sufficient conditions for
<i>complete testing</i>, i.e., a set of tests that can find every incorrect
input-output behavior. This paper studies <i>finite complete testing</i>,
namely complete testing by instantiating type parameters with
finite-domain types (Boolean type, in particular). The finiteness
brings not only exhaustive testing but also simpler test cases and
debugging than the existing state-of-the-art method, which may derive
complicated types whose elements are costly or even computationally
infeasible to identify. Based on the theory of parametric
polymorphism, known as relational parametricity or Wadler’s free
theorem, we formulate a sufficient condition for finite complete
testing; moreover, we provide a transformation that yields functions
more suitable for applying the theorem. Our theory only examines types
and hence applies even to black-box testing. A preliminary experiment
with the Haskell 98 Prelude library demonstrated the promise of the
current proposal, enabling finite complete testing of 57 functions
among 79 polymorphic functions.

</details>

<details>
<summary>
Boyland, P., Hyatt, S., Dewey, K., Hardekopf, B.: Breccia: A Functional DSL Compiled to Egglog for Test Input Generation
</summary>

Some prominent efforts within fuzz testing to automatically generate
test inputs with complex invariants (e.g., well-typed programs for
fuzzing compilers) have exploited logical satisfaction, such as using
Prolog to describe constraints and generate satisfying
instances. However, using Prolog has met with resistance from the
community due to the difficulty of writing Prolog descriptions with
acceptable performance. We propose an alternative logic
programming-based approach: Datalog. While Datalog improves on the
“effective programmability” of Prolog, it has its own issues: it is
less expressive than Prolog, its bottom-up evaluation strategy
requires keeping all generated terms in memory, and while it is easier
to program effective generators in Datalog than Prolog, it still
requires a specific style and has hidden pitfalls (such as
bounding). We introduce Breccia, a functional DSL for generating
objects with complex invariants that compiles to Egglog, a Datalog
language extended with equality saturation. We show that Breccia is
expressive enough to describe interesting objects such as well-typed
programs with non-trivial type systems, and that equality saturation
can greatly improve the performance of the resulting Egglog
generator. We compare Breccia against Prolog implementations of
similar generators in order to understand the tradeoffs involved.
</details>

#### 16:20-16:40 Closing, Awards

