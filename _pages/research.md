---
layout: single
title: "Research"
permalink: /research/
author_profile: true
---

My work sits where **LLM agents** meet **human behavior**: how to make language agents behave like real people, and what happens to a social system once such agents are part of it.

## Agentic User Simulation for Conversational Search

<div class="timeline-entry">
  <div class="t-head"><span class="t-title">NIST TREC 2026 User Simulation Track · CFDA Lab, Academia Sinica</span><span class="t-date">Jul 2026 – Present</span></div>
  <div class="t-sub">Advisor: Dr. Chuan-Ju Wang · Team member</div>
</div>

TREC, run by the U.S. National Institute of Standards and Technology (NIST), is one of the most established evaluation campaigns in Information Retrieval. The 2026 User Simulation Track, co-organized by international scholars including Krisztian Balog (Google DeepMind), asks how to build a simulator that reproduces how real people search in a conversation.

- **Architecture.** An Agentic Workflow in which a **Planner LM** makes the core decisions (what to ask, when to stop) and a **Speaker LM** turns those decisions into natural user queries.
- **Why this split.** Off-the-shelf user LMs sound human but follow instructions poorly, so instead of retraining one model, the decision-making is moved to a separate planner that steers the speaker.
- **Training.** Reinforcement learning with PPO and GRPO, using reward functions designed for turn-level and session-level realism.
- **Status.** The final simulator is scheduled for submission to the TREC platform in early October 2026.

## Hybrid Coevolutionary Opinion Games (H-COG)

<div class="timeline-entry">
  <div class="t-head"><span class="t-title">Undergraduate Research Project · Economics and Computing Lab, NYCU</span><span class="t-date">Feb 2026 – Present</span></div>
  <div class="t-sub">Advisor: Prof. Po-An Chen · First author (CSoNet 2026)</div>
</div>

![H-COG pipeline](/images/pubs/hcog-pipeline.jpg)

- **Gap.** Classical opinion games (Bhawalkar et al., STOC 2013) have no language reasoning, while LLM social simulations (Wang et al., COLING 2025) do not measure social efficiency.
- **Method.** H-COG places cost-minimizing Friedkin–Johnsen agents and LLM-driven agents in the same dynamically rewired network, initialized from real Reddit stance data, and varies their mixing ratio α.
- **Findings.** Over 540 simulations, LLM-heavy populations reach about five times the social cost of purely analytical ones; the cost comes from agents drifting away from their own prior beliefs under conformity pressure inside echo chambers.

Reviewers at CSoNet described the work as *"an innovative hybrid framework that combines opinion dynamics models with LLMs, addressing a clear gap in existing research and bridging formal theory and modern AI practice"*, with *"a thorough experimental protocol that evaluates social costs, echo-chamber formation, and polarization"*.

[Paper page](/publications/2026-11-16-hcog-csonet/) · [Code & Data](https://github.com/Evan-Jiamg/Echo-Chamber-Simulation)

## Other Projects

- **[Python-ML-Quant](https://github.com/Evan-Jiamg/Python-ML-Quant):** notebooks on Black–Scholes option pricing, genetic algorithms, LPPL bubble detection, decision trees and CNNs.
- **[H-CAP](https://github.com/Evan-Jiamg/H-CAP):** an inclusive-finance system for migrant workers in Taiwan, combining OID4VCI digital credentials, AI voice interviews and blockchain remittance tracking.
- **[Algorithm-Practice-Collections](https://github.com/Evan-Jiamg/Algorithm-Practice-Collections):** C++ implementations of Knight's Tour, N-Queens, Kruskal/Prim MST and more, each with a GUI visualization.
