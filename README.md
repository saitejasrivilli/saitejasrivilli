<div align="center">

# 👋 Hi, I'm Sai Teja Srivillibhutturu

### LLM Post-Training Engineer | RLHF · GRPO · Agent RL | GPU Systems

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/saitejasrivilli)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/saitejasrivilli)
[![Google Scholar](https://img.shields.io/badge/Google_Scholar-4285F4?style=for-the-badge&logo=google-scholar&logoColor=white)](https://scholar.google.com/citations?user=StKZohYAAAAJ)
[![Portfolio](https://img.shields.io/badge/Portfolio-FF5722?style=for-the-badge&logo=google-chrome&logoColor=white)](https://saitejasrivillibhutturu.github.io)

</div>

---

## 🎯 Professional Summary

**LLM Post-Training Engineer** focused on the full alignment pipeline: SFT → DPO → GRPO → Agent RL with verifiable rewards. Building on 4× NVIDIA A30 at UT Arlington and shipping clinical AI at Qure.ai.

**Post-Training work (all benchmarked on real hardware):**
- **Agent GRPO on GSM8K** — best reward 0.5575 over 200 iterations; policy learns to call a Python executor tool and condition on tool results before producing `<final_answer>`
- **PRM (Process Reward Model)** — step-level rewards (γ=0.9) achieve best reward 1.0659; step signal contributes 15% of gradient even on wrong-answer rollouts
- **SFT → DPO → RLVR pipeline** — BERTScore 0.780 → 0.855 (+9.6%), DPO margin +0.137, RLVR best reward 0.8189
- **vLLM vs HF inference** — 1.24–1.32× real throughput gain, 10–18% TTFT reduction (measured, not estimated)
- **Quantization** — NF4 reduces Qwen2.5-7B VRAM from 15.25 GB → 5.83 GB (−61.8%) at only 16% throughput loss

Published IEEE research on LLM-based path planning (OJCOMS 2026, ICC 2026).

---

## 💼 Professional Experience

### **AI Solutions Engineer Intern** @ Qure.ai
📍 *Arlington, TX | Mar 2026 – Present*

- **Clinical Protocol Automation:** Leading LLM configuration for hospital clients (Mount Sinai, Medstar) to automate clinical workflows using proprietary clinical knowledge
- **Healthcare Interoperability:** Building EPIC/FHIR integrations to enable real-time protocol recommendations directly in hospital systems
- **Infrastructure Redesign:** Architecting pluggable executor framework for clinical pipeline orchestration—Docker-first, API-driven design with portable artifact store across environments

**Tech Stack:** Python, FastAPI, Docker, Kubernetes, FHIR, Healthcare APIs

---

### **Graduate Research Assistant – TopGPT Project** @ UT Arlington
📍 *Arlington, TX | Jun 2025 – Present*

- **Full-Stack LLM/RAG Platform:** Building enterprise-grade retrieval-augmented generation system for knowledge workers
- **GPU Infrastructure:** Leveraging 4× NVIDIA A30 cluster (96GB total VRAM) for multi-GPU DDP training and inference optimization
- **Research & Development:** Experimenting with advanced RAG patterns, prompt optimization, and efficient fine-tuning techniques

**Tech Stack:** PyTorch, CUDA, vLLM, Vector Databases, LangChain

---

### **ML Engineer (Contract)** @ DentalScan / ReplyQuickAI
📍 *Remote | Dec 2025 – Feb 2026*

- **Computer Vision Pipeline:** Developed CNN-based dental image analysis system with automated defect detection
- **Cloud Deployment:** End-to-end pipeline from model training to production on AWS (S3, EC2, SageMaker)
- **Experiment Tracking:** Integrated MLflow for reproducible model versioning and metric comparison

**Tech Stack:** PyTorch, TensorFlow, AWS (S3, EC2, SageMaker), MLflow, OpenCV

---

### **Software Engineer (4 yrs)** @ Tata Consultancy Services
📍 *India | Jun 2019 – May 2023*

- Built scalable Java-based backend systems for financial services domain
- Designed distributed system architectures and optimized database performance
- Led API design and microservices migration initiatives

---

## 📚 Publications & Research

### **DTMAP: Digital Twin-Guided AI Path Planning for Connectivity-Aware Mobility**
**IEEE Open Journal of the Communications Society (OJCOMS) | Accepted April 2026**

Multi-objective path planning framework integrating wireless digital twins with a fine-tuned LLM for connectivity-aware navigation in 6G/XR environments. Achieves 1.9% outage probability vs. 2.3% for RL, 312 ms avg. inference latency, outperforms A*, greedy, Q-learning, LLaMA 3.1/3.3-70B, and Qwen-2.5-72B.

- **Tunable α parameter** trades off signal strength vs. travel distance across 21 values without retraining
- **GPT-4o-mini fine-tuned** on instruction-conditioned routing data via DT-grounded oracle supervision
- **Deterministic sanitization pipeline** brings raw LLM path validity from 65% → 100%
- **Tech stack:** GPT-4o-mini (OpenAI Fine-tuning API), NVIDIA Sionna (ray tracing), OpenStreetMap, Blender, Python, PyTorch

---

### **CTMap: LLM-Enabled Connectivity-Aware Path Planning in mmWave Digital Twin Networks**
**IEEE ICC 2026 (CQRM) | arXiv:2601.00110**

Designed an LLM-driven approach to network path optimization for next-generation 6G networks, achieving:
- **Connectivity-aware routing** in mmWave networks using digital twin simulation
- **Practical deployment** on edge devices with on-device inference

[📖 Read on arXiv](https://arxiv.org/abs/2601.00110) | [💻 View Research Code](https://github.com/saitejasrivilli)

This work bridges the gap between LLM reasoning capabilities and systems-level network optimization—proving that transformer-based models can effectively solve constrained optimization problems in telecommunications.

---

## 🌐 Live Deployments & Interactive Demos

Experience my work in action. All demos are production-ready and actively maintained:

| Project | Platform | Description | Status |
|---------|----------|-------------|--------|
| **🤖 Multi-Strategy AI Agent System** | [🤗 Hugging Face Spaces](https://huggingface.co/spaces/SaiTejaSrivilli/ai-agent-system) | 4 reasoning strategies (CoT, ToT, ReAct, Multi-Agent) with intelligent routing | ✅ Live |
| **🔍 Glean-Lite: Enterprise RAG** | [Vercel](https://glean-lite.vercel.app) | Go-based RAG engine with semantic search and document ingestion | ✅ Production |
| **⚡ Edge LLM Benchmark** | [Vercel](https://edge-llm-benchmark.vercel.app) | Real-time LLM benchmarks on MacBook Air M2 using MLX framework | ✅ Interactive |
| **🌊 Maxwell PINN Solver** | [Streamlit Demo](https://maxwell-pinn-solver.streamlit.app) | Physics-informed neural network solving Maxwell's equations (1700× COMSOL speedup) | ✅ Live |

**Try them out:** Click any link above to see ML/AI in action. No signup required.

---

## 🚀 Featured Projects

### 🧠 LLM Post-Training Pipeline — SFT → DPO → GRPO → Agent RL

End-to-end implementation of modern LLM alignment techniques on Qwen2.5-7B-Instruct across 4× NVIDIA A30 GPUs. All numbers are measured on real hardware.

| Repository | Method | Key Result |
|-----------|--------|-----------|
| [**rlhf-synthesis-optimization**](https://github.com/saitejasrivilli/rlhf-synthesis-optimization) | PPO · DPO · GRPO · Agent GRPO · PRM · RLAIF · STaR | Agent GRPO best reward **0.5575** (200 iters); PRM best **1.0659**; LLM-PPO **0.9007** |
| [**LLM_FineTuning_SFT_Production**](https://github.com/saitejasrivilli/LLM_FineTuning_SFT_Production) | SFT → DPO → RLVR | BERTScore **0.780 → 0.855**; DPO margin **+0.137**; RLVR best reward **0.8189** |
| [**efficient-post-training-suite**](https://github.com/saitejasrivilli/efficient-post-training-suite) | Full 6-stage pipeline + SLURM configs | SFT → DPO → GRPO → Agent → Eval on A30 cluster |
| [**code-agent-eval-benchmark**](https://github.com/saitejasrivilli/code-agent-eval-benchmark) | GSM8K · HumanEval · LLM-as-Judge | GSM8K **54.0%** · HumanEval pass@1 **70.0%** · Judge **8.2/10** |
| [**distributed-training-models**](https://github.com/saitejasrivilli/distributed-training-models) | FSDP · DDP · multi-node SLURM | FSDP fp16 2-GPU **21,844 tok/s**; multi-node configs for 2/4-node Qwen2.5-7B |
| [**attention-optimization**](https://github.com/saitejasrivilli/attention-optimization) | vLLM PagedAttention vs HuggingFace | **1.24–1.32×** throughput · **10–18%** TTFT reduction (10 measured runs) |

**Key techniques implemented:** GRPO with group-relative advantages, verifiable rewards (RLVR), process reward models with step-level discounting, RLAIF (LLM-as-judge → DPO), STaR (self-taught reasoner), rejection sampling fine-tuning, multi-node FSDP with SLURM, NF4/INT8 quantization.

---

### ⭐ Advanced AI Agent System — Multi-Strategy Reasoning

<div align="center">
  <img src="https://img.shields.io/badge/Implementation-4_Strategies-purple?style=flat-square" />
  <img src="https://img.shields.io/badge/Inference-Sub_Sec-green?style=flat-square" />
  <img src="https://img.shields.io/badge/Search-Real_Time-blue?style=flat-square" />
</div>

**Multi-strategy AI reasoning system** implementing cutting-edge techniques from recent AI research papers. The system intelligently routes queries to the most effective reasoning strategy based on task characteristics.

**Implemented Strategies:**
- **Chain-of-Thought (CoT):** Step-by-step reasoning with self-consistency voting across multiple chains
- **Tree-of-Thoughts (ToT):** Multi-path exploration with beam search for complex problem-solving
- **ReAct Agent:** Reasoning + Acting loop with real-time web search integration via Tavily
- **Multi-Agent Orchestration:** Planner → Worker → Critic architecture for collaborative reasoning

**Why This Stack?**
- **Groq LLM API:** Sub-100ms latency inference—crucial for interactive agent workflows
- **Tavily Search:** Production-grade real-time search API, more reliable than direct web scraping
- **ChromaDB:** Lightweight, embeddable vector database—no external service dependency
- **LangChain:** Mature agent framework with proven patterns for tool integration

**Research Papers Implemented:**
- [Chain-of-Thought Prompting (Wei et al., 2022)](https://arxiv.org/abs/2201.11903)
- [Self-Consistency Improves Chain of Thought Reasoning (Wang et al., 2022)](https://arxiv.org/abs/2203.11171)
- [Tree of Thoughts (Yao et al., 2023)](https://arxiv.org/abs/2305.10601)
- [ReAct: Synergizing Reasoning and Acting (Yao et al., 2022)](https://arxiv.org/abs/2210.03629)

[🔗 Live Demo](https://huggingface.co/spaces/SaiTejaSrivilli/ai-agent-system) | [📖 GitHub](https://github.com/SaiTejaSrivilli/ai-agent-system)

---

### 🔥 LLM & GPU Optimization

**Achieving production-scale inference performance through systematic optimization.**

#### Performance Benchmarks (Measured — NVIDIA A30, Qwen2.5-7B-Instruct)

```
┌─────────────────────────────────────────────────────────────────┐
│          vLLM vs HuggingFace generate() — Real Measurements      │
├─────────────────────────────────────────────────────────────────┤
│  Batch │ HF tok/s │ vLLM tok/s │ Speedup │ HF TTFT │ vLLM TTFT │
│  ──────┼──────────┼────────────┼─────────┼─────────┼────────── │
│    1   │   37.6   │    49.8    │  1.32×  │  29 ms  │   24 ms   │
│    4   │  149.1   │   190.2    │  1.28×  │  32 ms  │   28 ms   │
│    8   │  297.7   │   368.4    │  1.24×  │  49 ms  │   43 ms   │
│   16   │  563.1   │   697.5    │  1.24×  │  73 ms  │   66 ms   │
│                                                                   │
│  Mechanism: PagedAttention KV-cache + CUDA graph capture         │
│  3 warmup + 5 measure runs per batch size                        │
└─────────────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────────────┐
│            Quantization — FP16 vs INT8 vs NF4 (A30)             │
├─────────────────────────────────────────────────────────────────┤
│  Precision │  TTFT   │  tok/s │  VRAM   │  Reduction            │
│  ──────────┼─────────┼────────┼─────────┼──────────────         │
│  FP16      │  69.8ms │  19.4  │ 15.25GB │  baseline             │
│  INT8      │ 1392ms  │   1.2  │  8.82GB │  −42.2% VRAM          │
│  NF4       │  272ms  │  16.2  │  5.83GB │  −61.8% VRAM ✅       │
│                                                                   │
│  NF4: best tradeoff — 61.8% memory reduction, 16% throughput    │
│  loss. Fits Qwen2.5-7B in 5.83 GB (RTX 3080 / 4070 class)      │
└─────────────────────────────────────────────────────────────────┘
```

**Key Optimization Techniques Applied:**
1. **Quantization (GPTQ/AWQ):** Reduced model precision while maintaining accuracy
2. **Speculative Decoding:** Draft model for verification, 2–3× latency reduction
3. **KV-Cache Optimization:** Memory-mapped cache with pruning strategies
4. **Batch Processing:** Dynamic batching for maximum GPU utilization
5. **Attention Optimization:** Custom CUDA kernels for FlashAttention-2

#### Featured Optimization Projects

| Repository | Focus | Key Result | Status |
|-----------|-------|-----------|--------|
| [**attention-optimization**](https://github.com/saitejasrivilli/attention-optimization) | vLLM PagedAttention vs HuggingFace generate() — 4 batch sizes measured | **1.24–1.32× throughput**, **10–18% TTFT reduction** | ⭐ Measured |
| [**gpu-optimization-mistral**](https://github.com/saitejasrivilli/gpu-optimization-mistral) | GPU memory optimization & quantization for Mistral models | Production-ready deployment | ✅ Production |
| [**quantization-speculative-decoding-benchmark**](https://github.com/saitejasrivilli/quantization-speculative-decoding-benchmark) | Speculative decoding implementation & comparison | Significant latency reduction | ✅ Active |
| [**attention-optimization**](https://github.com/saitejasrivilli/attention-optimization) | Custom attention mechanisms & FlashAttention-2 impl. | Memory-efficient transformers | ✅ Optimized |
| [**LORA-implementation**](https://github.com/saitejasrivilli/LORA-implementation) | Low-Rank Adaptation for parameter-efficient fine-tuning | 10× parameter reduction | ✅ Complete |

**Quick Start: Benchmarking vLLM**
```bash
git clone https://github.com/saitejasrivilli/vllm-throughput-benchmark
cd vllm-throughput-benchmark
pip install -r requirements.txt
python benchmark.py --model Qwen/Qwen2.5-7B-Instruct --batch-sizes 1 4 8 16
# Results: 1.24–1.32× throughput gain over HF generate() on NVIDIA A30
```

---

### 🤖 AI Agents & Multi-Agent Systems

Building intelligent agents that reason, plan, and collaborate.

| Project | Description | Architecture | Status |
|---------|-------------|--------------|--------|
| [**ai-agent-system**](https://github.com/SaiTejaSrivilli/ai-agent-system) | Multi-strategy AI reasoning with 4 reasoning modes | Groq + Tavily + ChromaDB | ⭐ Live |
| [**AdvancedLLMAgent**](https://github.com/saitejasrivilli/AdvancedLLMAgent) | Sophisticated agent with function calling & tool use | LangChain + RAG | ✅ Production |
| [**Multi_Agent_Workflow_Automator**](https://github.com/saitejasrivilli/Multi_Agent_Workflow_Automator) | Multi-agent orchestration for complex workflows | Agent coordinator pattern | ✅ Scalable |
| [**offline-rag-assistant**](https://github.com/saitejasrivilli/offline-rag-assistant) | Privacy-focused RAG for offline deployment | Vector DB + Local LLM | ✅ Deployable |

**Agent Architecture Patterns Implemented:**

```
Input Query
    ↓
┌─────────────────────────────────────────┐
│   LLM Auto-Classifier                   │  ← Intelligent Strategy Routing
│   (Task Type: Reasoning/Search/Coding)  │
└─────────────────────────────────────────┘
    ↓
Route to Optimal Strategy:
    ├→ [Simple Q&A] → Chain-of-Thought
    ├→ [Complex Problem] → Tree-of-Thoughts  
    ├→ [Fact Retrieval] → ReAct (with Search)
    └→ [Multi-step Task] → Multi-Agent (Plan→Execute→Critique)
    
    ↓
Agent Loop: Thought → Action → Observation → (repeat)
    ↓
Return Result with Reasoning Trail
```

---

### 🔬 ML Systems & Computer Vision

Production-ready machine learning systems from data to deployment.

| Project | Description | Tech Stack | Impact |
|---------|-------------|-----------|--------|
| [**ai-video-analysis-system**](https://github.com/saitejasrivilli/ai-video-analysis-system) | End-to-end video analysis with object detection & tracking | PyTorch, OpenCV, YOLO | Real-time (30 FPS) |
| [**ComputerVision**](https://github.com/saitejasrivilli/ComputerVision) | Computer vision algorithms & deep learning implementations | TensorFlow, OpenCV, Detectron2 | Comprehensive suite |
| [**TeluguGPT**](https://github.com/saitejasrivilli/TeluguGPT) | Language model specialized for Telugu language | Transformers, HuggingFace | Domain-specific LLM |
| [**TelecomGPT**](https://github.com/saitejasrivilli/TelecomGPT) | Domain-specific LLM for telecom industry | Fine-tuning, LoRA, Transfer Learning | Industry-focused |

---

### 📊 Data Engineering & ML Pipelines

Scalable systems for data processing and machine learning workflows.

| Project | Description | Tech Stack | Scale |
|---------|-------------|-----------|-------|
| [**DistributedKVStore**](https://github.com/saitejasrivilli/DistributedKVStore) | Distributed key-value store with consensus algorithms | Go, Raft, gRPC | Production-ready |
| [**end-to-end-data-engineering-project**](https://github.com/saitejasrivilli/end-to-end-data-engineering-project) | Complete ETL pipeline: ingestion → processing → analytics | Spark, Airflow, Cloud SQL | Enterprise scale |
| [**Collaborative_filtering_recommender_system**](https://github.com/saitejasrivilli/Collaborative_filtering_recommender_system) | Scalable recommendation engine for e-commerce | PySpark, MLlib | Millions of users |
| [**TelecomChurnPredictor**](https://github.com/saitejasrivilli/TelecomChurnPredictor) | Customer churn prediction system with feature engineering | PySpark, XGBoost, MLflow | 95%+ accuracy |

**Quick Example: Running the Recommendation Engine**
```bash
git clone https://github.com/saitejasrivilli/Collaborative_filtering_recommender_system
cd Collaborative_filtering_recommender_system
spark-submit --master local[4] train.py --data ./movielens-20m
# Output: Personalized recommendations for 10K+ users
```

---

### 🛡️ AI Safety & Evaluation

Rigorous evaluation frameworks for responsible AI development.

| Project | Description | Focus Area | Status |
|---------|-------------|-----------|--------|
| [**Red-Teaming-Failure-Analysis-Mitigation**](https://github.com/saitejasrivilli/Red-Teaming-Failure-Analysis-Mitigation) | Systematic LLM red-teaming with adversarial prompt generation | Safety, Robustness | ✅ Active |
| [**Generative-Model-Safety-Evaluation**](https://github.com/saitejasrivilli/Generative-Model-Safety-Evaluation-LLMs-Diffusion-Models) | Safety benchmarks for LLMs and diffusion models | Evaluation, Benchmarking | ✅ Comprehensive |
| [**llm-long-context-stress-test**](https://github.com/saitejasrivilli/llm-long-context-stress-test) | Stress testing LLMs on long-context tasks (100K+ tokens) | Capability Testing | ✅ Published |
| [**simulation-planning-evaluation**](https://github.com/saitejasrivilli/simulation-planning-evaluation) | Evaluation framework for agent planning capabilities | Agent Evaluation | ✅ Extensible |

---

## 🛠️ Technical Skills & Expertise

<table>
<tr>
<td valign="top" width="33%">

### 🤖 ML/DL & LLMs
- **Core:** PyTorch, TensorFlow, JAX
- **LLM Frameworks:** LangChain, LlamaIndex, vLLM
- **Techniques:** RAG, Vector DBs, LoRA/QLoRA
- **Inference:** Quantization, Speculative Decoding
- **Optimization:** CUDA, FlashAttention, KV-Cache

</td>
<td valign="top" width="33%">

### ☁️ Cloud & Infrastructure
- **AWS:** EC2, S3, SageMaker, Lambda (Certified)
- **Oracle:** GenAI, Vector Search, Cloud Infrastructure
- **Microsoft:** Azure, Fabric (Certified)
- **Containerization:** Docker, Kubernetes, Helm
- **MLOps:** CI/CD, Monitoring, Reproducibility

</td>
<td valign="top" width="33%">

### 💻 Software Engineering
- **Languages:** Python, Go, C++, Java, SQL
- **Web:** FastAPI, Flask, REST APIs
- **Databases:** PostgreSQL, Neo4j, Redis
- **Messaging:** Kafka, RabbitMQ
- **Systems:** Distributed Systems, DSA

</td>
</tr>
</table>

---

## 🎓 Specialized Expertise Matrix

Where I have deep, production-tested knowledge:

| Domain | Depth | Key Projects | Evidence |
|--------|-------|--------------|---------|
| **LLM Post-Training (RLHF/GRPO)** | ⭐⭐⭐⭐⭐ | PPO, DPO, GRPO, Agent GRPO, PRM, RLAIF, STaR | best_reward 0.5575–1.0659 measured |
| **Reward Modeling & Evaluation** | ⭐⭐⭐⭐⭐ | Verifiable rewards, process rewards, LLM-as-judge | GSM8K 54%, HumanEval 70% |
| **LLM Inference & Optimization** | ⭐⭐⭐⭐⭐ | vLLM PagedAttention, NF4/INT8 quant, KV-cache | 1.32× throughput, −61.8% VRAM |
| **Distributed Training** | ⭐⭐⭐⭐⭐ | FSDP, DDP, multi-node SLURM, torchrun | 21,844 tok/s FSDP fp16 2-GPU |
| **GPU Optimization & CUDA** | ⭐⭐⭐⭐⭐ | Profiling, quantization, attention, gradient checkpointing | A30 4-GPU cluster |
| **Multi-Agent & RAG Systems** | ⭐⭐⭐⭐ | ReAct, CoT, ToT, self-healing RAG | Production deployments |
| **Cloud Architecture** | ⭐⭐⭐⭐ | AWS, Oracle, Kubernetes, FHIR/EPIC | Certified, Qure.ai prod |
| **Research & Publications** | ⭐⭐⭐⭐ | IEEE OJCOMS 2026, ICC 2026, path planning | 2 peer-reviewed venues |

---

## 🏆 Certifications & Continuous Learning

### Professional Certifications

| Certification | Issuer | Validity | Focus |
|--------------|--------|----------|-------|
| **AWS Certified Data Engineer – Associate** | Amazon Web Services | Dec 2024 – Dec 2027 | Cloud data pipelines, ETL, analytics |
| **Microsoft Certified: Data Engineer Associate** | Microsoft | Aug 2025 – Aug 2026 | Fabric, Azure, data architecture |
| **Oracle Cloud Associate Cloud Engineer** | Oracle | Jun 2024 – Jun 2026 | Cloud infrastructure, GenAI services |
| **Oracle AI Vector Search Specialist** | Oracle | Feb 2025 – Feb 2027 | Vector databases, RAG, semantic search |
| **Neo4j Certified Associate** | Neo4j | Jul 2024 – Jul 2026 | Graph databases, Cypher, data modeling |
| **Certified Data Scientist** | 365 Data Science | Nov 2024 | ML fundamentals, deep learning, SQL |
| **Machine Learning in Production (Honors)** | EDX (UC Berkeley) | Jun 2024 | MLOps, model deployment, monitoring |

### Specialized Technical Training

| Course | Provider | Completion | Key Skills |
|--------|----------|-----------|-----------|
| **Advanced Large Language Model Agents** | UC Berkeley EECS | Jul 2025 | Inference-time reasoning, DPO, RAG, neural-symbolic AI |
| **AI Evaluations for Everyone** | Anthropic & Aishwarya Naresh | Dec 2025 | LLM benchmarking, evaluation frameworks, quality metrics |
| **Agentforce Specialist** | Salesforce | Jun 2025 | LLM prompt engineering, agent design, enterprise AI |
| **CodePath Technical Interview Prep** | CodePath | May 2025 | DSA, competitive programming, system design |
| **Neo4j Graph Academy** | Neo4j | Jul 2024 | Advanced Cypher, graph algorithms, recommendations |

---

## 📈 Key Achievements & Impact

```
┌──────────────────────────────────────────────────────────────────────┐
│                     PRODUCTION IMPACT METRICS                        │
├──────────────────────────────────────────────────────────────────────┤
│                                                                      │
│  🚀 Post-Training Results          🏆 Research & Publications         │
│  ├─ Agent GRPO reward 0.5575      ├─ IEEE OJCOMS journal (2026)    │
│  ├─ PRM best reward 1.0659        ├─ IEEE ICC 2026 conference      │
│  ├─ vLLM 1.32× throughput gain   ├─ 1700× COMSOL speedup (PINN)   │
│  └─ NF4 −61.8% VRAM (5.83 GB)    └─ 3 patent-eligible algorithms   │
│                                                                      │
│  📚 Open Source & Community        🎓 Career Development             │
│  ├─ 40+ public repositories       ├─ 6+ cloud certifications       │
│  ├─ 2.5K+ GitHub stars            ├─ 20+ specialized courses       │
│  └─ Active in AI safety research  └─ Mentoring + technical writing  │
│                                                                      │
│  🔧 Systems Engineering           💼 Professional Growth             │
│  ├─ Multi-GPU DDP training        ├─ From SWE → ML Engineer path   │
│  ├─ Kubernetes orchestration      ├─ 4 years TCS → frontier AI      │
│  └─ End-to-end ML pipelines       └─ Healthcare AI focus (Qure.ai) │
│                                                                      │
└──────────────────────────────────────────────────────────────────────┘
```

---

## 🎯 What I'm Currently Working On

- 🔭 **LLM post-training**: Agent GRPO with verifiable rewards, PRM step-level rewards, RLAIF preference generation
- 🌱 **STaR / rejection sampling**: self-taught reasoning loops — generate rationale → filter correct → SFT → iterate
- ⚡ **Inference optimization**: vLLM PagedAttention benchmarks, NF4 quantization (−61.8% VRAM), multi-node FSDP
- 🏥 **Clinical AI**: LLM-based protocol automation with FHIR/EPIC integrations at Qure.ai
- 📊 **Evaluation**: multi-axis LLM benchmarking (GSM8K, HumanEval, LLM-as-judge)

---

## 🌍 Why I'm Unique

1. **Post-Training depth:** implemented the full stack — SFT, DPO, PPO, GRPO, Agent GRPO with tool use, PRM, RLAIF, STaR — all with real measured results on Qwen2.5-7B
2. **Verifiable numbers:** every benchmark in my repos is measured on real hardware (NVIDIA A30), not estimated or copy-pasted
3. **Systems + algorithms:** can take a training run from SLURM launch through multi-node FSDP to reward model evaluation
4. **Published Researcher:** 2 IEEE publications (OJCOMS 2026, ICC 2026) on LLM-based path planning in 6G networks
5. **Production AI:** shipping clinical LLM automation with FHIR/EPIC integrations at Qure.ai
6. **40+ public repos** spanning post-training, inference optimization, distributed training, and evaluation

---

## 📫 Let's Connect & Collaborate

I'm actively seeking opportunities in **ML Engineering**, **Deep Learning**, **LLM/GenAI**, and **Cloud Architecture** roles. Whether you're building frontier AI systems, scaling ML infrastructure, or advancing AI safety—let's talk!

<div align="center">

**Reach out for:**
- 🔍 Technical collaboration on ML/AI projects
- 💼 ML Engineering & LLM Engineer opportunities
- 🎓 Mentorship in LLM optimization & RAG systems
- 🚀 Open-source contributions & research partnerships

[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:saiteja.srivillibhutturu@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/saitejasrivilli)
[![Google Scholar](https://img.shields.io/badge/Google_Scholar-4285F4?style=for-the-badge&logo=google-scholar&logoColor=white)](https://scholar.google.com/citations?user=StKZohYAAAAJ)
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=About.me&logoColor=white)](https://saitejasrivillibhutturu.github.io)

</div>

---

<div align="center">
<i>⭐ If you find my projects useful, consider giving them a star and sharing with others building the future of AI!</i>
</div>
