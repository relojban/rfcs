- Feature Name: lojban-fork-charter
- Start Date: 2018-04-22
- RFC pull request:

# A Charter for a Lojban Fork

This document describes the creation of a new language derived from Lojban, that is, a Lojban fork.

## Table of Contents
[Table of Contents]: #table-of-contents

  - [Goals]
  - [Non-goals]
  - [Name]
  - [Assets]
  - [Tools]
  - [Governance and Processes]
  - [Initial Scope]

## Goals
[Goals]: #goals
 
Forking a project with the history of Lojban cannot be done lightheartedly. Yet, it can be a potential solution to the state of torpor that apperas to engulf the project and that leaves the feeling, shared by casual observers as well as experienced contributors, that the lanugage is destined to be forever left unfinished. Striving to reach an ideal final level of perfection, but never actually getting there.

The goal of this project is to bring back into Lojban a sense of progress, maintaining all of the substance and form of the language, but designing new processes around it to move it forward in a practical and efficient way. 

More concretely, the project will stay true to the core objectives of the Lojban language: to be the entertaining, challenging experiment in human language and communication that we all know, to explore the interconnections between human language and software, and to be used in the real world to speak with each other and create art.

All of this, while putting additional emphasis on:
  - Standarization.
  - Stability, but with a clear path for evolution.

By _standardization_, we mean that the project will focus on providing complete specifications of the language, and will make an effort to provide and maintain reference tools implementing such specifications. We also mean that development of a rich software ecosystem around the language, to parse it, manipulate it and produce it, should be recognized as one of the most fertile areas for innovation.

To make a fitting comparison, take a look at the case of the [CommonMark specification](http://commonmark.org/). Lojban, in its own way, faces challenges that are similar to the ones addressed by CommonMark: details of the language left unspecified, divergence of different dialects and fragmentation of the community. This project feels as a natural way forward the emergence of a well-specified "common Lojban", providing a stable foundation for language learners and for software developers.

By _stability with a clear path for evolution_, we mean that the language should not be a testing ground for every new idea in the field of linguistics. Instead, it should be a language that can be learnt once and used basically forever. However, we do not envisage to ever reach a "final", immutable state of the language. The vision is, on the contrary, to continuously allow refinements and adjustments (even rather big adjustments, if warranted) through a well-defined and simple process.

Think, as an example, at the way in which extremely popular programming languages such as C++ or Python evolve. There is a strong guarantee that a program written once will continue to be valid for a very long time. Still, every 5, 10 or 15 years, one can expect new versions of the language that introduce new constructs, change the semanitc of some corner cases or even (rarely) break compatibility with existing code. This is the kind of "careful evolution" that we think is appropriate for a constructed language like Lojban.

The exception to the careful evolution described above would the initial "beta" phase of the project. As it breaks free from the original Lojban, the opportunity arises to "start clean" and introduce changes with a relatively fast pace, including some of the proposals that emerged in and around the community and were "backlogged" to different extent during the last 15 years. These are suggested in the section [Initial Scope] below. After this "beta" phase, the approach would naturally become more conservative.

Taken together, the previous objectives can be summarized in a philosophy of _"Specify first, use later"_. This means that the effort to specify the language should come first, before the implications of the specifications on actual usage are fully known and understood (which is an impossible goal in practice). This is acceptable, since the mechanisms are there to make adjustments later if the rules in place and the needs of real-world users of the language become visibly misaligned.

This is in contrast with the historical approach of Lojban, more geared towards _"Use first, specify later"_, meaning that decisions tend to be taken only after gathering evidence of what works best in practice. Unfortunately, this leads to the vicious circle that, when there is no clear winner among a set of alternatives, fragmentation ensues, exacerbated by the lack of specifications. As a result, some aspects of the language end up being de-facto in a state of _"Use first, specify never"_.

Finally, we hope that this project will help relieve some pressure on Lojban by offering an avenue for a certain degree of experimentation and innovation outside of the historical project. Perhaps this could even help reignite some activity on Lojban itself as a result, which would be a worthy goal by itself.

## Non-goals
[Non-goals]: #non-goals

To avoid possible misunderstandings, it is appropriate to list here also the things that the project does _not_ try to achieve:
  - Quickly solve every problem of Lojban.
  - Accomodate all individual expectations on how the Lojban language should change.
  - Make a definitive statement on what a logical language should be.
  - Investigate all philosophical ramifications of the interactions between logic and language.

## Name
[Name]: #name

A nice project needs a nice name. We suggest __Relojban__.

To a speaker of English, French, Spanish (and many other languages) this name conveys the idea of "Lojban done again" or "Lojban done anew", which is roughly in line with the philosophy. And to a speaker of Lojban, it sounds somewhat as "Version 2 of Lojban", which is also pertinent. 

The forked language would then be `{la .relojban.}`. On the other hand, the gismu `lojbo` would remain to represent the general Lojbanic culture of which Relojban is part. If there is a need to refer specically to the forked language through a selbri, then the lujvo `reljbo` can be used.

## Assets
[Assets]: #assets

We believe that a significant part of the success of an endevour can be attributed to a judicious choice of the goals to pursue. Much more important than the name of the project, therefore, is its reach: if it is well-defined and well-delimited, it contributes to guide in a common direction the focus and attention of the members of the community (a very precious and scarce resource!).

Following this philosophy, Relojban defines as follows its _core assets_, the main products that the project commits itself to develop and maintain:

  - __A forked version of the CLL__ as the main reference for the language. It will keep of course the original copyright notice, and have a new title ("_The Relojban Language_") and author attribution "_derived from the original 'The Complete Lojban Language' by John Woldemar Cowan / maintained by the Relojban Community_".

  - __A reference course__. One official beginner's course for learning the language (in english) to be maintained within the project (while additional material can be maintained outside the project).

  - __A dictionary__. Comprising curated lists of cmavo, gismu, lujvo, and fuhivla with their definitions and properties (in machine-readable format) to be used as a reference.

  - __A reference parser__. The software (libraries and associated tools) implementing the language specifications.

  - __A corpus__. Standard texts with their associated parsing, to serve as reference material as well as test suite for software tools.

That's it, everything else is not a core asset of the project, at least in its first phase. This does not mean, however, that efforts towards different initiatives or activities would not be appreciated. On the contrary! Every Relojban-related contribution or idea, relating or not to the core resources, is welcome and should be pursued by anyone who so desires.

What the list means, is that at the end of the day we will look at the core assets to determine how much we have progressed and how much work still remains to be done. If those are not in good shape, the project as a whole is not in good shape. Any additional work outside the scope of the project enriches the community and comes as a bonus, but strictly speaking only the items above count when we assess whether the project is in good health or not.

## Tools
[Tools]: #tools

The main activities of the projects will take place in [Github](https://github.com/). Why Github? Honestly there is no emotional attachment to this choice, and for first-time users Github has indeed a steep learning curve. That said, a minimum requirement for the project is to have a place to maintain its assets, including the possibility to do version control (of course), propose and review changes, track issues, and discuss about them. This means that _some_ kind of tool is needed for these purposes, and there is a clear positive effect in having all of these activities done in the same place, limiting the cognitive burden for potential users and contributors. Github offers the path of least resistance for satisfying the requirements, simply because it is the platform where people are more likely to already have an account.

In practice, the resources of the projects will be maintained in Github public repositories, essentially:
  - one repository for the Relojban book
  - one repository for the course
  - one repository for the dictionary
  - one repository for the parser
  - one repository for the corpus
  - possibily other convenience repositories as needed for additional content (additional parsers, bindings, tools, administration, documentation)

In addition, two open mailing lists can be setup, one dedicated to general discussions about Relojban, the other dedicated to development-oriented topics.

English will be the "operational language" for running the project. This means that all day-to-day activities and interactions within the project, such as recording issues, commits, comments and proposals, are expected to be carried out in english. But discussions in Relojban would be highly appreciated on the general mailing list, of course!

## Governance and Processes
[Governance and Processes]: #governance-and-processes

When talking about the [Goals] of the project, we mentioned that Relojban should evolve through a well-defined and simple process. Here we state some principles that show, in general terms, how we envisage this process and what kind of interactions are expected among the people that are involved in it.

On the topic of interactions, one general but very important principle is this: the project should be run as much as possible in the spirit of openness, inclusiveness and kindness towards newcomers, valuing participation and contributions in all their forms, and supporting a collaborative and meritocratic approach to solving problems and forming consensus. As in every volunteer community, the community itself is the most important asset. Therefore any effort should be made to create a friendly and stimulating environment where respectful interactions and exchange of ideas are the norm, inspired by a basic [code of conduct](https://meta.wikimedia.org/wiki/Don%27t_be_a_jerk).

In terms of organizational structure, our view of Relojban is quite simple: we see it as a community formed by its _maintainers_ (defined as those with write access to the resources of the project) and its _contributors_ (anyone else that is interested in the project, including potential contributions that are not actively participating). That is, no complex internal structures and no specific roles are envisaged (at least from the point of view of Relojban's governance), apart from the roles implicitly defined by the access rights.

Against this background, the main question is then how changes can be introduced to make the project evolve over time. In other words, what should be the typical workflow for developing Relojban resources? How changes are proposed and discussed? How to form consensus around them?

The approach we propose consists in having two different workflows, depending on the type of change under consideration.

  1. For changes that are "ordinary day-to-day maintenance", we envisage a process based on __[lazy consensus](https://openoffice.apache.org/docs/governance/lazyConsensus.html)__, complemented by a __mandatory review__.

Everyone (maintainer or contributor) can propose a change. Then, if the change is just ordinary maintenance, it can be committed as soon as it has passed a review by a maintainer (different from the proposer).

Which changes are "ordinary maintenance"? Well, a bit of common sense will be needed for this assessment, of course. In general, these are changes such as bugfixes, corrections, improvements and additions that do not touch the features of the Relojban language (in the case of changes to the book or dictionary) and that do not touch the overall design or architecture of the object being changed (in the case of the parser and of other similar resources).

  2. For the other, "substantial" changes, we will follow an RFC process modeled around the __[Rust RFCs](https://github.com/rust-lang/rfcs)__.

The RFC process, in short, allows any member of the community, maintainer or contributor, to propose a substantial change (think of a change in the Relojban grammar, for instance) and makes sure that the discussion and consensus around the proposal is tracked and documented in a single place. It is then the role of the maintainers to evaluate the proposal, taking into account the consensus of the community, and finally take a decision after the benefits and drawbacks are well understood. For an overview of this process, please check the link above (making the necessary adjustments to relate it to the Relojban case).

We believe that this approach provides a good mix of simplicity, transparency and effectiveness, at least as a starting point while the project is in its infancy. But of course experience might tell us otherwise. We will not be afraid to change if the evidence is that this arrangement does not work very well in practice.

One important aspect that influences the dynamics described above is the size of the maintainers' team. In this respect, two contrasting philosophies are usually taken in consideration. One philosophy supports involving and promoting as many contributors as possible to the role of maintainers, to allow an higher flow of contributions and more "manpower" for the project. Another philosophy argues that the maintainers' team should be quite restricted, to make sure the project keeps [coneptual integrity](http://www.dcs.warwick.ac.uk/oldmodelling/hi/theses/allan/chapter5.pdf). This position is usually supported by the fact that the Github workflow makes it very easy to accept outside contributions. For Relojban, we advocate the latter view: having a restricted set of maintainers. But we note also that this might be a moot question: no more than one or two people might show interest in the project anyway :)

## Initial Scope
[Initial Scope]: #initial-scope

The following is a list of topics that we consider "in scope" of an hypothetical first release of Relojban. As you can see, almost none of these proposals is new, most of them refer to recurring items within the Lojban world, or are proposals that were already brought forward in one form or another in the last decades. The list assumes CLL Lojban+xorlo+dotside as the starting point (that is, xorlo and dotside are considered to be part of standard Lojban).

  - __Ortography__:
      - reconsider the function of commas and capital letters.
      - replace `'` with `h`. This proposal can be considered perhaps the more radical, as it changes the "visual signature" of Lojban/Relojban. There is however a potential argument in favour of introducing an intentional visually-breaking change: it will make the forked language instantly recognizable and distinct from Lojban, avoiding confusion between the two.
  - __Morphology__: a general re-specification and simplification of the morphology would be in scope, covering everything from the definition of syllables, to the formation of words of the different morphology types (cmavo, cmevla, gismu, lujvo, fuhivla). This will imply (together with the previous point) a rewrite of Chapter 3 and Chapter 4 of the CLL.
  - __Grammar__:
     - Redesign of the connective system
     - Consider (some of) the ce-ki-tau-jau substitutions.
     - Consider the introduction of adverbial clauses.
     - Other interventions on the grammar and on the cmavo space would be in scope when there is the potential for simplification or for better consistency (think for example of NAI grammar, mekso, "magic words", `soi`, termsets, ...). For instance, changes of the type included in [zasni gerna](https://mw.lojban.org/papri/zasni_gerna_cenba_vreji) could be considered in scope and evaluated.
  - __Relojban and Logic__: Taking xorlo as a starting point, it would be nice to create a consistent story around logical quatifiers in Relojban and their relations with the quantifiers of predicate logic. This would imply a rewrite of Chapter 16 of the CLL.
  - __Specifications__: Write new ones, to replace Chapter 21 of the CLL. They should not be tied to any implementation. They should cover separately the syntax rules (where a PEG is the natural representation) and rules or algorithms for ortography, morphology and magic words (where a PEG is _not_ the natural representation). Ideally, they should specify how to parse an input and produce a representation of the text in a suitable [object model](https://en.wikipedia.org/wiki/Object_model) (in the [DOM](https://en.wikipedia.org/wiki/Document_Object_Model) sense).
