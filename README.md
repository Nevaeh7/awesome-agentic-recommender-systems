# Awesome Agent Recommender Systems

A curated reading list for agentic recommender systems, LLM-based recommendation agents, multi-agent recommendation, agent recommendation, evaluation, safety, and governance.

Last updated: 2026-05-25.

## Scope

This list focuses on papers where agents are part of the recommender system itself: memory, planning, tool use, user simulation, multi-agent interaction, reward modeling, safety, auditing, or system orchestration. Adjacent resources are included when they are useful for writing related work or building systems.

Code links point to public repositories that are official, project-named, or clearly tied to the paper. If no public code was found, the entry uses `N/A`.

## Contents

- [Priority Reading Order](#priority-reading-order)
- [2026 Core Agentic Recommender Papers](#2026-core-agentic-recommender-papers)
- [2026 Benchmarks, Evaluation, Safety, and Governance](#2026-benchmarks-evaluation-safety-and-governance)
- [2026 Conversational, Multi-Agent, and Domain Systems](#2026-conversational-multi-agent-and-domain-systems)
- [Foundational and Active Repositories](#foundational-and-active-repositories)
- [Thematic Map](#thematic-map)
- [Related Work Notes](#related-work-notes)

## Priority Reading Order

1. MemRec, MARS, AMEM4Rec, RecNet, SAGER: memory and self-evolving user modeling in agentic recommenders.
2. AgenticRec, ChainRec, RecThinker, RRCM: tool use, reasoning, routing, and ranking-oriented agent optimization.
3. AgenticRS and AgenticRS-Architecture: conceptual and system-level framing for agentic recommender systems.
4. RecRM-Bench, RecoAtlas, AgentRecBench, LLMEvalRec: evaluation and benchmarking for recommendation agents.
5. TriRec, Visual Inception, AgentAttack, governable personalization: fairness, robustness, security, and policy risks.
6. MATCHA, ARARA, TRACE, LLMGreenRec, Rank-GRPO: domain and conversational systems.

## 2026 Core Agentic Recommender Papers

| # | Year | Title | Paper | Code | Venue / Status | Topic | Why relevant |
|---|---:|---|---|---|---|---|---|
| 1 | 2026 | Agentic Recommender System with Hierarchical Belief-State Memory | [link](https://arxiv.org/abs/2605.14401) | N/A | arXiv, submitted 2026-05-14 | Memory, belief state | Models recommendation as partial observability and manages event, preference, and profile memory with LLM-scheduled lifecycle operations. |
| 2 | 2026 | RRCM: Ranking-Driven Retrieval over Collaborative and Meta Memories for LLM Recommendation | [link](https://arxiv.org/abs/2605.07129) | N/A | arXiv, submitted 2026-05-08 | Memory retrieval, ranking | Connects collaborative memory and meta-memory retrieval to ranking-driven LLM recommendation. |
| 3 | 2026 | SAGER: Self-Evolving User Policy Skills for Recommendation Agent | [link](https://arxiv.org/abs/2604.14972) | N/A | arXiv, submitted 2026-04-16; revised 2026-04-21 | User policy skills | Studies how recommendation agents evolve per-user reasoning policies, not only semantic memory. |
| 4 | 2026 | Self-Distilled Reinforcement Learning for Co-Evolving Agentic Recommender Systems | [link](https://arxiv.org/abs/2604.10029) | N/A | arXiv, submitted 2026-04-11; revised 2026-04-17 | RL, co-evolution | Targets co-evolving user and recommender agents with self-distilled reinforcement learning. |
| 5 | 2026 | Rethinking Recommendation Paradigms: From Pipelines to Agentic Recommender Systems | [link](https://arxiv.org/abs/2603.26100) | N/A | arXiv, submitted 2026-03-27; revised 2026-04-09 | Concept, paradigm | Defines when modules become agents and how agent evolution differs from static recall, ranking, and reranking pipelines. |
| 6 | 2026 | AgenticRS-Architecture: System Design for Agentic Recommender Systems | [link](https://arxiv.org/abs/2603.26085) | N/A | arXiv, submitted 2026-03-27; revised 2026-04-09 | System architecture | Presents AutoModel-style lifecycle automation with training, feature, and performance agents. |
| 7 | 2026 | AgenticRec: End-to-End Tool-Integrated Policy Optimization for Ranking-Oriented Recommender Agents | [link](https://arxiv.org/abs/2603.21613) | N/A | arXiv, submitted 2026-03-23 | Tool use, RL, ranking | Combines ReAct-style recommendation tools with list-wise GRPO to align reasoning, tool calls, and ranking feedback. |
| 8 | 2026 | Entropy Guided Diversification and Preference Elicitation in Agentic Recommendation Systems | [link](https://arxiv.org/abs/2603.11399) | N/A | AAAI Spring Symposium 2026 | Preference elicitation | Uses uncertainty and diversification to guide agentic recommendation when user preferences are ambiguous. |
| 9 | 2026 | RecThinker: An Agentic Framework for Tool-Augmented Reasoning in Recommendation | [link](https://arxiv.org/abs/2603.09843) | N/A | arXiv, submitted 2026-03-10 | Tool-augmented reasoning | Focuses on external tool use and reasoning traces for recommendation agents. |
| 10 | 2026 | Deep Research for Recommender Systems | [link](https://arxiv.org/abs/2603.07605) | N/A | arXiv, submitted 2026-03-08 | Agentic recommendation service | Reframes recommendation from item lists to proactive research reports with user-trajectory simulation and report-generation agents. |
| 11 | 2026 | ChainRec: An Agentic Recommender Learning to Route Tool Chains for Diverse and Evolving Interests | [link](https://arxiv.org/abs/2602.10490) | N/A | arXiv, submitted 2026-02-11 | Tool-chain routing | Learns to route recommendation tool chains for diverse and changing interests. |
| 12 | 2026 | AMEM4Rec: Leveraging Cross-User Similarity for Memory Evolution in Agentic LLM Recommenders | [link](https://arxiv.org/abs/2602.08837) | N/A | arXiv, submitted 2026-02-09 | Cross-user memory | Uses cross-user similarity to improve memory evolution for LLM-based recommendation agents. |
| 13 | 2026 | RecNet: Self-Evolving Preference Propagation for Agentic Recommender Systems | [link](https://arxiv.org/abs/2601.21609) | N/A | arXiv, submitted 2026-01-29 | Preference propagation | Studies self-evolving preference propagation inside agentic recommender systems. |
| 14 | 2026 | LLMs as Orchestrators: Constraint-Compliant Multi-Agent Optimization for Recommendation Systems | [link](https://arxiv.org/abs/2601.19121) | N/A | arXiv, submitted 2026-01-27; revised 2026-02-04 | Multi-agent orchestration | Uses LLM orchestration for constraint-compliant multi-agent recommendation optimization. |
| 15 | 2026 | MemRec: Collaborative Memory-Augmented Agentic Recommender System | [link](https://arxiv.org/abs/2601.08816) | [code](https://github.com/rutgerswiselab/MemRec) | ACL 2026 Main | Collaborative memory | Builds a collaborative memory graph plus lightweight memory manager for LLM-based recommendation. |
| 16 | 2026 | ScienceDB AI: An LLM-Driven Agentic Recommender System for Large-Scale Scientific Data Sharing Services | [link](https://arxiv.org/abs/2601.01118) | N/A | arXiv, submitted 2026-01-03 | Scientific data recommendation | Applies agentic recommendation to large-scale scientific dataset discovery and data sharing services. |

## 2026 Benchmarks, Evaluation, Safety, and Governance

| # | Year | Title | Paper | Code | Venue / Status | Topic | Why relevant |
|---|---:|---|---|---|---|---|---|
| 1 | 2026 | RecRM-Bench: Benchmarking Multidimensional Reward Modeling for Agentic Recommender Systems | [link](https://arxiv.org/abs/2605.11874) | N/A | arXiv, submitted 2026-05-12 | Reward modeling benchmark | Benchmarks reward modeling dimensions for agentic recommender evaluation. |
| 2 | 2026 | RecoAtlas: From Semantic Plausibility to Set-Level Utility in LLM Recommendation Agents | [link](https://arxiv.org/abs/2605.18805) | [code](https://github.com/anonymized9/reco-atlas) | arXiv, submitted 2026-05-11 | LLM agent evaluation | Evaluates structured recommendation reports beyond semantic plausibility, including set-level utility. |
| 3 | 2026 | Visual Inception: Compromising Long-term Planning in Agentic Recommenders via Multimodal Memory Poisoning | [link](https://arxiv.org/abs/2604.16966) | N/A | arXiv, submitted 2026-04-18 | Safety, memory poisoning | Studies multimodal memory poisoning attacks against long-term planning in agentic recommenders. |
| 4 | 2026 | Is Your LLM-as-a-Recommender Agent Trustable? LLMs' Recommendation is Easily Hacked by Biases (Preferences) | [link](https://arxiv.org/abs/2603.17417) | N/A | arXiv, submitted 2026-03-18; revised 2026-04-23 | Trust, bias | Tests how easily recommendation agents can be shifted by biased preference signals. |
| 5 | 2026 | Breaking User-Centric Agency: A Tri-Party Framework for Agent-Based Recommendation | [link](https://arxiv.org/abs/2603.10673) | N/A | arXiv, submitted 2026-03-11; revised 2026-05-20 | Fairness, platform policy | Adds item agents and platform reranking to balance user utility, item exposure, and platform objectives. |
| 6 | 2026 | AgentSelect: Benchmark for Narrative Query-to-Agent Recommendation | [link](https://arxiv.org/abs/2603.03761) | N/A | arXiv, submitted 2026-03-04 | Agent recommendation benchmark | Useful when the task is recommending agents from narrative queries rather than recommending items to users. |
| 7 | 2026 | AgentAttack: LLM agents for multi-strategy shilling attacks in recommenders | [link](https://www.sciencedirect.com/science/article/pii/S0957417426000771) | N/A | Expert Systems with Applications 2026 | Security, shilling attack | Uses LLM agents to model multi-strategy recommender-system attacks. |
| 8 | 2026 | From Hidden Profiles to Governable Personalization: Recommender Systems in the Age of LLM Agents | [link](https://www.microsoft.com/en-us/research/publication/from-hidden-profiles-to-governable-personalization-recommender-systems-in-the-age-of-llm-agents/) | N/A | Microsoft Research, 2026 | Governance | Frames hidden user profiles and controllable personalization as policy issues for LLM-agent recommenders. |
| 9 | 2026 | A Survey on Generative Recommendation: Data, Model, and Tasks | [link](https://www.sciencedirect.com/science/article/pii/S2666651026000100) | N/A | AI Open 2026 | Survey | Broader generative recommendation survey useful for positioning agentic systems. |
| 10 | 2025 | AgentRecBench: Benchmarking LLM Agent-based Personalized Recommender Systems | [link](https://arxiv.org/abs/2505.19623) | N/A | arXiv, revised 2025-05-28 | Benchmark | Early benchmark for personalized LLM agent-based recommender systems. |

## 2026 Conversational, Multi-Agent, and Domain Systems

| # | Year | Title | Paper | Code | Venue / Status | Topic | Why relevant |
|---|---:|---|---|---|---|---|---|
| 1 | 2026 | Multi-Agent Video Recommenders: Evolution, Patterns, and Open Challenges | [link](https://arxiv.org/abs/2604.02211) | N/A | WSDM Companion 2026 | Video, multi-agent | Surveys evolution patterns and open challenges for multi-agent video recommender systems. |
| 2 | 2026 | LLMGreenRec: LLM-Based Multi-Agent Recommender System for Sustainable E-Commerce | [link](https://arxiv.org/abs/2603.11025) | N/A | DEFI 2025 proceedings; to appear in IEEE Xplore | Sustainable e-commerce | Multi-agent recommendation system for sustainability-aware e-commerce. |
| 3 | 2026 | MATCHA: A Multi-Agent Framework for Credible Health Conversational Recommender Systems | [link](https://openreview.net/forum?id=8kRtKj915L) | N/A | OpenReview, 2026 | Health CRS | Multi-agent health recommendation with credibility and conversational constraints. |
| 4 | 2026 | ARARA: A Personalized Learning Companion for Middle-School Mathematics | [link](https://genai-personalization.github.io/assets/papers/GenAIRecP2026/NainaChaturvedi_AgenticOrchestration.pdf) | N/A | GenAI Personalization workshop 2026 | Education, orchestration | Agentic orchestration for personalized learning support. |
| 5 | 2026 | TRACE: Training-free Retrieval-Augmented Conversational Recommendation | [link](https://aclanthology.org/2026.findings-eacl.238/) | N/A | Findings of EACL 2026 | Conversational recommendation | Retrieval-augmented conversational recommendation without model training. |
| 6 | 2026 | A Multi-Agent Conversational Recommender System | [link](https://ojs.aaai.org/index.php/AAAI/article/view/42382) | N/A | AAAI 2026 | Conversational recommendation | Direct multi-agent CRS design and evaluation. |
| 7 | 2026 | LLMEvalRec: An agentic framework for simulating users to evaluate news recommendation systems | [link](https://www.amazon.science/publications/llmevalrec-an-agentic-framework-for-simulating-users-to-evaluate-news-recommendation-systems) | N/A | Amazon Science, 2026 | User simulation, news | Uses LLM agents as simulated users for news recommender evaluation. |
| 8 | 2026 | ProPerSim: Developing Proactive and Personalized AI Assistants through User-Assistant Simulation | [link](https://openreview.net/forum?id=RV2aeCgxdB) | N/A | ICLR 2026 Poster | Proactive assistant simulation | Useful adjacent work for proactive personalization and user-assistant simulation. |
| 9 | 2026 | Rank-GRPO: Training LLM-based Conversational Recommender Systems with Reinforcement Learning | [link](https://openreview.net/forum?id=Xgw2D9cALS) | N/A | ICLR 2026 Poster | RL for CRS | Trains LLM-based conversational recommenders with ranking-oriented reinforcement learning. |
| 10 | 2026 | Emotion-Enhanced Dual-Agent Recommendation: Understanding and Leveraging Cognitive Conflicts for Better Personalization | [link](https://www.mdpi.com/2076-3417/16/1/253) | N/A | Applied Sciences 2026 | Dual-agent recommendation | Models cognitive conflict and emotion with dual agents for personalization. |
| 11 | 2026 | End-to-End Personalization via Unifying LLM Agents and Graph Attention Networks for Entertainment Recommendation | [link](https://www.mdpi.com/2078-2489/17/4/344) | N/A | Information 2026 | Entertainment, GAT | Combines LLM agents with graph attention networks for entertainment recommendation. |

## Foundational and Active Repositories

| # | Year | Title | Paper | Code | Venue / Status | Topic | Why relevant |
|---|---:|---|---|---|---|---|---|
| 1 | 2026 | AgentRecSys: A Survey of Recommender System with LLM-based Agent | [link](https://github.com/agiresearch/AgentRecSys) | [code](https://github.com/agiresearch/AgentRecSys) | Active survey repository | Survey, repository | Maintained list of LLM-agent recommender papers and repositories. |
| 2 | 2024 | On Generative Agents in Recommendation | [link](https://arxiv.org/abs/2310.10108) | [code](https://github.com/LehengTHU/Agent4Rec) | SIGIR 2024 | Generative agents | One of the key early generative-agent recommender papers. |
| 3 | 2024 | AgentCF: Collaborative Learning with Autonomous Language Agents for Recommender Systems | [link](https://arxiv.org/abs/2310.09233) | [code](https://github.com/RUCAIBox/AgentCF) | WWW 2024 | Collaborative agents | Uses autonomous language agents for collaborative recommendation. |
| 4 | 2024 | MACRec: A Multi-Agent Collaboration Framework for Recommendation | [link](https://arxiv.org/abs/2402.15235) | [code](https://github.com/wzf2000/MACRec) | arXiv 2024 | Multi-agent collaboration | Canonical multi-agent collaboration framework for recommendation. |
| 5 | 2024 | Prospect Personalized Recommendation on Large Language Model-based Agent Platform | [link](https://arxiv.org/abs/2402.18240) | [code](https://github.com/jizhi-zhang/Rec4Agentverse_Case) | arXiv 2024 | Agent platform | Explores personalized recommendation on an LLM-based agent platform. |
| 6 | 2024 | RAH! RecSys-Assistant-Human: A Human-Centered Recommendation Framework with LLM Agents | [link](https://ieeexplore.ieee.org/document/10572486) | [code](https://github.com/TheRepoForRAH/RAH) | IEEE 2024 | Human-centered agents | Human-centered recommendation framework involving recommender, assistant, and user. |
| 7 | 2024 | Large Language Models are Learnable Planners for Long-Term Recommendation | [link](https://dl.acm.org/doi/10.1145/3626772.3657683) | [code](https://github.com/jizhi-zhang/BiLLP) | SIGIR 2024 | Planning | Uses LLMs as learnable planners for long-term recommendation. |
| 8 | 2024 | A LLM-based Controllable, Scalable, Human-Involved User Simulator Framework for Conversational Recommender Systems | [link](https://arxiv.org/abs/2405.08035) | [code](https://github.com/zlxxlz1026/CSHI) | arXiv 2024 | User simulation | User simulator framework for conversational recommender systems. |
| 9 | 2024 | SUBER: An RL Environment with Simulated Human Behavior for Recommender Systems | [link](https://arxiv.org/abs/2406.01631) | [code](https://github.com/SUBER-Team/SUBER) | OpenReview 2024 | Simulation, RL | RL environment with simulated human behavior for recommender systems. |
| 10 | 2023 | Recommender AI Agent: Integrating Large Language Models for Interactive Recommendations | [link](https://arxiv.org/abs/2308.16505) | [code](https://github.com/microsoft/RecAI/tree/main/InteRecAgent) | arXiv 2023 | Interactive recommendation | Early LLM-powered interactive recommendation agent. |
| 11 | 2023 | User Behavior Simulation with Large Language Model based Agents | [link](https://arxiv.org/abs/2306.02552) | N/A | arXiv 2023 | User simulation | Early LLM-agent user behavior simulator for recommender research. |
| 12 | 2023 | RecMind: Large Language Model Powered Agent For Recommendation | [link](https://arxiv.org/abs/2308.14296) | N/A | arXiv 2023 | LLM recommender agent | Early LLM-powered recommendation agent baseline. |

## Thematic Map

| Theme | Start with | Useful next |
|---|---|---|
| Memory and evolving user models | MemRec, MARS, AMEM4Rec | RecNet, SAGER, RRCM |
| Tool use and reasoning | AgenticRec, RecThinker | ChainRec, Deep Research for Recommender Systems |
| Benchmarks and evaluation | RecRM-Bench, RecoAtlas | AgentRecBench, LLMEvalRec |
| Safety, trust, and governance | Visual Inception, bias hacking | AgentAttack, TriRec, governable personalization |
| Conversational recommendation | TRACE, Rank-GRPO | MATCHA, AAAI Multi-Agent CRS |
| Multi-agent and domain systems | MACRec, LLMGreenRec | ARARA, ScienceDB AI, video recommenders |

## Related Work Notes

- Use `agentic recommender systems` when the recommender has explicit agent properties: memory, planning, tool use, feedback loops, or autonomous lifecycle management.
- Use `LLM-based recommender agents` for LLM-centered systems that reason, converse, simulate users, or call tools.
- Use `agent recommendation` for systems like AgentSelect that recommend agents rather than items.
- Separate benchmarking papers from system papers. Evaluation work now covers reward modeling, report-level utility, simulated users, robustness, and bias.
- Treat code availability conservatively. A paper gets `N/A` unless a public repository is clearly connected to the work.

## Contributing

Contributions are welcome. Please keep entries concise and use the existing table format:

```markdown
| # | Year | Title | Paper | Code | Venue / Status | Topic | Why relevant |
|---|---:|---|---|---|---|---|---|
| 1 | 2026 | Paper title | [link](PAPER_URL) | [code](CODE_URL) | Venue / status | Topic | One-sentence relevance. |
```

Use `N/A` in the `Code` column when public code is unavailable.
