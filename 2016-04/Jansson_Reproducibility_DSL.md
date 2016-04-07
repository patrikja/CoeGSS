# Who am I?

* [Patrik Jansson](https://www.chalmers.se/en/staff/Pages/patrik-jansson.aspx), Prof. of Comp. Sci., Chalmers, Sweden
    * Programming languages
    * Software technology
* Two EU projects about "Global Systems Science (GSS)"
    * [CoeGSS.eu](http://www.CoeGSS.eu/)
    * [GRACeFUL-project.eu](http://www.GRACeFUL-project.eu/)
    * a \href{https://twitter.com/patrikja/status/299857568392704001}{``tweet-sized definition'' (from 2013)}:
\begin{quote}
GSS is about developing systems, theories, languages and tools for
computer-aided policy making with potentially global implications.
\end{quote}

# Why reproduce?

* Why is reproducibility a good thing?
    * trust \pause
    * correctness \pause
    * independent checking \pause

* Terminology:
    * From "[12 Rs, de Roure, 2010](http://www.scilogs.com/eresearch/replacing-the-paper-the-twelve-rs-of-the-e-research-record/)"
\begin{quote}
Reproducible - enough information for an independent experiment to reproduce the results.
\end{quote}
\pause
    * Let's call "Enough information [...]" a **specification**
    * of an experiment = **implementation**

# Specification, implementation and proof

* "Enough information [...]" a **specification**
* of an experiment = **implementation**
\pause
* When is the implementation *correct* w.r.t. the spec.?
    * tradition science: *trust*
    * for maths and software: *proof* \pause
* If we have a formal system (a logic)
    * we may give a proof of correctness
    * (moving trust)

# Machine checked proof

* Dependent type theory
    * can express many specifications
    * and implementations
    * and proofs
* in the same formal system.

Proof assistants: [Coq](https://coq.inria.fr/), [Agda](http://wiki.portal.chalmers.se/agda/pmwiki.php), [Idris](http://www.idris-lang.org/), ...

# Back to some of all the "Rs" (for software)

 1. Repeatable: needs an implementation (source code or executable) \pause
 2. Reproducible: needs a specification \pause
 3. Reliable: strengthened by proofs \pause
 4. Reusable: helped by a language for combining experiments \pause

Risk: formal proofs improve 3. but damage 4.

# A short story about Dee and Foo

Actors: Dee the Domain Expert & Foo the Formaliser

Starting point: Dee has an experiment + informal description

Dee + Foo work on formalisation.

Happy ending?: formal spec. and computer proof of correctness

\pause

Drama:

* Dee cannot understand the formal spec.
* Foo cannot understand the domain.

# A Domain Specific Language to the rescue

Develop a Domain Specific Language for expressing the specification

* Dee can use familiar terminology
* Foo understands enough to construct the proof \pause

Or even better,

* Foo develops a library of proof components (like LEGO-bricks)
* now Dee can "assemble" the proof herself!

\pause

This is the ideal we strive for:

* not merely correct programs,
* nor even proven correct programs;
* we want proof done against a specification that is naturally expressed for a domain expert.

# Summary

Key points:

* experiment = implementation
* reproducibility requires also a *specification*
* *provability* is stronger than reproducibility
* dependently typed languages can express spec., impl. and proof
* formal specifications can introduce a "comprehension gap"
* Domain-specific languages (DSLs) can be used to bridge the gap

This is the ideal we strive for:

* not merely correct programs,
* nor even proven correct programs;
* we want proof done against a specification that is naturally expressed for a domain expert.
