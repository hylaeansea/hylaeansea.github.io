---
layout: post
title:  "An Exploration of the Seed of a Project"
date:   2024-12-14 09:27:02 +0000
categories: blog
---

# Introduction and Motivation

This blog is an experiment in response to my taking of the [Blue Dot Impact AI Alignment](https://aisafetyfundamentals.com/alignment/). In this course we get the oprotunity to study various definitions and approaches to AI alignment and then apply them to a project of our choosing in the final month of the class. The course work included techniques such as Reinforcement Learning from Human Feedback (RLHF), Constitutional AI, Mechanisitic Interpretability, and many more. The coursework was intended to provide a broad overview and then allow the students do dive into a field of their choosing. I was particularly intrigued by the discussion around and attempts to understand higher level cognition within a large laguage model as there seems to be a high level of debate about 1) how LLMs represent abstractions internal to the model, and 2) alignment techniques that operate on this level. I wanted to explore this a bit more through my project, however the time constraint of 4 weeks seems rather aggressive to acomplish anything meaningful in this area.

![AI Learning from Physics]({{site.baseurl}}/assets/images/DALL·E2024-12-19_09.49.53_generate_an_image_of_a_personification_of_an_LLM_interacting_with_a_personification_of_a_group_of_physics_and_math_models_just_to_answer_questions.webp)

Another one of my long time interests is in how we can use AI, ML, and Bayesian reasoning to understand how to make better decisions expecially under uncertainty and even in situations where we don't have readily computable cost functions, benefit functions, or a mathematical notion of preference. I have spent much of my career modeling physical systems through several mathematical and science domains and this field is very well developed and there are several efforts to integrate these mathematical models with Large Language Models:

1. **Anoop Cherian**, **Radu Corcodel**, **Siddarth Jain**, & **Diego Romeres**. (2024). *LLMPhy: Complex Physical Reasoning Using Large Language Models and World Models*. [arXiv:2411.08027](https://arxiv.org/abs/2411.08027)


1. **Haining Pan**, **Nayantara Mudur**, **Will Taranto**, **Maria Tikhanovskaya**, **Subhashini Venugopalan**, **Yasaman Bahri**, **Michael P. Brenner**, & **Eun-Ah Kim**. (2024). *Quantum Many-Body Physics Calculations with Large Language Models*. [arXiv:2403.03154](https://arxiv.org/abs/2403.03154)

1. **Raj Jaiswal**, **Dhruv Jain**, **Harsh Parimal Popat**, **Avinash Anand**, **Abhishek Dharmadhikari**, **Atharva Marathe**, & **Rajiv Ratn Shah**. (2024). *Improving Physics Reasoning in Large Language Models Using Mixture of Refinement Agents*. [arXiv:2412.00821](https://arxiv.org/abs/2412.00821)

1. **Hengguan Huang**, **Xing Shen**, **Songtao Wang**, **Dianbo Liu**, & **Hao Wang**. (2024). *Verbalized Probabilistic Graphical Modeling with Large Language Models*. [arXiv:2406.05516](https://arxiv.org/abs/2406.05516)

These are but a drop in the ocean of examples of researchers connecting physics or mathematical models to LLMs to produce better LLM results, correct high level concepts, and help the researchers understand how these models work. I have found relatively little work however in attempting to use feedback from the external physics and math models to fine-tune or otherwise alter the LLM itself. 

    *note: I didn't write there has been relatively little work, this is the obligatory nod to me knowing there are people out there doing this kind of work, however I havent found great examples of it*

The main goal of these papers is to give the model inferance time access to the external math models in order to refine the inferance time output. That is a nobel pursuit, and likely will produce a very large impact on the big science, complex systems, and big problem solving that our society needs to figure out. 

I am however going to explore the idea in this paper that external models can be used to generate feedback for fine-tuning of a base model. This idea is highly motivated by the concept of mental-models and mental model building in humans. This blog will attempt to answer the question: can we fine tune LLMs with feedback from math, science, and policy models to drive the LLM to build "mental models" of the simulation domain.


