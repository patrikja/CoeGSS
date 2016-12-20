# CoeGSS
Informal repository of material for the DSL task of the http://coegss.eu/ project.

* [Reproducibility](2016-04/): An invited presentation by Patrik Jansson at the [ATI](https://turing.ac.uk/) [Symposium on Reproducibility for Data Intensive Research](http://www.bodleian.ox.ac.uk/whats-on/upcoming-events/2016/april/reproducibility-symposium).

Links:
* [Deliverable D3.2](http://coegss.eu/resources/d3-2/): [First Specification of new Methods, Tools and Mechanisms Proposed for the Support of the Application User and Programmer](http://coegss.eu/wp-content/uploads/2016/04/D3.2.pdf)

## Publications

### Published in LMCS 2016

**Title**: Sequential decision problems, dependent types and generic solutions

https://arxiv.org/abs/1610.07145

**Authors**: Nicola Botta, Patrik Jansson, Cezar Ionescu, David R. Christiansen, Edwin Brady
(Submitted on 23 Oct 2016)

**Abstract**: We present a computer-checked generic implementation for solving finite-horizon sequential decision problems. This is a wide class of problems, including inter-temporal optimizations, knapsack, optimal bracketing, scheduling, etc. The implementation can handle time-step dependent control and state spaces, and monadic representations of uncertainty (such as stochastic, non-deterministic, fuzzy, or combinations thereof). This level of genericity is achievable in a programming language with dependent types (we have used both Idris and Agda). Dependent types are also the means that allow us to obtain a formalization and computer-checked proof of the central component of our implementation: Bellman's principle of optimality and the associated backwards induction algorithm. The formalization clarifies certain aspects of backwards induction and, by making explicit notions such as viability and reachability, can serve as a starting point for a theory of controllability of monadic dynamical systems, commonly encountered in, e.g., climate impact research.

**Source code**: https://github.com/nicolabotta/SeqDecProbs

```bibtex
@article{DBLP:journals/corr/BottaJICB16,
  author    = {Nicola Botta and
               Patrik Jansson and
               Cezar Ionescu and
               David Christiansen and
               Edwin Brady},
  title     = {Sequential decision problems, dependent types and generic solutions},
  journal   = {CoRR},
  volume    = {abs/1610.07145},
  year      = {2016}
}
```

### In submission to JFP (2016-11-11):

**Title**: Contributions to a computational theory of policy advice and avoidability

**Authors**: Nicola Botta, Patrik Jansson, Cezar Ionescu

**Abstract**: We present the starting elements of a mathematical theory of
policy advice and avoidability. More specifically, we formalize a
cluster of notions related to policy advice, such as policy,
viability, reachability, and propose a novel approach for assisting
decision making, based on the concept of avoidability. We formalize
avoidability as a relation between current and future states,
investigate under which conditions this relation is decidable and
propose a generic procedure for assessing avoidability.  The
formalisation is constructive and makes extensive use of the
correspondence between dependent types and logical propositions,
decidable judgements are obtained through computations.  Thus, we aim
for a computational theory, and emphasize the role that computer
science can play in global system science.

**Support**: The work was supported by the GRACeFUL project (640954,
from the call H2020-FETPROACT-2014) and by the CoeGSS project (676547,
H2020-EINFRA-2015-1) in the context of Global Systems Science (GSS).

**Source code**:
https://gitlab.pik-potsdam.de/botta/IdrisLibs/tree/master/SequentialDecisionProblems/
