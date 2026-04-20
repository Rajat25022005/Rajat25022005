<div align="center">

# Rajat Malik

**AI / ML Engineer**

*Representation Learning · Reasoning Systems · Autonomous Intelligence*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/rajat-malik-a62876278)
[![HuggingFace](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black)](https://huggingface.co/rajat5039)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/Rajat25022005)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:rajatmalik5039@gmail.com)

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=16&pause=1200&color=58E6B0&center=true&vCenter=true&width=680&lines=Latent+Reasoning+Without+Chain-of-Thought;Graph-Based+Memory+%26+Retrieval;Agentic+Systems+%26+Autonomous+Planning;Research+Models+%E2%86%92+Production+Systems)](https://git.io/typing-svg)

![Profile views](https://komarev.com/ghpvc/?username=Rajat25022005&style=flat-square&color=58e6b0)

</div>

---

## About

B.E. Computer Science (AI & ML), Chandigarh University · Python Developer Intern, EDSHODH LLP

I build AI systems at the intersection of **representation learning**, **structured reasoning**, and **systems engineering** — enabling models to move beyond surface-level pattern matching toward memory-grounded, causally-aware, and long-horizon inference.

Recurring themes: learning over time and structure, explicit memory via graphs and retrieval, multi-agent decomposition of complex tasks, and translating research into deployable systems.

---

## Featured Research

### think-in-silence &nbsp; [![HuggingFace](https://img.shields.io/badge/model-published-FFD21E?style=flat-square&logo=huggingface&logoColor=black)](https://huggingface.co/rajat5039/think-in-silence)

> **Latent Reasoning Without Chain-of-Thought**

A latent reasoning architecture that performs silent K-step reasoning entirely in a **256-dimensional vector space** — no chain-of-thought tokens, no RL. Trained with a JEPA objective and an EMA teacher on 504K synthetic multi-hop QA pairs.

**Architecture**

- Backbone: Gemma-3-4B-it with 4-bit NF4 quantization — frozen in Stage 1–2, partially unfrozen in Stage 3
- EMA teacher produces regression targets for latent step prediction
- K-step latent rollout via a lightweight stepper MLP
- Evaluated on answer generation (BLEU, ROUGE) and embedding retrieval (Recall@K)

**Results**

| Metric | K=4 | K=8 |
|:---|:---:|:---:|
| BLEU | — | 0.231 |
| ROUGE-1 | — | 0.594 |
| Recall@1 | 0.504 | — |

> K=0 yields zero scores across all metrics — confirming latent steps perform real reasoning work, not decorative computation.

**Artifacts**

[![Model Checkpoint](https://img.shields.io/badge/Checkpoint%20(1.55%20GB)-rajat5039%2Fthink--in--silence-FFD21E?style=flat-square&logo=huggingface&logoColor=black)](https://huggingface.co/rajat5039/think-in-silence)
[![Dataset](https://img.shields.io/badge/Dataset%20(504K%20pairs)-rajatmalik%2Fwiki--multihop--qa--500k-FFD21E?style=flat-square&logo=huggingface&logoColor=black)](https://huggingface.co/datasets/rajatmalik/wiki-multihop-qa-500k)
[![Repo](https://img.shields.io/badge/Repository-think--in--silence-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/Rajat25022005/think-in-silence)

---

## Engineering Projects

<details>
<summary><b>Visual Deep Research</b> — Multimodal Autonomous Research Engine &nbsp;<img src="https://img.shields.io/badge/status-in%20progress-58e6b0?style=flat-square" /></summary>

<br />

An extension of text-only deep research that processes images — charts, paper figures, diagrams — as first-class inputs alongside text. Vision understanding fuses into a shared knowledge graph, enabling cross-modal retrieval and synthesis.

- CNN/ViT for visual feature extraction; Tesseract OCR for embedded text
- LLaVA-based VQA for figure-level question answering
- Neo4j knowledge graph with typed edges spanning both modalities
- LangGraph orchestration; ChromaDB for cross-modal RAG

**Stack:** Python · LangGraph · LLaVA · Neo4j · ChromaDB · Tesseract

[![Repo](https://img.shields.io/badge/Repository-Visual--Deep--Research-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/Rajat25022005/Visual-Deep-Research)

</details>

<details>
<summary><b>CodeMind</b> — Temporal Knowledge Graph over Git History</summary>

<br />

A local-first developer tool that ingests a repository's full commit history and constructs a temporal knowledge graph over architectural decisions, code evolution, and module relationships. Enables natural-language queries like "why was this module refactored?" backed by structured retrieval.

**Stack:** Python · Neo4j · Qdrant · Ollama · Docker · Nginx

[![Repo](https://img.shields.io/badge/Repository-CodeMind-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/Rajat25022005/CodeMind)

</details>

<details>
<summary><b>Argus-V</b> — Spatio-Temporal Video Reasoning with Causal Graphs</summary>

<br />

A research system for extracting events, actors, and causal structure from video. Models temporal continuity and entity relationships rather than treating frames as independent. The resulting causal graph supports queryable long-term memory via GraphRAG.

**Stack:** Python · V-JEPA · Neo4j · GraphRAG · DeepFace

[![Repo](https://img.shields.io/badge/Repository-argus--V--graph--reasoning-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/Rajat25022005/argus-V-graph-reasoning)

</details>

<details>
<summary><b>Nexus Workplace AI</b> — Persistent Memory for Human–AI Collaboration</summary>

<br />

An agent-augmented collaboration platform exploring how LLMs maintain long-term shared context within team environments. Focuses on workspace-level semantic memory, cross-lingual embedding alignment, and real-time human–agent interaction.

**Stack:** React · Node.js · FastAPI · Socket.IO · Azure · Vector Search

[![Repo](https://img.shields.io/badge/Repository-Nexus--chat-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/Rajat25022005/Nexus-chat)

</details>

<details>
<summary><b>Multi-Agent Task Orchestrator</b> — Autonomous Planning, Execution, and Repair</summary>

<br />

Investigates how complex objectives can be decomposed and solved by specialized cooperating agents. Separates planning, execution, and validation — enabling autonomous error detection and iterative repair without human re-prompting.

**Stack:** Python · Ollama · LangChain

[![Repo](https://img.shields.io/badge/Repository-Multiagents-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/Rajat25022005/Multiagents)

</details>

---

## Technical Stack

<div align="center">

| Layer | Tools |
|:---|:---|
| **Languages** | Python · JavaScript · C++ · SQL |
| **ML / AI** | PyTorch · Hugging Face · LangChain · LangGraph · Ollama |
| **Memory & Retrieval** | Neo4j · ChromaDB · Qdrant · GraphRAG |
| **Infrastructure** | Docker · FastAPI · Azure · React · Linux · Git |

</div>

---

## Current Research Focus

```
01  Silent latent reasoning — structured multi-step inference without surfaced tokens
02  Spatio-temporal abstraction in video world models
03  Graph-based long-term memory for autonomous agents
04  Reliability, evaluation, and failure modes in multi-agent systems
05  Offline-first and privacy-preserving AI system design
```

---


---

## Credentials

![TensorFlow](https://img.shields.io/badge/TensorFlow%202.0-Udemy-A435F0?style=flat-square&logo=udemy&logoColor=white)
![Azure AI](https://img.shields.io/badge/AI%20Fundamentals%20AI--900-Microsoft-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![GenAI](https://img.shields.io/badge/Generative%20AI%20Series-LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)

---

<div align="center">

*Open to applied research roles, AI engineering internships, and collaborative research projects.*

</div>
