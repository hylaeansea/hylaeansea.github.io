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

The ECO is also home to instructions for LLMs. We are still working through as practitioners of AI reasoning and code assist, the best practices of how to use these models; and furthermore the best practices are ever evolving. However, there seems to be a strong signal that some degree of LLM specialization, context engineering, skills and instructions are useful for efficiently using LLMs. The ECO also houses these, in the form of claude.md files, /skills/update_references.md files, etc. The instructions on how to interact with this repository of knowledge and simulations are directly encoded in the same repository. 

The simulation output, the verified prompt response pairs generated from runs of the simulation, or encoding conference proceedings - the truth statements - are also encoded in the ECO. The GB of data that are thrown off by humans interacting with an ECO can be filtered, vetted, and used to test future updates to the ECO. There can be a sort of language based set of unit tests for the ECO (along side the simulation code unit tests of course). After we make a change we test it against these statements to see if we broke anything. 

## Non-Singular

The ECO is singular in that it houses all of the shards of information, functions, conversations in a single repo. But a feature of ECOs is that they can be overlapping, and interact with each other, and in a way be *non-singular*. Much like open source software, git sub-repositories, python packages, and rust crates reference each other, and specific versions of each other, ECOs can do the same. If there is a sub-domain that has a vibrant community maintained ECO, reference it, fork it and include it as a part of your domain ECO, create branches that leverage other simulation code or data or LLM weights. The power of software (and in particular open source software) is **not** that it is a bullet proof monolith that you can always trust, the power of open source is that it is an ecosystem of interacting individuals, code bases, and communities. ECOs should be the same vibrant ecology of data, ideas, and functions.

## Communication
While listening to a [podcast](https://www.forethought.org/subscribe#podcast) from Forethought on AI for societal decision making, I was struck with the idea that ECOs can have "high bandwidth communications between themselves." If we collect in one place papers, LLM instructions, simulations with MCPs, we can have LLMs reference this and communicate with other ECOs. These LLMs can either be specialized models fine tuned on the contents of the ECO, or frontier models that have skills, MCPs, instructions, and context derived from the ECO. This could look like "Anthropomorphic carbon driven heating ECO, debate the Developing Economies ECO about reasonable but precise treaties and legislation that should be proposed in this session of congress" - for example. 

This mode of agent based communication is far superior to engaging with a single frontier model on these topics for the primary reason that: **you can inspect and audit the interactions between these two models, precisely because they are different models.** You fundamentally cannot do this with single model interactions without complex mech interp, or reading (nowadays highly suspect) chain of thought reasoning. 

You could also conceive of different versions or branches or forks of the same ECO having high bandwidth but auditable conversations. Again, enabled by git, this could be a way to test new sims, or papers, or instructions that were added to the ECO. Akin to the qualitative unit test idea described above. 

## Collaboration

Again, leveraging the power of git (or similar version and change tracking system, you can use svn if you want to I guess), we inherit all of the collaboration features of git, and the associated cloud based git tools. Imagine if the best starting parameters of a science simulation were debated on a github issue in addition to it being debated at the bar after a day of the domain conference (I write in addition to because the hallway, breakout, and over a beer talk will never be replaced). You could have scientists rushing to these ECO discussion boards or issues to get their ideas in to be discussed and debated rather than throwing email barbs on distros, or from the back row at dimly lit conferences. If you want to be heard, put it in the issue. If you have a better idea, submit a pull request. The software community was handed the gift of these tools from Saint Linus, we can directly apply them to debates and simulations in whole scientific domains.

## Debate

There has been a ground swell of open science data movements encouraging or in some cases demanding that the authors of papers publish their code and or data. I am most excited when looking at a new arxiv paper on a topic I am interested in, and there is a blog, video, paper, data, and code link all in the prepub! When we have domain ECOs and there is a sticky topic to debate, the relevant parties can check out a branch or fork the ECO and make their adjustments, do their tests, write their LLM instructions, and then check in their work to be run, compiled, inspected, and verified by anyone, by everyone if it is an important topic. By leveraging the ECO, the debate is trackable, public, and has an implicit foundation to start from.

I envision conversations like: 
- "If you don't agree with my conclusions from the sim that I ran, critique the sim starting parameters, or the elements of the sim, or the statistical equations used to draw conclusions from the output data", and 
- "I am fairly confident in the system of linear equations, can someone run this update through their golden data set of sim configurations to see if the conclusions change?", and
- "We have sparse data on this domain, what are the sensors, or telemetry we need to make this more precise?", and
- "If you were to change this assumption about your model what would you expect to change about your conclusions?"

In my career, I have gotten a lot of milage out of the statement "I think my code, data, and conclusions are correct, but I also acknowledge that I might have made a mistake or an incorrect assumption, here is my code, and data, in a single repo, please tell me where I am wrong." And this is dramatically more effective than, "I coded it, and I am an expert, therefore my code is likely right, and I don't want to, or don't have the capacity to debate other folks about their code or conclusions." 

We would still, I hope have spirited debate and playful banter, but I think ECOs provide a common computational language as a foundation for this debate.

## Literacy

While I acknowledge that ECOs might not solve the problem of being complex, hard to install, single OS, and bug ridden, I hope that engaging in this way might bring better software discipline, testing, and documentation. The inclusion and adoption of LLMs alone can bring these features, but maybe the most effective way to ward off tech debt and bad code is a wider user base. An ECO **could** be a repo that ANYONE can clone and install and run and ask questions of. By bringing software practices and discipline to prose knowledge and mental models via ECOs, we may stand a chance to make the layperson more literate in a wide variety of highly technical domains. 

Instead of relying on the conclusions of an economist, a single parent could "play" the grocery prices ECO and see how different policies affect their monthly food bill. Instead of relying on oil exploration companies to do thorough environmental impact analysis, a town council can run the ECO themselves and verify (or refute) these reports. If we make the UI good enough, and the sim engaging enough (and this is a big if) we maybe get a much wider set of people literate in economics, and environment, and science, and public health, and international diplomacy. There are risks in this of course, but I have to believe that the more human minds we have thinking about these things the better.

# Failure Modes of ECS

Any account of the features of an idea, should also include the bugs, drawbacks, and failure modes. Here are a few that I predict for ECOs, I am sure there are many more.

## Tribalism

Even the best examples of open source software teams have their tribes, cliques, and factions that sometimes go to war, and sometimes very publicly. I fully expect this to happen in this construct as well, especially when the system that is being built and debated, crosses between confirmable compilation, and more fuzzy natural language based knowledge. I expect the severity of this to mirror the culture in the respective domains, public policy might have more unresolvable disagreements than say modeling rainfall in a specific county (but maybe not!). This is part of human nature, we evolved in tribes, and our multi-scaled institutions that we have built with our big brains and mythology will inevitably have fissures and collapse. My hope is that ECOs will provide more of a common ground during these fissures. And while they wont be able to stave off the inevitable, they might make sharper and more coherent the arguments that cause them.

## Limits of Simulation

Simulationists in any domain, have to continually grapple with the fidelity, compromises, computational complexity, observability, and fundamental knowledge. Do I scale up the grid size to make the run faster so I can iterate, or do I keep it fine grained so I am confident in the results? Do I spend time to make the data visualization have a better color palate, or do I use the power point defaults because anyone who cares to read my work will deal with the colors? Or (near and dear to my heart), do I make this more of a game that people "play" or more of a sim that people "run." Any ECO simulation that makes compromises so that you don't need a HPC cluster to run, will INEVITABLY run up against "well that is a game not a sim so I don't trust the physics." This is a constant battle and will continue to be one. BUT.... an amazing reply could be - "You are a domain expert and pillar in this field, could you please look at the code and tell me what other nuance, system, or feature I should model to make this more realistic?" I am not going to compromize on art or UI because that is important, but I would love your input on making the science better." Maybe we don't get to everyone understanding every domain by playing compromised but beautiful simulations, but even if we increase the number of people thinking about these problems, that is winning. 

Maybe we will need disclaimers and science vs play ratings indicators, like "this game is rated 4 on the science vs game scale of 0-10 and shouldn't be used for final decision making in public policy." But then follow with "This ECO game development focused on implementing these species in ecological and environmental simulation, but did not include simulation of annual drought cycles." And you know what would be really good at writing these statements? The LLMs that are part of the ECO of course. 

The problems of simulation validation and verification wont go away, but this approach might make these systems legible and bring more eyes and minds to that fight.

## Corporate or National Proprietary Information

The ECO is designed from the beginning to be open. Openness is the oxygen, food, life of the ECO. There are now and will always be domains, or specific configurations of simulations, models, and data that the owner doesn't want to be in the open. I get that, I respect that. An mineral company that paid a University researcher to come up with a new quantum sensing technique for mineral exploration, doesn't necessarily want their competitor to "git clone" their innovation. I would contend though, that a good majority (maybe greater than 60%) of scientific data and models that underpin corporate innovation, started in 1) the open source, 2) government funded Universities, or 3) international consortiums. The ECO for global tech development doesn't exist yet, so these numbers are merely a guess, however the vast majority of value a company adds to their products or services are specific applications of fundamental tech and science, not the tech or science itself. 

The vast majority of the internet runs on Linux, the internet itself was built by a consortium; Apple has a great implementation of a device that connects to cell networks, data services, and websites that other companies built and own; Commercial companies that perform environmental impact assessments use publicly sourced data (NOAA, BLM, Census etc); on and on. Rather than being a mark against ECOs as an idea, there might spring up economies of ECOs and ECO derived products. Rather than just using open source software to bootstrap your company, imagine if you could use open source models, data, articles, and LLM skills to bootstrap your company. If you are successful, you contribute back or donate, or hire the developers. There are problems with this model as well. And there might very well be inherent evil in markets, but markets are very efficient at moving resources to places where they can be used to add value, and we might need some of this movement of resources if this idea is to take hold.

# Conclusions and Intellectual Humility

This idea is surely not new or novel. This formalism and way of talking about ECOs might, though, spark others (hopefully people that can code faster and better than I can) to think about organizing their knowledge like this. This might also add extra gravity to the wave of open source, open science data, AI alignment, and AI skills that are being developed, and give practitioners a way to think about their systems. There are hopefully other benefits, and certainly other failure modes, these are merely the ones that come up for me in my though experiments about this idea. I haven't formally built an ECO yet by this name, but I am actively working on one and hopefully can provide concrete examples in the near future. 




