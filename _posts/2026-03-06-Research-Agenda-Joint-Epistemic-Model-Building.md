---
layout: post
title:  "A Research Agenda for Joint Epistemic Model Building"
date:   2026-03-06 12:00:00 +0000
categories: blog
---

# A Research Agenda for Joint Epistemic Model Building

## Introduction

In a [previous post]({{ site.baseurl }}{% post_url 2025-01-18-World-Models-and-Language-Models %}), I explored the philosophical foundations of connecting Language Models with World Models to make policy computable. That investigation demonstrated that LLMs can generate world models, that those world models can produce emergent "new knowledge," and that the interplay between natural language and simulation opens a promising path toward computational policy analysis.

This post distills that philosophy into a concrete research agenda. The central idea is the construction of what I am calling an **Epistemic Computational Object (ECO)** — a jointly built artifact that fuses three layers of model:

1. **Mental Models** — the conceptual frameworks, assumptions, and intuitions that domain experts and stakeholders bring to a problem
2. **World Models** — computational simulations that encode the dynamics, agents, and physical or social processes of a domain
3. **Language Models** — the LLM layer that mediates between human reasoning and computational simulation, translating intent into code, interpreting outputs into insight, and surfacing tradeoffs in natural language

The thesis is that none of these layers alone is sufficient for exploring complex multi-domain problems. Mental models lack computational rigor. World models lack the flexibility and communicability of natural language. Language models lack grounded, domain-specific dynamics. But together — jointly constructed, iteratively refined — they form an epistemic object that can be interrogated, debated, and evolved by multiple stakeholders.

There are numerous problem domains in which policy, economics, and physics all combine to make for a non-linear complex environment in which optimization schemes are non-intuitive and dynamic. In fact most of the social and economic development, natural resources stewardship, geo-political, and scientific advancement domains fall into this description; they are multi-faceted and very complex. Simultaneous to this increase in complexity though, is the increased availability of software, models, fundamental science, and especially computation that might provide a way to probe these complex domains. This research agenda is fundamentally focused on methods, models, and interfaces to make these complex domains **legible** to the subject matter expert and novice alike.

## Visualization Matters, Play Matters

A simulation that no one can interact with is an epistemic dead end. The ECO framework demands an interface layer — a way for stakeholders, domain experts, and even novices to explore tradeoffs and build intuition about complex systems. How an ECO is visualized, how it is manipulated, and how its outputs are presented fundamentally shapes whether it produces genuine shared understanding or just numerical artifacts.

Visualization is not a secondary concern — it is constitutive of the epistemic work. The choice of what to render, what to abstract away, and what controls to expose to a user determines which mental model updates are even possible. And there is a strong case that the most effective interfaces for exploring complex systems are *playful* ones — interfaces that invite experimentation, reward curiosity, and make it feel natural to ask "what if?" Serious games, interactive dashboards, and explorable explanations all belong in the design space for ECO interfaces. Getting this right is a research problem in its own right, and one that cuts across all three domains in this agenda.

## The Three Simulations

To ground this agenda, I propose building ECOs across three deliberately diverse domains. The diversity is the point: if the framework holds across domains with radically different physics, politics, and timescales, it has generality worth pursuing.

### 1. AI Technology Uptake

Building on the [AI Tech Adoption Model]({{ site.baseurl }}{% post_url 2025-01-12-AI-tech-adoption-model %}) and the agent-based simulations from the World Models post, this simulation extends the work into a fuller ECO:

Recent work on the macroeconomics of transformative AI, notably [Trammell's analysis of economic growth under AI-driven automation](https://philiptrammell.com/static/egtai_new.pdf), suggests that unequal adoption of AI could break the standard assumptions of balanced growth — the Kaldor Facts that have held for decades. If AI capabilities concentrate among early movers, the resulting lock-in could fundamentally alter the distribution of economic power in ways that are difficult to reverse. This makes AI uptake policy not just a matter of efficiency but of long-run equity and economic structure.

- **Mental Model layer**: Stakeholder assumptions about adoption barriers — cost, trust, literacy, infrastructure, cultural resistance. What do policymakers *believe* drives or inhibits uptake? Where do those beliefs diverge from one another?
- **World Model layer**: An agent-based simulation (extending the agentpy work) that models populations, institutions, incentive structures, and network effects. Parameters drawn from real demographic and economic data where possible.
- **Language Model layer**: LLMs serve as the interface — translating policy proposals into simulation configurations, interpreting simulation outputs into policy briefs, and generating counterfactual scenarios ("what if we doubled the education budget but halved the subsidy?").

**Key research questions:**
- Can the ECO reveal non-obvious tradeoffs between equity and speed of adoption?
- Do emergent simulation behaviors challenge the mental models of domain experts?
- Can the language model faithfully translate between stakeholder intent and simulation parameters?

### 2. Marine Protected Areas Monitoring, Control, and Surveillance

The ocean is a domain where mental models are particularly fragile — our intuitions about deep-sea ecology, migratory patterns, and enforcement economics are limited by the sheer inaccessibility of the system. This makes it an ideal candidate for joint epistemic model building.

Research in the last 30 years has revealed the importance of the Earth's ocean in global biodiversity, carbon and temperature regulation, and the health of ecosystems — even land-based ecosystems. All of our global economy, our health, biodiversity, global temperatures, atmospheric carbon, and in fact all life on Earth, critically relies on a healthy ocean. Yet bottom trawling, Illegal, Unregulated, and Unreported (IUU) fishing, illegal whaling, and potentially in the future extensive deep sea mining are having a long term destructive effect on the health of our oceans. Fortunately, we are seeing more countries protect large swaths of their territorial and EEZ waters through Marine Protected Areas. In 2024 the UN passed the Biodiversity Beyond National Jurisdiction (BBNJ) Treaty, ratified in 2025 and entering into force this year, which establishes the structures, recommendations, and policy for establishing MPAs in the High Seas.

Legal structures alone though do not make for a healthy ocean. These MPAs need to be monitored, controlled, and surveilled for them to be effective, and increasing the amount of area protected will necessitate creative ideas to monitor and enforce them. The BBNJ also calls out the need for technology transfer and sharing between nations, as monitoring will be the responsibility of everyone — especially Small Island Developing States whose territory is largely water and whose economies are even more critically dependent on a healthy ocean.

- **Mental Model layer**: Conservation biologists, fisheries economists, coastal communities, and policy makers each hold different models of what an MPA should protect, how large it should be, and what enforcement looks like. These models often conflict.
- **World Model layer**: A simulation incorporating ocean circulation, species migration, fishing fleet behavior, economic pressures on coastal communities, and enforcement logistics — including the allocation of autonomous surface vehicles, earth observing satellites, aerial drones, and manned patrol vessels. This is a coupled human-natural system; the interesting dynamics live at the interface.
- **Language Model layer**: The LLM mediates between the ecological simulation and the policy conversation. It can generate natural language summaries of simulation runs, propose MPA boundary configurations based on stated objectives, and translate between the vocabularies of ecology, economics, and law.

**Key research questions:**
- Can the ECO help stakeholders with conflicting objectives (conservation vs. livelihood) find Pareto-improving MPA designs?
- Does the world model surface ecological dynamics (e.g., spillover effects, trophic cascades) that reshape stakeholder mental models?
- Can the framework handle the deep uncertainty inherent in ocean systems?

### 3. Lunar Regolith Development

This domain stretches the framework into a frontier with almost no established mental models — and that is precisely the value. Lunar resource development is a domain where we must build our epistemic foundations from scratch, making the joint construction process itself the primary object of study.

With natural resources becoming increasingly expensive to uncover and exploit on Earth, countries and corporations have been pursuing outer space resources for decades. In this decade, the cost to launch a kg of mass to space has dropped precipitously, and much of the raw materials for AI development, quantum computing, and nuclear fusion are present in abundance in asteroids and especially on Earth's Moon. These two factors — lower cost and abundance of resources — have tipped the risk vs. reward calculus to make outer space exploitation feasible now and highly probable within the near term.

Even with lower launch costs, automated mining and factories in space could potentially be captured by early movers and enable lock-in for very long time horizons, fundamentally breaking the Kaldor Facts of macroeconomic behaviour. The inevitability of this lock-in is highly dependent on several factors including automation, the physics and geology of regolith mining, additive manufacturing, power generation, economics on Earth, policy (currently the mining and exploitation of Lunar resources would be regulated by the 1960s Outer Space Treaty and a patchwork of laws giving companies the right to the resources they extract), and international diplomacy. Assuming that lock-in is a negative outcome, we should be studying ways of making lunar development more equitable, more secure, and ultimately beneficial to all of humanity.

Organizations like the [Open Lunar Foundation](https://www.openlunar.org/) have begun articulating what commons-based governance of the Moon might look like — emphasizing cooperative frameworks, shared stewardship, and open-access infrastructure like the Lunar Ledger for coordinating surface activities. This work provides an important counterpoint to the default trajectory of competitive extraction and first-mover lock-in, and offers a starting point for the governance assumptions that an ECO for this domain would need to encode and test.

- **Mental Model layer**: What do we *think* we know about lunar regolith processing, in-situ resource utilization (ISRU), and the governance of extraterrestrial resources? These mental models are drawn from small-scale experiments, analogue missions, and speculative policy frameworks (the Outer Space Treaty, the Artemis Accords). They are thin and contested.
- **World Model layer**: A simulation of regolith extraction, processing, and utilization — energy budgets, equipment degradation, supply chain logistics, and the economic viability of different ISRU pathways. Coupled with a governance model that explores resource rights, international cooperation, and commercial incentives. The likely operational reality is swarms of rovers, robots, and semi-autonomous agents on the Moon — the environment is far too harsh for sustained human presence, so automation is not optional but foundational.
- **Language Model layer**: Here the LLM is especially valuable as a synthesis engine — pulling together scattered technical literature, helping formulate simulation parameters from sparse data, and generating policy scenarios for a domain where no real-world policy laboratory exists.

**Key research questions:**
- Can the ECO framework function in a data-sparse, high-uncertainty domain?
- How do different governance assumptions (commons vs. property rights vs. cooperative frameworks) change the optimal development pathway?
- Can the joint model-building process itself serve as a form of anticipatory governance?

## The Joint Construction Process

The three simulations above are not just parallel projects — they are instances of a shared methodology that I want to formalize:

### Step 1: Mental Model Elicitation
Capture the assumptions, beliefs, and conceptual frameworks of relevant stakeholders. This can be done through structured interviews, workshops, or LLM-mediated dialogue. The output is a documented set of causal assumptions, contested claims, and shared objectives.

### Step 2: World Model Construction
Use the Language Model to translate the elicited mental models into computational simulations. This is the step explored in the World Models post — LLMs generating agentpy code, configuring parameters, building coupled system models. The key discipline is maintaining traceability: every simulation parameter should map back to a mental model assumption.

### Step 3: Simulation and Divergence Detection
Run the world model under various configurations. The critical moment is when simulation outputs *diverge* from mental model expectations. These divergences are the epistemic payload — they are where new knowledge lives.

### Step 4: Epistemic Update
Feed simulation results back through the Language Model to update, challenge, or refine the mental models. This is not a one-shot process — it is iterative. The ECO evolves through cycles of construction, simulation, surprise, and revision.

### Step 5: Cross-Domain Transfer
Examine whether patterns, methods, or insights from one domain transfer to another. Does the agent-based adoption model from AI Uptake share structural similarities with fishing fleet behavior in the MPA model? Do governance frameworks for lunar resources illuminate anything about MPA enforcement? The cross-domain comparison is where the framework's generality is tested.

## What Makes This Epistemic

The word "epistemic" is doing specific work here. This is not just about building simulations — it is about building *shared understanding*. The ECO is a boundary object in the sense that Star and Griesemer (1989) described: an artifact that sits at the intersection of multiple communities of practice, flexible enough to be interpreted differently by each, but robust enough to maintain coherence across them.

The joint construction process — mental model elicitation, LLM-mediated translation, simulation, and epistemic update — is designed to make the model-building process itself a site of learning and negotiation. The goal is not a single "correct" model but a shared computational object that multiple stakeholders can interrogate, challenge, and evolve.

## Open Questions and Next Steps

- **Tooling**: What is the right software stack for building ECOs? Agentpy is a starting point, but richer coupled simulations may require frameworks like Mesa, NetLogo, or custom physics engines. The LLM integration layer needs formalization.
- **Validation**: How do we validate an ECO? Traditional model validation (calibration against data) applies to the world model layer, but what does it mean to validate a mental model or an epistemic update?
- **Scaling participation**: Can the LLM layer make ECOs accessible to non-technical stakeholders? Can a fisherman in a coastal village or a local government official meaningfully interrogate and contribute to an MPA ECO?
- **Visualization and interaction**: The right interface can make complex dynamics legible; the wrong one can obscure them. Serious games, explorable explanations, and interactive dashboards all belong in the design space — getting the interface right is as much a research problem as getting the simulation right.
- **Alignment implications**: The World Models post raised the possibility of weak-to-strong self-generalization through LLM-generated world models. If ECOs produce genuine new knowledge, what are the alignment implications of AI systems that can extend their own epistemic reach through simulation?

## Conclusion

This research agenda is an invitation. The three domains — AI Uptake, Marine Protected Areas, and Lunar Regolith Development — are chosen to stress-test the framework across radically different contexts. The Epistemic Computational Object is the proposed unit of analysis: a jointly constructed, iteratively refined artifact that fuses mental models, world models, and language models into something greater than the sum of its parts.

The next posts in this series will begin the construction process for each of the three ECOs. The work starts now.
