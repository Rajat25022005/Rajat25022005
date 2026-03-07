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

###  think-in-silence
**Latent Chain-of-Thought Reasoning — No Tokens, No RL, No CoT Labels**

Most models think out loud. This one doesn't.

think-in-silence implements **LC-Thought**: a reasoning architecture where the entire chain of thought exists only as latent vectors — never decoded to tokens. A recurrent cross-attention **ThoughtModule** runs K steps, each refining an internal thought vector by attending to the question context. Training uses a JEPA-style MSE objective against an EMA teacher encoder.

```
Question → Encoder (frozen) → ThoughtModule (K steps) → Predictor → pred
                                h₀ → h₁ → h₂ → ... → hₖ                     MSE ↕
Answer  → EMA Teacher Encoder ─────────────────────────────────────────► target
```

**What makes it different from Coconut / Quiet-STaR:**
- Dedicated reasoning module — backbone stays frozen
- Pure JEPA MSE training signal — no RL, no token supervision  
- K is a runtime parameter — more think time at inference, no retraining

**Trained on:** GSM8K · HotpotQA · CommonsenseQA · ARC-Challenge · StrategyQA  
**Key experiment:** Same checkpoint evaluated at K=1,2,4,8,16 — "think time = performance" curve

**Stack:** PyTorch · HuggingFace Transformers · Streaming QA datasets

🔗 [github.com/Rajat25022005/think-in-silence](https://github.com/Rajat25022005/think-in-silence)

---

###  T-JEPA
**Text Joint Embedding Predictive Architecture — Self-Supervised Semantic Learning**

A text adaptation of Meta's I-JEPA. Instead of predicting masked tokens, T-JEPA predicts **masked span representations in latent space** — forcing the model to learn semantics, not surface patterns.

```
Masked text → Student Encoder → Predictor → pred ∈ ℝ²⁵⁶
Clean text  → EMA Teacher   ─────────────────────► target
                               MSE in latent space
```

**Results vs DistilBERT** (trained on 30× less data):

| Metric | T-JEPA | DistilBERT |
|--------|--------|-----------|
| Masked Reconstruction Quality | **89.8%** ★ | −19.0% |
| Semantic Gap (MRPC) | **0.084** ★ | 0.014 |
| Recall@1 | 0.562 | **0.841** ★ |
| 5-Shot Accuracy | 0.433 | **0.745** ★ |

T-JEPA wins decisively on JEPA-specific metrics. DistilBERT wins classification — explained entirely by the 30× data gap, not the objective. Currently training on the full BookCorpus + Wikipedia corpus (16 GB, same as DistilBERT) using streaming mode.

**Stack:** PyTorch · DistilBERT · WikiText-103 → BookCorpus + Wikipedia · NVIDIA L4

 [github.com/Rajat25022005/self-supervised-text-jepa](https://github.com/Rajat25022005/self-supervised-text-jepa)

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

**ML & Research**  
Self-Supervised Learning · JEPA Objectives · EMA Teachers · Representation Learning  
Latent-Space Reasoning · Agentic Systems · GraphRAG · Knowledge Graphs  
Spatio-Temporal Modelling · Computer Vision · LLM Systems

**Engineering**  
Python · PyTorch · HuggingFace · JavaScript · SQL · C++  
Docker · Linux · Azure · Git · Ollama · Full-Stack Web

---

## GitHub

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=Rajat25022005&show_icons=true&hide_border=true&theme=tokyonight" />
  <img height="165" src="https://github-readme-streak-stats.herokuapp.com/?user=Rajat25022005&hide_border=true&theme=tokyonight" />
</p>

---

<div align="center">
  <sub>
    Open to applied research roles, AI engineering internships, and collaborative research.  
    Most interested in self-supervised learning, reasoning systems, and latent-space objectives.
  </sub>
</div>
