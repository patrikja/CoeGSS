# Background

* [Patrik Jansson](https://www.chalmers.se/en/staff/Pages/patrik-jansson.aspx), Prof. of Comp. Sci., Chalmers, Sweden
    * Programming languages
    * Software technology
* Two current EU projects about "Global Systems Science (GSS)"
    * [CoeGSS.eu](http://www.CoeGSS.eu/)
    * [GRACeFUL-project.eu](http://www.GRACeFUL-project.eu/)
    * a \href{https://twitter.com/patrikja/status/299857568392704001}{``tweet-sized definition'' (from 2013)}:
\begin{quote}
GSS is about developing systems, theories, languages and tools for
computer-aided policy making with potentially global implications.
\end{quote}

Note that any computer simulation (and any model) of a global system
is bound to be a rather crude approximation in some aspects. Hopefully
we can still make it a good approximation in the aspects we want to
study.

## Earlier history:

* 2008 onwards: Collaboration with the Potsdam Institute for Climate Impact Research (PIK) and the Global Climate Forum (GCF)
* FP7 FET-Open project 2010-2013: GSDP (Carlo Jaeger)
* leading up to the FETPROACT1 call

# Theory and technology for "Computer-Aided policy making"

* Sequential Decision Problems TODO cite
* Economic (Game) Theory
* Agent Based Modelling
* Network Science
* [HPC was covered in the keyote yesterday]

# GSS Applications: some pilot projects

* Green Growth
* Health Habits
* Global Urbanisation
* Climate Resiliant Urban Design

TODO: fill in more about them

# GSS and language

* Any GSS model is bound to involve different scientific fields
    * what is the common specification language?
    * Mathematics
* "Computer-aided" means we also need *implementation* languages
    * often a *large* gap between mathematical model and implementation
    * need bridging: a tower of languages connected by tools

TODO: perhaps look up GRACeFUL slides about the gap?

# Challenges

* Validation & Correctness
    * Specification in computer-checked language
    * understandable for domain experts
    * static checking, interval arithmetics
    * proof tools, automated testing
* Mature implementations
    * running code /= HPC-ready code
* Access to data
    * open access data
    * integrity
    * confidentialty
    * standards
* Reproducibility
    * open source
    * models, theories
    * tools, methodologies
    * proper meta-data

# Conclusions

* The \href{https://twitter.com/patrikja/status/299857568392704001}{``tweet-sized definition'' (from 2013)}:
\begin{quote}
GSS is about developing systems, theories, languages and tools for
computer-aided policy making with potentially global implications.
\end{quote}
* Applications
    * Green Growth
    * Health Habits
    * Global Urbanisation
    * Climate Resiliant Urban Design
* Challenges
    * Validation & Correctness
    * Mature implementations
    * Access to data
    * Reproducibility

# Bibliography and links

jaeger13:GSSshort

Related projects:
* CoeGSS, GRACeFUL, DOLFINS, FOC, SIMPOL, SYMPHONY


[P7.GSS] C. Jaeger, P. Jansson, S. van der Leeuw, M. Resch and J. D. Tàbara. GSS: Towards a Research Program for Global Systems Science, Conference Version, prepared for the Second Open Global Systems Science Conference June 10-12, 2013, Brussels.

[P7.Economy] Cezar Ionescu, Patrik Jansson: Dependently-Typed Programming in Scientific Computing - Examples from Economic Modelling. Implementation and Application of Functional Languages (IFL) 2012: 140-156.

[P7.Climate] Cezar Ionescu, Patrik Jansson: Testing versus proving in climate impact research.  TYPES 2011: 41-54

[P7.Systems] Daniel Lincke, Patrik Jansson, Marcin Zalewski, Cezar Ionescu: Generic Libraries in C++ with Concepts from High-Level Domain Descriptions in Haskell - A Domain-Specific Library for Computational Vulnerability Assessment. IFIP TC 2 Working Conference, DSL 2009: 236-261

[P7.Exchange] Nicola Botta, Antoine Mandel, Cezar Ionescu, Mareen Hofmann, Daniel Lincke, Sybille Schupp, Carlo Jaeger: A Functional Framework for Agent-Based Models of Exchange.  Applied Mathematics and Computation, Vol. 218 Issue 8: 4025-4040.

Relevant Projects (Patrik Jansson, Chalmers)
* GRACeFUL: Global systems Rapid Assessment tools through Constraints FUnctional Languages (H2020-FETPROACT-2014: GSS - 2015-2018)
* GSDP: Global Systems Dynamics and Policy (FETOPEN 2010-2013)
* RAWFP: Resource AWare Functional Programming (Swedish Foundation for Strategic Research 2011-2016)
* StrongLib: Strongly Typed Libraries for Programs and Proofs (Swedish Research Council 2011-2015)
* FunC: "Putting Functional Programming to Work - Software Design and Verification using Domain Specific Languages" (Swedish Research Council 2009-2012)

Online sources:
* https://www.graceful-project.eu/
* https://sites.google.com/site/fhpcworkshops/
* http://global-systems-science.eu/
* http://global-systems-science.org/
* http://www.sigplan.org/
* https://github.com/patrikja
