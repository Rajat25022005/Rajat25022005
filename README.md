<div align="center">

<h1>Rajat Malik</h1>

<p><b>AI / ML Engineer &nbsp;&mdash;&nbsp; Representation Learning &nbsp;&middot;&nbsp; Reasoning Systems &nbsp;&middot;&nbsp; Autonomous Intelligence</b></p>

<a href="https://linkedin.com/in/rajat-malik-a62876278">
  <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
</a>
&nbsp;
<a href="https://huggingface.co/rajat5039">
  <img src="https://img.shields.io/badge/Hugging%20Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black" alt="HuggingFace" />
</a>
&nbsp;
<a href="mailto:rajatmalik5039@gmail.com">
  <img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
</a>

<br /><br />

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&pause=1200&color=6AE3FF&center=true&vCenter=true&width=720&lines=Latent+Reasoning+in+Silence;Graph-Based+Memory+and+Retrieval;Agentic+Systems+and+Autonomous+Planning;From+Research+Models+to+Production+Systems)](https://git.io/typing-svg)

<img src="https://komarev.com/ghpvc/?username=Rajat25022005&style=flat-square&color=blueviolet" alt="Profile views" />

</div>

---

## About

B.E. Computer Science (AI & ML), Chandigarh University &nbsp;&middot;&nbsp; Python Developer Intern, EDSHODH LLP

I build AI systems at the intersection of **representation learning**, **structured reasoning**, and **systems engineering**. My work focuses on enabling models to move beyond surface-level pattern matching toward memory-grounded, causally-aware, and long-horizon reasoning.

Recurring themes: learning over time and structure, explicit memory via graphs and retrieval, multi-agent decomposition of complex tasks, and translating research into deployable systems.

---

## Technical Stack

<div align="center">

<b>Languages</b><br />
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" />
<img src="https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white" />
<img src="https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white" />

<br /><br />

<b>Machine Learning & AI</b><br />
<img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" />
<img src="https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black" />
<img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white" />
<img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white" />
<img src="https://img.shields.io/badge/Ollama-000000?style=flat-square&logo=ollama&logoColor=white" />

<br /><br />

<b>Memory & Retrieval</b><br />
<img src="https://img.shields.io/badge/Neo4j-008CC1?style=flat-square&logo=neo4j&logoColor=white" />
<img src="https://img.shields.io/badge/ChromaDB-FF6F00?style=flat-square&logo=databricks&logoColor=white" />
<img src="https://img.shields.io/badge/Qdrant-DC244C?style=flat-square&logo=qdrant&logoColor=white" />

<br /><br />

<b>Infrastructure</b><br />
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
<img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" />
<img src="https://img.shields.io/badge/Azure-0078D4?style=flat-square&logo=microsoftazure&logoColor=white" />
<img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" />
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" />
<img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black" />

</div>

---

## Research and Engineering

### think-in-silence &nbsp; [![HuggingFace](https://img.shields.io/badge/model-published-FFD21E?style=flat-square&logo=huggingface&logoColor=black)](https://huggingface.co/rajat5039/think-in-silence)

**Latent Reasoning Without Chain-of-Thought**

A latent reasoning architecture that performs silent K-step reasoning entirely in a 256-dimensional vector space. No chain-of-thought tokens. No RL. Trained with a JEPA objective and an EMA teacher on 504K synthetic multi-hop QA pairs.

**Architecture**
- Backbone: Gemma-3-4B-it with 4-bit NF4 quantization — frozen in Stage 1&ndash;2, partially unfrozen in Stage 3
- EMA teacher produces regression targets for latent step prediction
- K-step latent rollout via a lightweight stepper MLP
- Evaluated on answer generation (BLEU, ROUGE) and embedding retrieval (Recall@K)

**Results**

| Metric | K=4 | K=8 |
|:---|:---:|:---:|
| BLEU | &mdash; | 0.231 |
| ROUGE-1 | &mdash; | 0.594 |
| R@1 | 0.504 | &mdash; |

K=0 produces zero scores across all metrics, confirming the latent steps perform real reasoning work.

**Published artifacts**

<a href="https://huggingface.co/rajat5039/think-in-silence">
  <img src="https://img.shields.io/badge/Model%20Checkpoint%20(1.55%20GB)-rajat5039%2Fthink--in--silence-FFD21E?style=flat-square&logo=huggingface&logoColor=black" />
</a>
<br />
<a href="https://huggingface.co/datasets/rajatmalik/wiki-multihop-qa-500k">
  <img src="https://img.shields.io/badge/Dataset%20(504K%20pairs)-rajatmalik%2Fwiki--multihop--qa--500k-FFD21E?style=flat-square&logo=huggingface&logoColor=black" />
</a>
<br />
<a href="https://github.com/Rajat25022005/think-in-silence">
  <img src="https://img.shields.io/badge/Repository-think--in--silence-181717?style=flat-square&logo=github&logoColor=white" />
</a>

---

<details>
<summary><b>Visual Deep Research</b> &nbsp;&mdash;&nbsp; Multimodal Autonomous Research Engine &nbsp;<img src="https://img.shields.io/badge/status-in%20progress-orange?style=flat-square" /></summary>

<br />

An extension of text-only deep research tools that processes images — charts, paper figures, diagrams — as first-class inputs alongside text. Vision understanding is fused into a shared knowledge graph, enabling cross-modal retrieval and synthesis.

**Architecture**
- CNN/ViT for visual feature extraction; Tesseract OCR for embedded text
- LLaVA-based VQA for figure-level question answering
- Neo4j knowledge graph with typed edges spanning both modalities
- LangGraph orchestration; ChromaDB for cross-modal RAG

**Stack** &nbsp;&mdash;&nbsp; Python &middot; LangGraph &middot; LLaVA &middot; Neo4j &middot; ChromaDB &middot; Tesseract

<a href="https://github.com/Rajat25022005/Visual-Deep-Research">
  <img src="https://img.shields.io/badge/Repository-Visual--Deep--Research-181717?style=flat-square&logo=github&logoColor=white" />
</a>

<br />

</details>

<details>
<summary><b>CodeMind</b> &nbsp;&mdash;&nbsp; Temporal Knowledge Graph over Git History</summary>

<br />

A local-first developer tool that ingests a repository's full commit history and constructs a temporal knowledge graph over architectural decisions, code evolution, and module relationships. Enables natural-language queries like "why was this module refactored?" backed by structured retrieval.

**Stack** &nbsp;&mdash;&nbsp; Python &middot; Neo4j &middot; Qdrant &middot; Ollama &middot; Docker &middot; Nginx

<a href="https://github.com/Rajat25022005/CodeMind">
  <img src="https://img.shields.io/badge/Repository-CodeMind-181717?style=flat-square&logo=github&logoColor=white" />
</a>

<br />

</details>

<details>
<summary><b>Argus-V</b> &nbsp;&mdash;&nbsp; Spatio-Temporal Video Reasoning with Causal Graphs</summary>

<br />

A research system for extracting events, actors, and causal structure from video. Models temporal continuity and entity relationships rather than treating video as independent frames. The resulting causal graph supports queryable long-term memory via GraphRAG.

**Stack** &nbsp;&mdash;&nbsp; Python &middot; V-JEPA &middot; Neo4j &middot; GraphRAG &middot; DeepFace

<a href="https://github.com/Rajat25022005/argus-V-graph-reasoning">
  <img src="https://img.shields.io/badge/Repository-argus--V--graph--reasoning-181717?style=flat-square&logo=github&logoColor=white" />
</a>

<br />

</details>

<details>
<summary><b>Nexus Workplace AI</b> &nbsp;&mdash;&nbsp; Persistent Memory for Human&ndash;AI Collaboration</summary>

<br />

An agent-augmented collaboration platform exploring how LLMs can maintain long-term shared context within a team environment. Focuses on workspace-level semantic memory, cross-lingual embedding alignment, and real-time human&ndash;agent interaction.

**Stack** &nbsp;&mdash;&nbsp; React &middot; Node.js &middot; FastAPI &middot; Socket.IO &middot; Azure &middot; Vector Search

<a href="https://github.com/Rajat25022005/Nexus-chat">
  <img src="https://img.shields.io/badge/Repository-Nexus--chat-181717?style=flat-square&logo=github&logoColor=white" />
</a>

<br />

</details>

<details>
<summary><b>Multi-Agent Task Orchestrator</b> &nbsp;&mdash;&nbsp; Autonomous Planning, Execution, and Repair</summary>

<br />

Investigates how complex objectives can be decomposed and solved by specialized cooperating agents. Separates planning, execution, and validation, enabling autonomous error detection and iterative refinement without human re-prompting.

**Stack** &nbsp;&mdash;&nbsp; Python &middot; Ollama &middot; LangChain

<a href="https://github.com/Rajat25022005/Multiagents">
  <img src="https://img.shields.io/badge/Repository-Multiagents-181717?style=flat-square&logo=github&logoColor=white" />
</a>

<br />

</details>

---

## Current Research Focus

- Silent latent reasoning and the mechanics of structured multi-step inference
- Spatio-temporal abstraction in video world models
- Graph-based long-term memory for autonomous agents
- Reliability, evaluation, and failure modes in multi-agent systems
- Offline-first and privacy-preserving AI system design

---

## GitHub Activity

<div align="center">

<table>
  <tr>
    <td align="center">
      <img src="https://github-readme-stats.vercel.app/api?username=Rajat25022005&show_icons=true&hide_border=true&bg_color=00000000" alt="GitHub stats" />
    </td>
    <td align="center">
      <img src="https://github-readme-streak-stats.herokuapp.com/?user=Rajat25022005&hide_border=true&background=00000000" alt="GitHub streak" />
    </td>
  </tr>
</table>

</div>

---

## Credentials

<img src="https://img.shields.io/badge/TensorFlow%202.0-Udemy-A435F0?style=flat-square&logo=udemy&logoColor=white" />
&nbsp;
<img src="https://img.shields.io/badge/AI%20Fundamentals%20AI--900-Microsoft-0078D4?style=flat-square&logo=microsoftazure&logoColor=white" />
&nbsp;
<img src="https://img.shields.io/badge/Generative%20AI%20Series-LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" />

---

<div align="center">
<p>Open to applied research roles, AI engineering internships, and collaborative research projects.</p>
</div>
