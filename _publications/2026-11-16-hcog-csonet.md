---
title: "Agent-based Modeling: Equilibrium, Echo Chambers, and Efficiency in Hybrid Coevolutionary Opinion Games"
collection: publications
category: conferences
permalink: /publications/2026-11-16-hcog-csonet/
excerpt: '<b>Ming-Zhi Jiang</b>, An-Tzi Teng, Jun-En Liu, Po-An Chen, Yung-Ming Li. <span class="badge accepted">Accepted</span> <a href="https://arxiv.org/abs/2609.27639">arXiv</a> · <a href="https://github.com/Evan-Jiamg/Echo-Chamber-Simulation">Code &amp; Data</a>'
date: 2026-11-16
venue: 'International Conference on Computational Science and Network Intelligence (CSoNet 2026), Springer LNCS'
header:
  teaser: pubs/hcog-pipeline.jpg
paperurl: 'https://arxiv.org/abs/2609.27639'
citation: 'Ming-Zhi Jiang, An-Tzi Teng, Jun-En Liu, Po-An Chen, and Yung-Ming Li. (2026). &quot;Agent-based Modeling: Equilibrium, Echo Chambers, and Efficiency in Hybrid Coevolutionary Opinion Games.&quot; <i>In Proceedings of CSoNet 2026</i>, Ho Chi Minh City, Vietnam. To appear. arXiv:2609.27639.'
---

**Full paper:** [arXiv:2609.27639](https://arxiv.org/abs/2609.27639) · [Code & Data](https://github.com/Evan-Jiamg/Echo-Chamber-Simulation)

![H-COG pipeline](/images/pubs/hcog-pipeline.jpg)

**Abstract.** The rise of echo chambers and polarization in online social networks poses fundamental questions about the efficiency and stability of collective opinion formation. Traditional numerical opinion models provide formal tools for analyzing social cost and equilibrium, but often simplify communication into predefined update rules. Meanwhile, LLM-driven agents capture richer language-based reasoning and memory, yet neither paradigm accounts for their joint social cost.

We close this gap with the Hybrid Coevolutionary Opinion Game (H-COG) framework, integrating cost-minimizing Friedkin–Johnsen agents and Phi-4 LLM-driven reasoning agents in a dynamically rewired social network. Agent beliefs are initialized from 5,199 real-world Reddit stance comments, scored on a continuous [−1, +1] scale via a fine-tuned RoBERTa regressor, and a mixing parameter α controls the agent composition.

Our first result is that the coevolving graph converges under text-based updating as reliably as under an update rule with a known fixed point, which is what licenses reading a Price of Anarchy from it at all. On that basis, purely LLM-driven populations are roughly five times less efficient than purely analytical ones, and a decomposition of social cost locates the gap: language agents are displaced from their own prior positions rather than merely disagreeing with their neighbors. The same susceptibility makes them less polarized, so lower polarization here is a symptom of what makes them inefficient rather than evidence of better deliberation. No difference between three initial topologies is detected.

**Keywords:** Opinion dynamics · Echo chambers · Price of Anarchy · Language models · Agent-based modeling · Convergence

**Earlier versions.** An earlier version of this work was accepted at the Taiwan Summer Workshop on Information Management (TSWIM 2026), and won 1st place in the AI & Big Data Analytics division of the 2026 ORSTW Undergraduate Project Competition.
