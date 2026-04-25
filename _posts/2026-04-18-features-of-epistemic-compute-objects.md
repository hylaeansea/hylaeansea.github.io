---
layout: post
title:  "A List of Possible Features for Epistemic Compute Objects"
date:   2026-04-18 17:17:17 +0000
categories: blog
---

*Intellectual Honesty Statement - This post was written 100% by the human author. AI was not consulted in any way for writing, editing, or art.*

# Introduction

This blog post is a result of me writing in my notebook and dreaming about the possible use cases and features of *Epistemic Compute Objects*. I am in the process of developing the first ECO (by this name and with this framing), however I wanted to get these ideas out of my head.

# Epistemic Compute Objects

In a [previous post](https://hylaeansea.org/blog/2026/03/06/Research-Agenda-Joint-Epistemic-Model-Building.html), I outlined a research agenda that I will be pursuing over the next handful of years, and have been noodling through during the last handful of years in one form or another. The agenda orbited around the idea of the Epistemic Compute Object. I don't think I explicitly defined it in that post and rather gave examples of its application and played around with some ideas. Here goes then:

**Epistemic Compute Object** - A triad of three models: The Mental Model or models of the user or community, A World Model as a simulation of parts or the whole of the domain, and a Language Model for constructing, mediating between, translating, and interpreting the Mental and World Models. The ECO is realized as a single collection of reference material, equations, papers, translations, indexing, models, simulations, LLM instructions, LLM model weights, training data, prompt response pairs, and other bits of information for a particular domain. In my head this is implemented as a single git repository that inherits all of the benefits of git (collaboration, version control, branching, forking, pull requests, issues, discussions etc (these last three are more features of online git repository tools)), however it could be any repository or database of prose and code. In short, and ECO is an evolving repository of knowledge AND CODE, with which we can develop better Mental Models in the individual, in groups, and in society; develop better World Models that we can use to check our assumptions, test different hypotheses, and generate training data for LLM RL; and develop better Language Models either through fine tuning open models with simulation and community sourced data, or simply through the definition of AI skills, instructions, [Model Context Protocols](), and context.

Thats the idea, not very concise of a definition but it is still fairly nascent and I fully expect the edges of this idea to get fuzzier and not sharper as we forge ahead. So with that what are some of the promised features of this construct?

# Epistemic Compute Object Features

## Singular

Maybe **the** primary feature of an ECO is that it houses papers, reference material, links to discussions or blog posts, simulation code, simulation configurations, public record, public policy, data, and more all in a single compute object: a single git repository. This allows us to have comments in the code that point to a document in the very same repository where an LLM reasoned about implementing that specific algorithm. And that document can point to the original publication where the equation/model/method etc was published, peer reviewed, and debated. This traceability can go the other way as well; a new reference publication can be included in the repository and marked as "needs to be included in the simulation" or "indexed but not yet coded." 

The ECO is also home to instructions for LLMs. We are still working through as practitioners of AI reasoning and code assist the best practices of how to use these models; and furthermore the best practices are ever evolving. However, there seems to be a strong signal that some degree of LLM specialization, context engineering, skills and instructions are useful for efficiently using LLMs. The ECO also houses these, in the form of claude.md, /skills/update_references.md, etc. The instructions on how to interact with this repository of knowledge and simulations are directly encoded in the same repository. 

The simulation output, the verified prompt response pairs generated from runs of the simulation, or encoding conference proceedings - the truth statements - are also encoded in the ECO. The GB of data that are thrown off by humans interacting with an ECO can be filtered, vetted, and used to test future updates to the ECO. There can be a sort of language based set of unit tests for the ECO (along side the simulation code unit tests of course). After we make a change we test it against these statements to see if we broke anything. 

## Non-Singular

The ECO is singular in that it houses all of the shards of information, functions, conversations in a single repo. But a feature of ECOs is that they can be overlapping, and interact with each other, and in a way be *non-singular*. Much like open source software, git sub-repositories, python packages, and rust crates reference each other, and specific versions of each other, ECOs can do the same. If there is a sub-domain that has a vibrant community maintained ECO, reference it, fork it and include it as a part of your domain ECO, create branches that leverage other simulation code or data or LLM weights. The power of software (and in particular open source software) is not that it is a bullet proof monolith that you can always trust, the power of open source is that it is an ecosystem of interacting individuals, code bases, and communities. ECOs should be the same vibrant ecology of data, ideas, and functions.

## Communication
While listening to a [podcast]() from Forethought on AI for societal decision making, I was struck with the idea that ECOs can have "high bandwidth communications between themselves." If we collect in one place papers, LLM instructions, simulations with MCPs, we can have LLMs reference this and communicate with other ECOs. These LLMs can either be specialized models fine tuned on the contents of the ECO, or frontier models that have skills, MCPs, instructions, and context derived from the ECO. This could look like "Anthropomorphic carbon driven heating ECO, debate the Developing Economies ECO about reasonable but precise treaties and legislation that should be proposed in this session of congress" - for example. 

This mode of agent based communication is far superior to engaging with a single frontier model on these topics for the primary reason that: **you can inspect and audit the interactions between these two models, precisely because they are different models.** You fundamentally cannot do this with single model interactions without complex mech interp, or reading (nowadays highly suspect) chain of thought reasoning. 

You could also conceive of different versions or branches or forks of the same ECO having high bandwidth but auditable conversations. Again, enabled by git, this could be a way to test new sims, or papers, or instructions that were added to the ECO. Akin to the qualitative unit test idea described above. 

## Collaboration

Again, leveraging the power of git (or similar version and change tracking system, you can use svn if you want to I guess), we inherit all of the collaboration features of git, and the associated cloud based git tools. Imagine if the best starting parameters of a science simulation were debated on a github issue in addition to it being debated at the bar after a day of the domain conference (I write in addition to because the hallway, breakout, and over a beer talk will never be replaced). You could have scientists rushing to these ECO discussion boards or issues to get their ideas in to be discussed and debated rather than throwing email barbs on distros, or from the back row at dimly lit conferences. If you want to be heard, put it in the issue. If you have a better idea, submit a pull request. The software community was handed the gift of these tools from the St. Linus, we can directly apply them to debates and simulations in whole scientific domains.

## Debate

There has been a ground swell of open science data movements encouraging or in some cases demanding that the authors of papers publish their code and or data. I am most excited when looking at a new arxiv paper on a topic I am interested in, and there is a blog, video, paper, data, and code link all in the prepub! When we have domain ECOs and there is a sticky topic to debate, the relevant parties can check out a branch or fork the ECO and make their adjustments, do their tests, write their LLM instructions, and then check in their work to be run, compiled, inspected, and verified by anyone, by everyone if it is an important topic. By leveraging the ECO, the debate is trackable, public, and has an implicit foundation to start from.


