# Reproducibility, Proofs and Domain Specific Languages

(A rough "script" for the slides in Jansson_Reproducibility_DSL.md)

## Who am I?

My name is Patrik Jansson and I'm a professor of computer science at
Chalmers University of Technology in Sweden. I do research on
programming languages and software technology.

I apply my research to Global Systems Science where the topic of
Reproducibility often pops up.

  GSS is about developing systems, theories, languages and tools for
  computer-aided policy making with potentially global implications.

# Why reproduce?

If we go back to the core issue of this symposium and ask ourselves:
why is reproducibility a good thing?

I argue that it is we want to *trust* our results.

Or in other words: we want to build *trust* in the *correctness* our
our results.

There is no point in reproducing incorrect results but there is a
limit to the trust in any one scientist. I'm not trying to blame
anybody else - I don't trust my own results without some kind of
"independent checking". The traditional scientific method includes
convincing yourself and describing the "experiment" in sufficient
detail that others can try to reproduce it.

  Reproducible - enough information for an independent experiment to
  reproduce the results. ... start with the description of the
  experiment ...

# Specification, implementation and proof

For brevity lets use "specification" for "enough information ..." or
"description of the experiment".

Then a "specification" is needed for reproducibility to make sense.

With this terminology a particular experiment is an "implementation"
of that specification. And to reproduce a result is to provide
(another) "implementation" of the same specification.

But how do we know that an implementation actally satisfies a
specification? For scientific experiments that is usually based on
trust - but with mathematics (and software) we have something stronger
at hand: proof! If we can express the specification in a formal system
(a logic) then there is some hope to prove (inside that logic) that
the implementation is correct. With a correctness proof we don't need
to reproduce the "experiment" (implementation) because we know it will
work.

But note that we have only moved the trust one step: what if the proof
is incorrect or the logic flawed? What we really need is a
computer-checked proof of correctness.

# Machine checked proof

Thus, if we talk about "digital experiments" and if we can express the
specification in a language the computer understands we can get the
computer to check the correctness for us (and in a sense do an
infinite number of "experiments").

It turns out that specifications written in dependent type theory
support both implementations and proofs in the same formal system (a
"programming logic"). Furthermore there are several implementations of
theorem provers which help humans write specifications,
implementations and proofs.

Popular dependently typed languages include Coq, Agda, and Idris and
Nicola has already shown some snippets of Idris code in his
presentation.

# Back to some of all the "Rs" (for software)

Now I want to connect back to the introductory talk about all the
"Rs": repeatable, reproducible, reliable, reusable, repurposable, ...
Now in the context of software artefacts.

1. Repeatable is about runing the experiment again. We need enough
  information to repeat the exact experiment. This needs more than
  just a specification, this needs a precise decription of the
  implementation -- the source code. With access to the source code
  you can re-run the experiment. (And if the run-time machinery is
  constant this should cause no surprises.)

2. Reproducible means we have enough information for conducting an
  independent experiment to reproduce the results. As we just said
  this means we need a specification (in addition to the
  implementation = the original experiment). And if the specification
  and the implementation can be expressed formally we can even attempt
  at proving correctness in general as a *stronger* form of
  reproducibility.

Another R is

3. Reliable - to trust the Research Object we must be able to verify
   and validate it. This is clearly a very strong argument for
   formalisation and proof-systems. (We can make a small trusted core
   proof-checker to minimize the part of the system we need to trust.)

4. Reusable - using the experiment as part of new experiments
  (possibly as a black box). In the formalisation context this means
  that we want a formal system - a language - to combine existing
  implementations (and specifications) to form more complex ones. A
  general (and sufficiently powerful) language is formally enough, but
  often difficult to understand.

Now here comes an important point: in any formalisation effort there
is a clear risk that the quest for sufficient expressivity and
precision makes the resulting specification unreadable for mere
mortals.

# A short story about Dee and Foo

Let's say we have a domain expert Dee with an experiment (an
implementation) and an informal description (a specification).  And we
have a formalist Foo helping Dee with the formalisation and computer
proof of correctness. Even if Foo succeeds in constructing a precise
specification and a complete formal proof that Dee's "experiment" is
correct, we have not gained much if Dee cannot understand the formal
specification.

# A Domain Specific Language to the rescue

This points to the need for a Domain Specific Language for expressing
Dee's specification using terminology which is familiar to her while
still precise enough that Foo can construct the proof (and the
computer can check it). Or even better, if we can construct a library
of proof components (like LEGO-bricks) so that Dee can "assemble" the
proof herself!

This is the ideal we strive for: not merely correct programs, nor even
proven correct programs; we want proof done against a specification
that is naturally expressed for a domain expert.

# Summary

Key points:
* experiment = implementation
* reproducibility requires also a *specification*
* *provability* is stronger than reproducibility (and can be more difficult)
* dependently typed languages can express specification, implementation and proofs
* formal specifications can be hard to understand
* Domain-specific languages can be used to bridge the gap
