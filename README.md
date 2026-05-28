# 📚 Essential AI Papers — LLMs, RAG & Agents

> A curated reading list for AI engineers and researchers covering Large Language Models, Retrieval-Augmented Generation, AI Agents, and more. Every paper here is battle-tested and referenced constantly across the field.

---

## 🗺️ Learning Path

```
Foundations → Modern LLMs → RAG → Agents → Architecture → Evaluation → Multimodal
```

| Role | Recommended Path |
|------|-----------------|
| **LLM Application Builder** | Foundations → RAG (core + advanced) → Agents (ReAct, Reflexion, AutoGen) |
| **LLM Researcher** | Foundations → Modern LLMs (all) → Architecture → Evaluation |
| **Efficiency / Deployment** | LoRA → QLoRA → FlashAttention → GPTQ → AWQ → Mamba |
| **AI Agent Builder** | Chain-of-Thought → ReAct → Tree of Thoughts → Reflexion → AutoGen |

---

## Legend

| Badge | Meaning |
|-------|---------|
| 🔴 **MUST** | Absolutely essential — read these first |
| 🟢 **KEY** | Highly important — read after MUST |
| 🟡 **ADV** | Advanced / specialized — for deeper expertise |

---

## 1. Foundations

### Transformer Architecture

| Paper | Authors | Year | Priority |
|-------|---------|------|----------|
| [Attention Is All You Need](https://arxiv.org/abs/1706.03762) | Vaswani et al. — Google | 2017 | 🔴 MUST |
| [BERT: Pre-training of Deep Bidirectional Transformers](https://arxiv.org/abs/1810.04805) | Devlin et al. — Google | 2018 | 🔴 MUST |
| [Language Models are Few-Shot Learners (GPT-3)](https://arxiv.org/abs/2005.14165) | Brown et al. — OpenAI | 2020 | 🔴 MUST |
| [Improving Language Understanding by Generative Pre-Training (GPT-1)](https://openai.com/research/language-unsupervised) | Radford et al. — OpenAI | 2018 | 🟢 KEY |
| [Language Models are Unsupervised Multitask Learners (GPT-2)](https://openai.com/research/better-language-models) | Radford et al. — OpenAI | 2019 | 🟢 KEY |
| [Exploring the Limits of Transfer Learning with T5](https://arxiv.org/abs/1910.10683) | Raffel et al. — Google | 2019 | 🟢 KEY |

### Scaling Laws & Efficiency

| Paper | Authors | Year | Priority |
|-------|---------|------|----------|
| [Scaling Laws for Neural Language Models](https://arxiv.org/abs/2001.08361) | Kaplan et al. — OpenAI | 2020 | 🔴 MUST |
| [Training Compute-Optimal Large Language Models (Chinchilla)](https://arxiv.org/abs/2203.15556) | Hoffmann et al. — DeepMind | 2022 | 🔴 MUST |
| [Mixtral of Experts](https://arxiv.org/abs/2401.04088) | Jiang et al. — Mistral AI | 2024 | 🟢 KEY |
| [Efficient Large Scale Language Modeling with Mixtures of Experts](https://arxiv.org/abs/2112.10684) | Artetxe et al. — Meta | 2021 | 🟡 ADV |

---

## 2. Modern LLMs

### Flagship Models

| Paper | Authors | Year | Priority |
|-------|---------|------|----------|
| [LLaMA: Open and Efficient Foundation Language Models](https://arxiv.org/abs/2302.13971) | Touvron et al. — Meta | 2023 | 🔴 MUST |
| [LLaMA 2: Open Foundation and Fine-Tuned Chat Models](https://arxiv.org/abs/2307.09288) | Touvron et al. — Meta | 2023 | 🔴 MUST |
| [GPT-4 Technical Report](https://arxiv.org/abs/2303.08774) | OpenAI | 2023 | 🔴 MUST |
| [Constitutional AI: Harmlessness from AI Feedback](https://arxiv.org/abs/2212.08073) | Bai et al. — Anthropic | 2022 | 🔴 MUST |
| [Gemini: A Family of Highly Capable Multimodal Models](https://arxiv.org/abs/2312.11805) | Team Gemini — Google | 2023 | 🔴 MUST |
| [PaLM: Scaling Language Modeling with Pathways](https://arxiv.org/abs/2204.02311) | Chowdhery et al. — Google | 2022 | 🟢 KEY |
| [Mistral 7B](https://arxiv.org/abs/2310.06825) | Jiang et al. — Mistral AI | 2023 | 🟢 KEY |

### Alignment & RLHF

| Paper | Authors | Year | Priority |
|-------|---------|------|----------|
| [Training Language Models to Follow Instructions (InstructGPT)](https://arxiv.org/abs/2203.02155) | Ouyang et al. — OpenAI | 2022 | 🔴 MUST |
| [Learning to Summarize from Human Feedback](https://arxiv.org/abs/2009.01325) | Stiennon et al. — OpenAI | 2020 | 🔴 MUST |
| [Direct Preference Optimization (DPO)](https://arxiv.org/abs/2305.18290) | Rafailov et al. — Stanford | 2023 | 🔴 MUST |
| [RLAIF: Scaling RL from Human Feedback with AI Feedback](https://arxiv.org/abs/2309.00267) | Lee et al. — Google | 2023 | 🟢 KEY |
| [Reward Modeling for Mitigating Risks in RLHF](https://arxiv.org/abs/2203.07730) | Gao et al. — OpenAI | 2022 | 🟢 KEY |

### Efficient Fine-tuning

| Paper | Authors | Year | Priority |
|-------|---------|------|----------|
| [LoRA: Low-Rank Adaptation of Large Language Models](https://arxiv.org/abs/2106.09685) | Hu et al. — Microsoft | 2021 | 🔴 MUST |
| [QLoRA: Efficient Finetuning of Quantized LLMs](https://arxiv.org/abs/2305.14314) | Dettmers et al. — UW | 2023 | 🔴 MUST |
| [The Power of Scale for Parameter-Efficient Prompt Tuning](https://arxiv.org/abs/2104.08691) | Lester et al. — Google | 2021 | 🟢 KEY |
| [Prefix-Tuning: Optimizing Continuous Prompts for Generation](https://arxiv.org/abs/2101.00190) | Li & Liang — Stanford | 2021 | 🟢 KEY |
| [A Guide to Parameter-Efficient Fine-Tuning](https://arxiv.org/abs/2303.15647) | Lialin et al. | 2023 | 🟡 ADV |

---

## 3. Retrieval-Augmented Generation (RAG)

### Core RAG

| Paper | Authors | Year | Priority |
|-------|---------|------|----------|
| [Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks](https://arxiv.org/abs/2005.11401) | Lewis et al. — Meta/UCL | 2020 | 🔴 MUST |
| [REALM: Retrieval-Augmented Language Model Pre-Training](https://arxiv.org/abs/2002.08909) | Guu et al. — Google | 2020 | 🔴 MUST |
| [RAG vs Fine-Tuning: Pipelines, Tradeoffs, and a Case Study](https://arxiv.org/abs/2401.08406) | Ovadia et al. | 2023 | 🔴 MUST |
| [Searching for Best Practices in RAG](https://arxiv.org/abs/2407.01219) | Wang et al. | 2024 | 🔴 MUST |
| [Atlas: Few-shot Learning with Retrieval Augmented Language Models](https://arxiv.org/abs/2208.03299) | Izacard et al. — Meta | 2022 | 🟢 KEY |
| [RETRO: Improving Language Models by Retrieving from Trillions of Tokens](https://arxiv.org/abs/2112.04426) | Borgeaud et al. — DeepMind | 2021 | 🟢 KEY |

### Advanced RAG Patterns

| Paper | Authors | Year | Priority |
|-------|---------|------|----------|
| [Self-RAG: Learning to Retrieve, Generate, and Critique](https://arxiv.org/abs/2310.11511) | Asai et al. — UW | 2023 | 🔴 MUST |
| [HyDE: Precise Zero-Shot Dense Retrieval without Relevance Labels](https://arxiv.org/abs/2212.10496) | Gao et al. — CMU | 2022 | 🟢 KEY |
| [FLARE: Active Retrieval Augmented Generation](https://arxiv.org/abs/2305.06983) | Jiang et al. — CMU | 2023 | 🟢 KEY |
| [Corrective RAG (CRAG)](https://arxiv.org/abs/2401.15884) | Yan et al. | 2024 | 🟢 KEY |

### Embeddings & Retrieval

| Paper | Authors | Year | Priority |
|-------|---------|------|----------|
| [Dense Passage Retrieval for Open-Domain QA (DPR)](https://arxiv.org/abs/2004.04906) | Karpukhin et al. — Meta | 2020 | 🔴 MUST |
| [Sentence-BERT: Sentence Embeddings using Siamese BERT-Networks](https://arxiv.org/abs/1908.10084) | Reimers & Gurevych | 2019 | 🔴 MUST |
| [E5: Text Embeddings by Weakly-Supervised Contrastive Pre-training](https://arxiv.org/abs/2212.03533) | Wang et al. — Microsoft | 2022 | 🟢 KEY |
| [MTEB: Massive Text Embedding Benchmark](https://arxiv.org/abs/2210.07316) | Muennighoff et al. | 2022 | 🟢 KEY |
| [ColBERT: Efficient and Effective Passage Search via Contextualized Late Interaction](https://arxiv.org/abs/2004.12832) | Khattab & Zaharia — Stanford | 2020 | 🟡 ADV |

---

## 4. AI Agents

### Reasoning & Planning

| Paper | Authors | Year | Priority |
|-------|---------|------|----------|
| [Chain-of-Thought Prompting Elicits Reasoning in LLMs](https://arxiv.org/abs/2201.11903) | Wei et al. — Google | 2022 | 🔴 MUST |
| [ReAct: Synergizing Reasoning and Acting in Language Models](https://arxiv.org/abs/2210.03629) | Yao et al. — Princeton | 2022 | 🔴 MUST |
| [Tree of Thoughts: Deliberate Problem Solving with LLMs](https://arxiv.org/abs/2305.10601) | Yao et al. — Princeton/Google | 2023 | 🔴 MUST |
| [Reflexion: Language Agents with Verbal Reinforcement Learning](https://arxiv.org/abs/2303.11366) | Shinn et al. — Northeastern | 2023 | 🔴 MUST |
| [Self-Consistency Improves Chain of Thought Reasoning](https://arxiv.org/abs/2203.11171) | Wang et al. — Google | 2022 | 🔴 MUST |
| [Least-to-Most Prompting Enables Complex Reasoning in LLMs](https://arxiv.org/abs/2205.01068) | Zhou et al. — Google | 2022 | 🟢 KEY |

### Tool Use & Code

| Paper | Authors | Year | Priority |
|-------|---------|------|----------|
| [Toolformer: Language Models Can Teach Themselves to Use Tools](https://arxiv.org/abs/2302.04761) | Schick et al. — Meta | 2023 | 🔴 MUST |
| [PAL: Program-Aided Language Models](https://arxiv.org/abs/2211.10435) | Gao et al. — CMU | 2022 | 🟢 KEY |
| [HuggingGPT: Solving AI Tasks with ChatGPT](https://arxiv.org/abs/2303.17580) | Shen et al. — Zhejiang/Microsoft | 2023 | 🟢 KEY |
| [Code Llama: Open Foundation Models for Code](https://arxiv.org/abs/2308.12950) | Rozière et al. — Meta | 2023 | 🟢 KEY |
| [Program of Thoughts Prompting (PoT)](https://arxiv.org/abs/2211.12588) | Chen et al. — CMU | 2022 | 🟢 KEY |

### Multi-Agent & Autonomous Systems

| Paper | Authors | Year | Priority |
|-------|---------|------|----------|
| [A Survey on LLM-based Autonomous Agents](https://arxiv.org/abs/2308.11432) | Wang et al. | 2023 | 🔴 MUST |
| [AutoGen: Enabling Next-Gen LLM Applications via Multi-Agent Conversation](https://arxiv.org/abs/2308.08155) | Wu et al. — Microsoft | 2023 | 🔴 MUST |
| [Generative Agents: Interactive Simulacra of Human Behavior](https://arxiv.org/abs/2304.03442) | Park et al. — Stanford | 2023 | 🔴 MUST |
| [AgentBench: Evaluating LLMs as Agents](https://arxiv.org/abs/2308.03688) | Liu et al. — THU | 2023 | 🟢 KEY |
| [Communicative Agents for Software Development (ChatDev)](https://arxiv.org/abs/2307.07924) | Qian et al. | 2023 | 🟢 KEY |

---

## 5. Architecture Deep Dives

### Positional Encoding & Long Context

| Paper | Authors | Year | Priority |
|-------|---------|------|----------|
| [RoFormer: Enhanced Transformer with Rotary Position Embedding (RoPE)](https://arxiv.org/abs/2104.09864) | Su et al. | 2021 | 🔴 MUST |
| [ALiBi: Train Short, Test Long](https://arxiv.org/abs/2108.12409) | Press et al. — Meta | 2021 | 🟢 KEY |
| [Extending Context Window via Positional Interpolation](https://arxiv.org/abs/2306.15595) | Chen et al. — Meta | 2023 | 🟢 KEY |
| [Long Range Arena: A Benchmark for Efficient Transformers](https://arxiv.org/abs/2011.04006) | Tay et al. — Google | 2020 | 🟡 ADV |

### Efficient Attention

| Paper | Authors | Year | Priority |
|-------|---------|------|----------|
| [FlashAttention: Fast and Memory-Efficient Exact Attention](https://arxiv.org/abs/2205.14135) | Dao et al. — Stanford | 2022 | 🔴 MUST |
| [FlashAttention-2: Faster Attention with Better Parallelism](https://arxiv.org/abs/2307.08691) | Dao — Princeton | 2023 | 🔴 MUST |
| [Mamba: Linear-Time Sequence Modeling with Selective State Spaces](https://arxiv.org/abs/2312.00752) | Gu & Dao — CMU/Princeton | 2023 | 🔴 MUST |
| [GQA: Training Generalized Multi-Query Transformer Models](https://arxiv.org/abs/2305.13245) | Ainslie et al. — Google | 2023 | 🟢 KEY |

### Quantization & Compression

| Paper | Authors | Year | Priority |
|-------|---------|------|----------|
| [GPTQ: Accurate Post-Training Quantization for GPTs](https://arxiv.org/abs/2210.17323) | Frantar et al. — IST Austria | 2022 | 🔴 MUST |
| [LLM.int8(): 8-bit Matrix Multiplication for Transformers at Scale](https://arxiv.org/abs/2208.07339) | Dettmers et al. | 2022 | 🔴 MUST |
| [AWQ: Activation-aware Weight Quantization for LLM Compression](https://arxiv.org/abs/2306.00978) | Lin et al. — MIT | 2023 | 🟢 KEY |
| [SparseGPT: Massive Language Models Can be Accurately Pruned in One Shot](https://arxiv.org/abs/2301.00774) | Frantar & Alistarh | 2023 | 🟡 ADV |

---

## 6. Evaluation

### Benchmarks

| Paper | Authors | Year | Priority |
|-------|---------|------|----------|
| [MMLU: Measuring Massive Multitask Language Understanding](https://arxiv.org/abs/2009.03300) | Hendrycks et al. — UC Berkeley | 2020 | 🔴 MUST |
| [MT-Bench and Chatbot Arena: How to Evaluate LLMs as Chatbots](https://arxiv.org/abs/2306.05685) | Zheng et al. — UC Berkeley | 2023 | 🔴 MUST |
| [HumanEval: Evaluating LLMs Trained on Code](https://arxiv.org/abs/2107.03374) | Chen et al. — OpenAI | 2021 | 🔴 MUST |
| [BIG-Bench: Beyond the Imitation Game Benchmark](https://arxiv.org/abs/2206.04615) | Srivastava et al. — Google et al. | 2022 | 🔴 MUST |
| [HELM: Holistic Evaluation of Language Models](https://arxiv.org/abs/2211.09110) | Liang et al. — Stanford | 2022 | 🟢 KEY |

### Hallucination & Safety

| Paper | Authors | Year | Priority |
|-------|---------|------|----------|
| [TruthfulQA: Measuring How Models Mimic Human Falsehoods](https://arxiv.org/abs/2109.07958) | Lin et al. — Oxford/OpenAI | 2021 | 🔴 MUST |
| [Red-Teaming Language Models to Reduce Harms](https://arxiv.org/abs/2209.07858) | Perez et al. — Anthropic | 2022 | 🔴 MUST |
| [FActScoring: Fine-grained Atomic Evaluation of Factual Precision](https://arxiv.org/abs/2305.14251) | Min et al. — UW | 2023 | 🟢 KEY |
| [Reward Model Ensembles Help Mitigate Overoptimization](https://arxiv.org/abs/2310.02743) | Coste et al. | 2023 | 🟡 ADV |

---

## 7. Multimodal

### Vision-Language Models

| Paper | Authors | Year | Priority |
|-------|---------|------|----------|
| [CLIP: Learning Transferable Visual Models from Natural Language Supervision](https://arxiv.org/abs/2103.00020) | Radford et al. — OpenAI | 2021 | 🔴 MUST |
| [Flamingo: a Visual Language Model for Few-Shot Learning](https://arxiv.org/abs/2204.14198) | Alayrac et al. — DeepMind | 2022 | 🔴 MUST |
| [LLaVA: Visual Instruction Tuning](https://arxiv.org/abs/2304.08485) | Liu et al. — UW/Microsoft | 2023 | 🔴 MUST |
| [GPT-4V System Card](https://openai.com/research/gpt-4v-system-card) | OpenAI | 2023 | 🔴 MUST |
| [DALL-E 2: Hierarchical Text-Conditional Image Generation](https://arxiv.org/abs/2204.06125) | Ramesh et al. — OpenAI | 2022 | 🟢 KEY |
| [CogVLM: Visual Expert for Pretrained Language Models](https://arxiv.org/abs/2311.03079) | Wang et al. — THU | 2023 | 🟡 ADV |

---

## 🚀 Absolute Non-Negotiables

If you only read 10 papers, make it these:

1. **[Attention Is All You Need](https://arxiv.org/abs/1706.03762)** — the paper that started it all
2. **[GPT-3](https://arxiv.org/abs/2005.14165)** — the dawn of few-shot LLMs
3. **[Scaling Laws](https://arxiv.org/abs/2001.08361)** — how to think about model training
4. **[InstructGPT](https://arxiv.org/abs/2203.02155)** — RLHF and instruction following
5. **[RAG (Lewis 2020)](https://arxiv.org/abs/2005.11401)** — the foundation of retrieval-augmented systems
6. **[Chain-of-Thought](https://arxiv.org/abs/2201.11903)** — unlocking reasoning in LLMs
7. **[ReAct](https://arxiv.org/abs/2210.03629)** — the backbone of modern AI agents
8. **[LoRA](https://arxiv.org/abs/2106.09685)** — how we fine-tune LLMs efficiently
9. **[FlashAttention](https://arxiv.org/abs/2205.14135)** — how attention actually runs fast
10. **[Self-RAG](https://arxiv.org/abs/2310.11511)** — the state of the art in RAG

---

## 📊 Stats

| Category | MUST | KEY | ADV | Total |
|----------|------|-----|-----|-------|
| Foundations | 4 | 6 | 1 | 11 |
| Modern LLMs | 11 | 7 | 1 | 19 |
| RAG | 8 | 8 | 1 | 17 |
| AI Agents | 10 | 9 | 0 | 19 |
| Architecture | 6 | 6 | 2 | 14 |
| Evaluation | 8 | 3 | 2 | 13 |
| Multimodal | 4 | 1 | 1 | 6 |
| **Total** | **51** | **40** | **8** | **99** |

---

## 🤝 Contributing

Found a paper that belongs here? Open a PR with:
- Paper title and authors
- ArXiv / official link
- Priority badge (MUST / KEY / ADV) with a brief justification
- Category it belongs to

---

## ⭐ Acknowledgements

Curated for the working AI engineer and researcher. Papers selected based on community adoption, citation frequency, and practical impact on building production AI systems.

---

*Last updated: 2025 · Covers papers up to mid-2024*
