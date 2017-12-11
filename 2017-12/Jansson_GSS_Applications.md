# My GSS background

* [Patrik Jansson](https://www.chalmers.se/en/staff/Pages/patrik-jansson.aspx), Prof. of Comp. Sci., Chalmers, Sweden
* Two current EU projects about "Global Systems Science (GSS)"
    * [CoeGSS](http://www.CoeGSS.eu/): Centre of excellence in GSS
    * [GRACeFUL](http://www.GRACeFUL-project.eu/): Global systems Rapid Assessment tools through Constraint FUnctional Languages
    * a \href{https://twitter.com/patrikja/status/299857568392704001}{``tweet-sized GSS definition'' (from 2013)}:
\begin{quote}
GSS is about developing systems, theories, languages and tools for
computer-aided policy making with potentially global implications.
\end{quote}

# My earlier GSS history:

* 2008 onwards: Collaboration with the Potsdam Institute for Climate Impact Research (PIK) and the Global Climate Forum (GCF)
* FP7 FET-Open project 2010-2013: GSDP (Carlo Jaeger) \GSSpaper
* leading up to the [FETPROACT-1-2014](http://cordis.europa.eu/programme/rcn/665162_en.html) call
    * DOLFINS, CIMPLEX, **GRACeFUL**, \ldots

# Theory and technology for "Computer-Aided policy making"

* Sequential Decision Problems \nocite{DBLP:journals/corr/BottaJICB16}
    * computing optimal policies for single decision makers
* Economic (Game) Theory
    * equilibria, multiple decision makers
* Agent Based Modelling
    * simulation of plausible system trajectories
* Network Science
    * the evolution of the contact (or contagion) networks
* High Performance Computing (HPC)
    * [covered in the keynote by B. Koller]

# GSS Applications: some pilot projects

* Green Growth
    * simulate the spreading of "green cars" in Europe
* Health Habits
    * smoking and obesity spreads over facebook!
* Global Urbanisation
    * real-estate pricing, and public transport as cities grow
* Climate Resilient Urban Design
    * computer-aided stakeholder interaction
    * constraint solving and water management

# GSS and language

* Any GSS model is bound to involve different scientific fields
    * what is the common specification language?
    * Mathematics
* "Computer-aided" means we also need *implementation* languages
    * often a *large* gap between mathematical model and implementation
    * need bridging: a tower of languages connected by tools

Note that any computer simulation (and any model) of a global system
is bound to be a rather crude approximation in some aspects. Hopefully
we can still make it a good approximation in the aspects we want to
study.

# Challenges

* Validation & Correctness
    * Specification in computer-checked language
    * understandable for domain experts
    * static checking, interval arithmetics
    * proof tools, automated testing
* HPC implementations
    * a research prototype is *far* from HPC-ready code
* Access to data
    * open access data
    * confidentiality, security
    * standards
* Reproducibility
    * open source models, theories
    * tools, methodologies

# Conclusions

* The \href{https://twitter.com/patrikja/status/299857568392704001}{``tweet-sized GSS definition'' (from 2013)}:
\begin{quote}
GSS is about developing systems, theories, languages and tools for
computer-aided policy making with potentially global implications.
\end{quote}
* Applications
    * Green Growth
    * Health Habits
    * Global Urbanisation
    * Climate Resilient Urban Design
* Challenges
    * Validation & Correctness
    * Mature implementations
    * Access to data
    * Reproducibility

# Bibliography and links

Related projects:

* CoeGSS, GRACeFUL, DOLFINS, FOC, SIMPOL, SYMPHONY

Some papers:

* Botta, Jansson, Ionescu. The impact of uncertainty on optimal emission policies, In submission to ESD, 2017.
* Botta & Jansson et al. Sequential decision problems, dependent types and generic solutions, LMCS 2017.
* Botta, Jansson, Ionescu. Contributions to a computational theory of policy advice and avoidability, JFP 2017.
* Jaeger, Jansson, van der Leeuw, Resch, Tàbara. GSS: Towards a Research Program for Global Systems Science, Conference Version, prepared for the Second Open GSS Conference, 2013, Brussels.
* Ionescu, Jansson: Dependently-Typed Programming in Scientific Computing - Examples from Economic Modelling. Implementation and Application of Functional Languages (IFL) 2012: 140-156.
* Ionescu, Jansson: Testing versus proving in climate impact research.  TYPES 2011: 41-54

\nocite{DBLP:journals/corr/BottaJICB16, botta_jansson_ionescu_2017_avoidability, Algehed:2017:VVD:3122948.3122953, SandbergEriksson:2016:AFT:2976022.2976025, esd-2017-86}
