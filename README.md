<div align="center">

# Rajat Malik
**AI / ML Engineer · Self-Supervised Learning · Reasoning Systems**

[LinkedIn](https://linkedin.com/in/rajat-malik-a62876278) ·
[Email](mailto:rajatmalik5039@gmail.com) ·
[GitHub](https://github.com/Rajat25022005)

<img src="https://komarev.com/ghpvc/?username=Rajat25022005&style=flat&color=blueviolet" />

<br/>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=22&pause=1200&color=6AE3FF&center=true&vCenter=true&width=820&lines=Latent+Chain-of-Thought+Reasoning;Self-Supervised+Text+Representation+(JEPA);Spatio-Temporal+Reasoning+in+Video;Agentic+Systems+and+Autonomous+Planning" />

</div>

---

## About

B.E. Computer Science (AI & ML), Chandigarh University · Python Developer Intern, EDSHODH

I build **research-grade AI systems** at the intersection of **self-supervised learning**, **latent-space reasoning**, and **autonomous intelligence**. My work focuses on teaching models to reason and represent meaning without relying on expensive supervision — no labels, no RL, no chain-of-thought annotations.

Current focus: **JEPA-family objectives for language and reasoning** — predicting structure in latent space rather than reconstructing tokens.

---

## Research Projects

---

### [think-in-silence](https://github.com/Rajat25022005/think-in-silence) — Latent Reasoning Without Chain-of-Thought
 
> A model that reasons in pure embedding space. No tokens. No CoT labels. No RL.
 
K learned thought vectors run through a recurrent cross-attention chain before any answer is produced. Trained only on `(question, answer)` pairs via a JEPA MSE objective with an EMA teacher. The backbone is fully frozen — all reasoning happens in a dedicated 17M-parameter ThoughtModule.
 
**Empirical results (same checkpoint, varying K at inference):**
 
| K steps | R@1 | BLEU | ROUGE-1 |
|:-------:|:---:|:----:|:-------:|
| 0 (none) | 0.20% | 0.000 | 0.000 |
| 4 | **50.4%** | 0.044 | 0.218 |
| 8 | 47.5% | **0.231** | **0.594** |
 
K = 0 produces zero scores — the ThoughtModule does real work, not memorisation.
K is adjustable at inference with no retraining.
 
**Model weights:** [`rajat5039/think-in-silence`](https://huggingface.co/rajat5039/think-in-silence) · **Dataset:** [`rajatmalik/wiki-multihop-qa-500k`](https://huggingface.co/datasets/rajatmalik/wiki-multihop-qa-500k) (504K pairs)
 
---

###  Argus-V
**Spatio-Temporal Video Reasoning with Causal Graphs**

Argus-V extracts **events, actors, and causal structure** from video — modelling temporal continuity, physical intuition, and entity relationships rather than treating frames independently.

- Self-supervised video representation (V-JEPA)
- Event abstraction and temporal segmentation
- Causal graph construction over actors and actions
- Queryable long-term memory via GraphRAG + Neo4j

**Stack:** Python · V-JEPA · Neo4j · GraphRAG · DeepFace

 [github.com/Rajat25022005/argus-V-graph-reasoning](https://github.com/Rajat25022005/argus-V-graph-reasoning)

---

###  Nexus Workplace AI
**Persistent Memory for Human–AI Collaboration**

Agent-augmented collaboration platform exploring how LLMs can maintain **long-term, shared context** within a team. Focus on workspace-level semantic memory, cross-lingual embedding alignment, and real-time human–agent interaction.

**Stack:** React · Node.js · Socket.IO · Azure · Vector Search

 [github.com/Rajat25022005/Nexus-chat](https://github.com/Rajat25022005/Nexus-chat)

---

###  Multi-Agent Task Orchestrator
**Autonomous Planning, Execution, and Repair**

Investigates how complex objectives can be decomposed and solved via specialised cooperating agents — separating planning, execution, and validation to enable self-correction and iterative refinement.

**Stack:** Python · Ollama · LangChain

 [github.com/Rajat25022005/Multiagents](https://github.com/Rajat25022005/Multiagents)

----

## Technical Stack
 
**Languages**
 
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
 
**ML / AI**
 
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![HuggingFace](https://img.shields.io/badge/🤗_Transformers-FFD21E?style=flat-square)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square)
 
**Data / Retrieval**
 
![Neo4j](https://img.shields.io/badge/Neo4j-008CC1?style=flat-square&logo=neo4j&logoColor=white)
![Qdrant](https://img.shields.io/badge/Qdrant-DC244C?style=flat-square)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![ChromaDB](https://img.shields.io/badge/ChromaDB-orange?style=flat-square)
 
**Backend / Infra**
 
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GCP](https://img.shields.io/badge/GCP-4285F4?style=flat-square&logo=googlecloud&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
 
---
---
 
