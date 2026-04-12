---
layout: post
title:  "A Research Agenda for Joint Epistemic Model Building"
date:   2026-03-06 12:00:00 +0000
categories: blog
---

*Intellectual Honesty Statement - This article was co-written with Claude (Opus 4.6). The domain expertise, core thesis, editorial direction, both art pieces, and approximately 65% of the content are the author's and artists; the remaining ~35% — including structural framing, methodology formalization, and connective prose — was contributed by the AI.*

# A Research Agenda for Joint Epistemic Model Building

<figure style="text-align: center; margin: 2em 0;">
  <img src="../assets/images/Magenta_Sea.png" alt="Magenta Sea" style="display: block; margin: 0 auto; max-width: 100%; width: 600px; height: auto; border-radius: 4px;">
  <figcaption style="margin-top: 0.5em; font-style: italic; color: #666;">Magenta Sea - original art by Cheese Lord</figcaption>
</figure>

## Introduction

In a [previous post]({{ site.baseurl }}{% post_url 2025-01-18-World-Models-and-Language-Models %}), I explored the philosophical foundations of connecting Language Models with World Models to make policy computable. That investigation demonstrated that LLMs can generate world models, that those world models can produce emergent "new knowledge," and that the interplay between natural language and simulation opens a promising path toward computational policy analysis.

This post articulates the foundations of a research agenda built on that philosophy. The central idea is the **Epistemic Computational Object (ECO)** — a jointly built artifact that fuses three layers of model:

1. **Mental Models** — the conceptual frameworks, assumptions, and intuitions that domain experts and stakeholders bring to a problem
2. **World Models** — computational simulations that encode the dynamics, agents, and physical or social processes of a domain
3. **Language Models** — the LLM layer that mediates between human reasoning and computational simulation, translating intent into code, interpreting outputs into insight, and surfacing tradeoffs in natural language

The thesis is that none of these layers alone is sufficient for exploring complex multi-domain problems. Mental models lack computational rigor. World models lack the flexibility and communicability of natural language. Language models lack grounded, domain-specific dynamics. But together — jointly constructed, iteratively refined — they form an epistemic object that can be interrogated, debated, and evolved by multiple stakeholders.

An ECO is not simply a simulation built with AI assistance. The fundamental feedback between the three layers sharpens each of them: running the world model reveals where mental models are incomplete or contradictory; the language model surfaces assumptions that were previously implicit; updated mental models drive new simulation configurations that produce new surprises. More critically, the ECO serves as a **communication tool** and a **shared language**. Different stakeholders — scientists, policymakers, communities, engineers — inevitably carry different mental models of the same problem. These discrepancies are usually invisible, buried in jargon, unstated assumptions, and talking past one another. The ECO makes them visible. It gives people a shared computational object and a common vocabulary to identify where their models diverge, debate why, and work toward reconciliation. If everyone can jointly build, inspect, update, run, and *play* with the ECO, it becomes both the place where the debate happens and the language in which it is conducted.

There are numerous problem domains in which policy, economics, and physics all combine to make for a non-linear complex environment in which optimization schemes are non-intuitive and dynamic. In fact most of the social and economic development, natural resources stewardship, geo-political, and scientific advancement domains fall into this description; they are multi-faceted and very complex. Simultaneous to this increase in complexity though, is the increased availability of software, models, fundamental science, and especially computation that might provide a way to probe these complex domains. This research agenda is fundamentally focused on methods, models, and interfaces to make these complex domains **legible** to the subject matter expert and novice alike.

## Visualization Matters, Play Matters

A simulation that no one can interact with is an epistemic dead end. The ECO framework demands an interface layer — a way for stakeholders, domain experts, and even novices to explore tradeoffs and build intuition about complex systems. How an ECO is visualized, how it is manipulated, and how its outputs are presented fundamentally shapes whether it produces genuine shared understanding or just numerical artifacts.

Visualization is not a secondary concern — it is constitutive of the epistemic work. The choice of what to render, what to abstract away, and what controls to expose to a user determines which mental model updates are even possible. And there is a strong case that the most effective interfaces for exploring complex systems are *playful* ones — interfaces that invite experimentation, reward curiosity, and make it feel natural to ask "what if?" Serious games, interactive dashboards, and explorable explanations all belong in the design space for ECO interfaces. Getting this right is a research problem in its own right, and one that cuts across all three domains in this agenda.

## Three Domains

<figure style="text-align: center; margin: 2em 0;">
  <img src="../assets/images/ECO_vis_6.png" alt="Moon Sea" style="display: block; margin: 0 auto; max-width: 100%; width: 600px; height: auto; border-radius: 4px;">
  <figcaption style="margin-top: 0.5em; font-style: italic; color: #666;">Moon Sea - original art by kyjohnso</figcaption>
</figure>

To ground this agenda, I focus on three deliberately diverse domains. The diversity is the point: if the framework holds across domains with radically different physics, politics, and timescales, it has generality worth pursuing. I also chose these domains because they *could* be pivot points around which our future economic development, planetary health, and exploration hinge on.

### 1. AI Technology Uptake

Building on the [AI Tech Adoption Model]({{ site.baseurl }}{% post_url 2025-01-12-AI-tech-adoption-model %}) and the agent-based simulations from the World Models post, this domain is a natural starting point for the ECO framework.

Recent work on the macroeconomics of transformative AI, notably [Trammell's analysis of economic growth under AI-driven automation](https://philiptrammell.com/static/egtai_new.pdf), suggests that unequal adoption of AI could break the standard assumptions of balanced growth — the Kaldor Facts that have held for decades. Empirical efforts like the [Anthropic Economic Index](https://www.anthropic.com/research/the-anthropic-economic-index), which tracks real-world AI usage patterns across occupations, are beginning to provide observational data on where adoption is concentrating — currently dominated by mid-to-high wage technical roles, with minimal penetration in physical labor occupations — reinforcing concerns about uneven distribution. If AI capabilities concentrate among early movers, the resulting lock-in could fundamentally alter the distribution of economic power in ways that are difficult to reverse. This makes AI uptake policy not just a matter of efficiency but of long-run equity and economic structure.

- **Mental Model layer**: Stakeholder assumptions about adoption barriers — cost, trust, literacy, infrastructure, cultural resistance. What do policymakers *believe* drives or inhibits uptake? Where do those beliefs diverge from one another?
- **World Model layer**: An agent-based simulation (extending the agentpy work) that models populations, institutions, incentive structures, and network effects. Parameters drawn from real demographic and economic data where possible.
- **Language Model layer**: LLMs serve as the interface — translating policy proposals into simulation configurations, interpreting simulation outputs into policy briefs, and generating counterfactual scenarios ("what if we doubled the education budget but halved the subsidy?").

**Key research questions:**
- Can the ECO reveal non-obvious tradeoffs between equity and speed of adoption?
- Do emergent simulation behaviors challenge the mental models of domain experts?
- Can the language model faithfully translate between stakeholder intent and simulation parameters?

### 2. Marine Protected Areas Monitoring, Control, and Surveillance

The ocean is a domain where mental models are particularly fragile — our intuitions about deep-sea ecology, migratory patterns, and enforcement economics are limited by the sheer inaccessibility of the system. This makes it an ideal candidate for joint epistemic model building.

Research in the last 30 years has revealed the importance of the Earth's ocean in all of the planetary processes. All of our global economy, our health, biodiversity, global temperatures, atmospheric carbon, and in fact all life on Earth, critically relies on a healthy ocean. Yet bottom trawling, Illegal, Unregulated, and Unreported (IUU) fishing, illegal whaling, and potentially in the future extensive deep sea mining are having a long term destructive effect on the health of our oceans. Fortunately, we are seeing more countries protect large swaths of their territorial and EEZ waters through Marine Protected Areas. In 2024 the UN passed the Biodiversity Beyond National Jurisdiction (BBNJ) Treaty, ratified in 2025 and entering into force this year, which establishes the structures, recommendations, and policy for establishing MPAs in the High Seas.

Legal structures alone though do not make for a healthy ocean. These MPAs need to be monitored, controlled, and surveilled for them to be effective, and increasing the amount of area protected will necessitate creative ideas to monitor and enforce them. Organizations like [Ocean Mind](https://oceanmind.global/) and [Global Fishing Watch](https://globalfishingwatch.org/) have made extensive progress in monitoring fishing from satellite imagery, AIS, and VMS data, and these techniques will remain the workhorse for MPA enforcement. However, the incredible complexity of these interconnected systems, and the dramatic increase in protected area will likely necessitate new technical approaches. The BBNJ also calls out the need for technology transfer and sharing between nations, as monitoring will be the responsibility of everyone — especially Small Island Developing States whose territory is largely water and whose economies are even more critically dependent on a healthy ocean.

- **Mental Model layer**: Conservation biologists, fisheries economists, commercial fishing companies, coastal communities, and policy makers each hold different models of what an MPA should protect, how large it should be, and what enforcement looks like. These models often conflict.
- **World Model layer**: A simulation incorporating ocean circulation, species migration, fishing fleet behavior, economic pressures on coastal communities, and enforcement logistics — including the allocation of autonomous surface vehicles, earth observing satellites, aerial drones, and manned patrol vessels. This is a coupled human-natural system; the interesting dynamics live at the interface.
- **Language Model layer**: The LLM mediates between the ecological simulation and the policy conversation. It can generate natural language summaries of simulation runs, propose MPA boundary configurations based on stated objectives, and translate between the vocabularies of ecology, economics, and law.

**Key research questions:**
- Can the ECO help stakeholders with conflicting objectives (conservation vs. livelihood) find Pareto-improving MPA designs?
- Does the world model surface ecological dynamics (e.g., spillover effects, trophic cascades) that reshape stakeholder mental models?
- What are effective ways of monitoring MPAs
- Can the framework handle the deep uncertainty inherent in ocean systems?

### 3. Lunar Regolith Development

This domain stretches the framework into a frontier with almost no established mental models — and that is precisely the value. Lunar resource development is a domain where we must build our epistemic foundations from scratch, making the joint construction process itself the primary object of study.

With natural resources becoming increasingly expensive to uncover and exploit on Earth, countries and corporations have been pursuing outer space resources for decades. In this decade though, the cost to launch a kg of mass to space has dropped precipitously, and much of the raw materials for AI development, quantum computing, and nuclear fusion are present in abundance in asteroids and especially on Earth's Moon. These two factors — lower cost and abundance of resources — have tipped the risk vs. reward calculus to make outer space exploitation feasible now and highly probable within the near term.

Even with lower launch costs, automated mining and factories in space could potentially be captured by early movers and enable lock-in for very long time horizons, fundamentally breaking the Kaldor Facts of macroeconomic behaviour. The inevitability of this lock-in is highly dependent on several factors including automation, the physics and geology of regolith mining, additive manufacturing, power generation, economics on Earth, policy (currently the mining and exploitation of Lunar resources would be regulated by the 1960s Outer Space Treaty and a patchwork of laws giving companies the right to the resources they extract), and international diplomacy. Assuming that lock-in is a negative outcome, we should be studying ways of making lunar development more equitable, more secure, and ultimately beneficial to all of humanity.

Organizations like the [Open Lunar Foundation](https://www.openlunar.org/) have begun articulating what commons-based governance of the Moon might look like — emphasizing cooperative frameworks, shared stewardship, and open-access infrastructure like the Lunar Ledger for coordinating surface activities. This work provides an important counterpoint to the default trajectory of competitive extraction and first-mover lock-in, and offers a starting point for the governance assumptions that an ECO for this domain would need to encode and test.

- **Mental Model layer**: What do we *think* we know about lunar regolith processing, in-situ resource utilization (ISRU), and the governance of extraterrestrial resources? These mental models are drawn from small-scale experiments, analogue missions, and speculative policy frameworks (the Outer Space Treaty, the Artemis Accords). They are thin and contested.
- **World Model layer**: A simulation of regolith extraction, processing, and utilization — energy budgets, equipment degradation, supply chain logistics, and the economic viability of different ISRU pathways. Coupled with a governance model that explores resource rights, international cooperation, and commercial incentives. 
- **Language Model layer**: Here the LLM is especially valuable as a synthesis engine — pulling together scattered technical literature, helping formulate simulation parameters from sparse data, and generating policy scenarios for a domain where no real-world policy laboratory exists.

**Key research questions:**
- Can the ECO framework function in a data-sparse, high-uncertainty domain?
- How do different governance assumptions (commons vs. property rights vs. cooperative frameworks) change the optimal development pathway?
- Can the joint model-building process itself serve as a form of anticipatory governance?
- Assuming Lunar mining will be largely done by autonomous agents, what are the self replicating structures necessary to achieve this at scale?

## The Joint Construction Process

These three domains are not just parallel projects — they are instances of a shared methodology:

### Mental Model Elicitation
Capture the assumptions, beliefs, and conceptual frameworks of relevant stakeholders through structured interviews, workshops, or LLM-mediated dialogue. The output is a documented set of causal assumptions, contested claims, and shared objectives.

### World Model Construction
Use the Language Model to translate the elicited mental models into computational simulations. This is the approach explored in the World Models post — LLMs generating agentpy code, configuring parameters, building coupled system models. The key discipline is maintaining traceability: every simulation parameter should map back to a mental model assumption.

### Simulation and Divergence Detection
Run the world model under various configurations. The critical moment is when simulation outputs *diverge* from mental model expectations. These divergences are the epistemic payload — they are where new knowledge lives.

### Epistemic Update
Feed simulation results back through the Language Model to update, challenge, or refine the mental models. This is not a one-shot process — it is iterative. The ECO evolves through cycles of construction, simulation, surprise, and revision.

### Cross-Domain Transfer
Examine whether patterns, methods, or insights from one domain transfer to another. Does the agent-based adoption model from AI Uptake share structural similarities with fishing fleet behavior in the MPA model? Do governance frameworks for lunar resources illuminate anything about MPA enforcement? The cross-domain comparison is where the framework's generality is tested.

## What Makes This Epistemic

The word "epistemic" is doing specific work here. This is not just about building simulations — it is about building *shared understanding*. The ECO is a boundary object in the sense that Star and Griesemer (1989) described: an artifact that sits at the intersection of multiple communities of practice, flexible enough to be interpreted differently by each, but robust enough to maintain coherence across them.

The joint construction process — mental model elicitation, LLM-mediated translation, simulation, and epistemic update — is designed to make the model-building process itself a site of learning and negotiation. The goal is not a single "correct" model but a shared computational object that multiple stakeholders can interrogate, challenge, and evolve.


## Conclusion

The three domains — AI Uptake, Marine Protected Areas, and Lunar Regolith Development — stress-test the ECO framework across radically different contexts. The Epistemic Computational Object is the proposed unit of analysis: a jointly constructed, iteratively refined artifact that fuses mental models, world models, and language models into something greater than the sum of its parts. The problems are real, the tools are emerging, and the need for shared epistemic infrastructure has never been more acute.

*kyjohnso*
