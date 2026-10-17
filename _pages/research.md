---
layout: single
title: "Research"
permalink: /research/
author_profile: true
---

## Agentic User Simulation for Conversational Search

<div class="timeline-entry">
  <div class="t-head"><span class="t-title">NIST TREC 2026 User Simulation Track · CFDA Lab, Academia Sinica</span><span class="t-date">Jul 2026 – Present</span></div>
  <div class="t-sub">Advisor: Prof. Chuan-Ju Wang · Progress report: <i>Knowing When to Stop: A Planner–Speaker User Simulator for Conversational Dataset Search</i></div>
</div>

![Planner–Speaker user simulator and Planner training](/images/pubs/trec-planner-speaker.jpg)

- **Gap.** How many turns a user needs before being satisfied, and when the user gives up, are central signals for evaluating conversational search. Recent LLM-based user simulators make utterances more human-like, but none treats stopping as a separate decision: the conversation ends through text generated together with the wording, at a preset turn limit, or is not modeled at all.
- **Method.** A two-stage Planner–Speaker user simulator. At each turn, a trainable **Planner** tracks whether the information need has been met, revises an implicit profile record of how the user writes, and makes a binding decision to continue or end; a frozen **Speaker** then writes the message. The Planner is trained first with supervised fine-tuning (SFT) on real users' choices to continue or end, then with GRPO, using a calibrated turn-level stopping reward and a session-level reward that pulls the distribution of conversation lengths toward that of real users.
- **Findings.** On a test fold whose information needs and users never appear in training, the simulator is among the closest to real users in search moves and message length. The SFT Planner's mean conversation length deviates from real users by only 0.82 turns, less than any prior simulator compared (1.25–4.40), and a short GRPO run raises the rate of ending exactly where the real user ends by 33.3 percentage points.

TREC, run by the U.S. National Institute of Standards and Technology (NIST), is one of the most established evaluation campaigns in Information Retrieval; the 2026 User Simulation Track is co-organized by international scholars including Krisztian Balog (Google DeepMind). The final simulator was submitted to the TREC platform in October 2026, and full results will follow in the TREC 2026 notebook paper.

[Progress Report](https://drive.google.com/file/d/1mCF4xs1p5q5f17bQ70le_DFOFESeRUsR/view?usp=sharing)

## Hybrid Coevolutionary Opinion Games (H-COG)

<div class="timeline-entry">
  <div class="t-head"><span class="t-title">Undergraduate Research Project · Economics and Computing Lab, NYCU</span><span class="t-date">Feb 2026 – Present</span></div>
  <div class="t-sub">Advisor: <a href="https://iim.nycu.edu.tw/iim/ch/app/artwebsite/view?module=artwebsite&amp;id=37975&amp;serno=4cb17686-fcc1-48ac-bc4e-764d07d8555b">Prof. Po-An Chen</a> · First author (CSoNet 2026)</div>
</div>

![H-COG pipeline](/images/pubs/hcog-pipeline.jpg)

- **Gap.** Classical opinion games (Bhawalkar et al., STOC 2013) have no language reasoning, while LLM social simulations (Wang et al., COLING 2025) do not measure social efficiency.
- **Method.** H-COG places cost-minimizing Friedkin–Johnsen agents and LLM-driven agents in the same dynamically rewired network, initialized from real Reddit stance data, and varies their mixing ratio α.
- **Findings.** Over 540 simulations, LLM-heavy populations reach about five times the social cost of purely analytical ones; the cost comes from agents drifting away from their own prior beliefs under conformity pressure inside echo chambers.

Reviewers at CSoNet described the work as *"an innovative hybrid framework that combines opinion dynamics models with LLMs, addressing a clear gap in existing research and bridging formal theory and modern AI practice"*, with *"a thorough experimental protocol that evaluates social costs, echo-chamber formation, and polarization"*.

An earlier version was accepted at the TSWIM 2026 Research Incubator (workshop, no proceedings).

[arXiv](https://arxiv.org/abs/2609.27639) · [Conference Version](https://drive.google.com/file/d/1QeFYxf8hWJBCoYSXVHmx-F4M6fa_WBnx/view?usp=sharing) · [Accepted Proofs](https://drive.google.com/drive/folders/1j-7oCtDY1fzN_dVMAmKKIK1BdGHozUKe?usp=sharing) · [Paper page](/publications/2026-11-16-hcog-csonet/) · [Code & Data](https://github.com/Evan-Jiamg/Echo-Chamber-Simulation)
