<div align="center">

# 👋 Hi, I'm Sai Teja Srivillibhutturu

### Software Engineer – AI/ML | LLM Systems · ML Infrastructure · Distributed Systems · GPU Optimization

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge\&logo=linkedin\&logoColor=white)](https://linkedin.com/in/saitejasrivilli)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge\&logo=github\&logoColor=white)](https://github.com/saitejasrivilli)
[![Google Scholar](https://img.shields.io/badge/Google_Scholar-4285F4?style=for-the-badge\&logo=google-scholar\&logoColor=white)](https://scholar.google.com/citations?user=StKZohYAAAAJ)
[![Portfolio](https://img.shields.io/badge/Portfolio-FF5722?style=for-the-badge\&logo=google-chrome\&logoColor=white)](https://saitejasrivillibhutturu.github.io)

</div>

---

## 🎯 About Me

I'm a **Software Engineer – AI/ML at Oracle** focused on building production AI systems across **LLM applications, retrieval, model evaluation, inference optimization, and cloud infrastructure**.

My background combines:

* **Production AI/ML:** RAG, LLM evaluation, fine-tuning, model serving, inference optimization
* **ML Systems:** PyTorch, distributed training, CUDA, NCCL, FSDP, vLLM, FlashAttention
* **Distributed Systems:** microservices, replication, consensus, fault tolerance, Kubernetes
* **Backend Engineering:** Python, Go, Java, REST APIs, PostgreSQL, Redis
* **Research:** LLM-based path planning, digital twins, wireless connectivity optimization

I enjoy working at the intersection of **machine learning and systems engineering** — taking models from experimentation through optimization, deployment, evaluation, and production operation.

---

## 💼 Professional Experience

### **Oracle — Software Engineer, AI/ML**

**Jun 2025 – Present | United States**

* Engineer production ML/LLM systems spanning **data processing, retrieval, ranking, evaluation, and inference**.
* Built enterprise RAG pipelines covering **document processing, embeddings, hybrid search, reranking, and LLM generation**, improving retrieval relevance **21%** and reducing hallucinations **30%**.
* Developed Python/SQL pipelines and automated evaluation frameworks measuring accuracy, retrieval quality, ranking performance, latency, and failure rates across **thousands of queries**.
* Applied **SFT/LoRA fine-tuning, batching, KV caching, and quantization**, improving task accuracy **78% → 86%** and reducing p95 latency **1.2s → 420ms**.
* Productionized ML/GenAI services using **AWS, Docker, Kubernetes, and CI/CD** with validation, monitoring, versioning, and rollback.

### **University of Texas at Arlington — Graduate Research Assistant**

**Aug 2024 – May 2025 | Arlington, TX**

* Developed an LLM-powered connectivity-aware navigation system combining **OpenStreetMap/OSMnx, Blender Digital Twins, and NVIDIA Sionna** for realistic mmWave signal propagation.
* Automated Digital Twin dataset generation into **1,000+ instruction-tuning samples** using Python, NumPy, and Pandas on **4× NVIDIA A30 GPUs**.
* Fine-tuned GPT-4o Mini on routing datasets generated with a modified Dijkstra algorithm, improving valid route generation **71.4% → 100%** while achieving **76.4% oracle signal coverage**.
* Accelerated routing experiments **~60%** using Dockerized GPU environments and PyTorch/CUDA across **10K+ routing scenarios**.

### **Tata Consultancy Services — Software Engineer**

**Jun 2019 – May 2023 | Chennai, India**

* Scaled Java/Spring Boot microservices on OCI and Kubernetes from **20 to 50+ services** across development, staging, and production.
* Owned production services and resolved **20+ critical incidents**, improving SLA compliance from **95% → 99.9%**.
* Increased distributed-system capacity **40%** while reducing infrastructure overhead **20%** through Spring Boot, PostgreSQL, Redis, and connection-pool optimization.
* Automated deployments using **Jenkins, GitHub Actions, Docker, and Kubernetes**, enabling blue-green deployments and zero-downtime releases.
* Conducted **100+ code reviews** and mentored **5+ engineers** while improving API response time **25%** and reducing database load **20%**.

---

## 🚀 Featured Projects

### 🧠 LLM Post-Training

| Repository                                                                                            | Focus                                              | Key Result                                          |
| ----------------------------------------------------------------------------------------------------- | -------------------------------------------------- | --------------------------------------------------- |
| [**rlhf-synthesis-optimization**](https://github.com/saitejasrivilli/rlhf-synthesis-optimization)     | PPO · DPO · GRPO · Agent GRPO · PRM · RLAIF · STaR | Agent GRPO reward **0.5575**; PRM reward **1.0659** |
| [**LLM_FineTuning_SFT_Production**](https://github.com/saitejasrivilli/LLM_FineTuning_SFT_Production) | SFT → DPO → RLVR                                   | BERTScore **0.780 → 0.855**; DPO margin **+0.137**  |
| [**efficient-post-training-suite**](https://github.com/saitejasrivilli/efficient-post-training-suite) | SFT · DPO · GRPO · Agent RL                        | Multi-stage A30 training pipeline                   |
| [**reward-model-training**](https://github.com/saitejasrivilli/reward-model-training)                 | Bradley-Terry Reward Model                         | **65.0%** validation accuracy                       |

### ⚡ LLM Inference & GPU Optimization

| Repository                                                                                        | Focus                                        | Key Result                                           |
| ------------------------------------------------------------------------------------------------- | -------------------------------------------- | ---------------------------------------------------- |
| [**attention-optimization**](https://github.com/saitejasrivilli/attention-optimization)           | vLLM PagedAttention                          | **1.24–1.32× throughput**, **10–18% TTFT reduction** |
| [**gpu-optimization-mistral**](https://github.com/saitejasrivilli/gpu-optimization-mistral)       | Quantization · Kernel Fusion · GPU Profiling | NF4 **61.8% VRAM reduction**                         |
| [**distributed-training-models**](https://github.com/saitejasrivilli/distributed-training-models) | DDP · FSDP · Multi-GPU Training              | **21,844 tok/s** FSDP FP16 on 2 GPUs                 |
| [**LORA-implementation**](https://github.com/saitejasrivilli/LORA-implementation)                 | Parameter-efficient fine-tuning              | **10× parameter reduction**                          |

### 🌐 Distributed Systems

| Repository                                                                                                              | Focus                                          | Key Result                            |
| ----------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------- | ------------------------------------- |
| [**LedgerDB**](https://github.com/saitejasrivilli/ledgerdb)                                                             | Raft · Replication · Partitioning · MVCC · WAL | **0 data loss / 100 recovery cycles** |
| [**Distributed Object Store**](https://github.com/saitejasrivilli/distributed-object-store)                             | Replication · Quorum · Failure Recovery        | ~**5K writes/sec**                    |
| [**DistributedKVStore**](https://github.com/saitejasrivilli/DistributedKVStore)                                         | Distributed KV Storage · Consensus             | Go-based distributed storage          |
| [**distributed-service-mesh-control-plane**](https://github.com/saitejasrivilli/distributed-service-mesh-control-plane) | Service Discovery · xDS · Control Plane        | Kubernetes/Envoy-based control plane  |

### 🤖 AI Agents & Evaluation

| Repository                                                                                    | Focus                               | Result                                                                     |
| --------------------------------------------------------------------------------------------- | ----------------------------------- | -------------------------------------------------------------------------- |
| [**code-agent-eval-benchmark**](https://github.com/saitejasrivilli/code-agent-eval-benchmark) | ReAct · Tool Use · Agent Evaluation | **100% task success**, **100% error recovery**                             |
| [**ai-agent-system**](https://github.com/SaiTejaSrivilli/ai-agent-system)                     | CoT · ToT · ReAct · Multi-Agent     | [Live Demo](https://huggingface.co/spaces/SaiTejaSrivilli/ai-agent-system) |
| [**AdvancedLLMAgent**](https://github.com/saitejasrivilli/AdvancedLLMAgent)                   | Tool Calling · RAG · Agents         | LangChain-based agent                                                      |
| [**offline-rag-assistant**](https://github.com/saitejasrivilli/offline-rag-assistant)         | Local LLM · Vector Search · RAG     | Offline deployment                                                         |

---

## 🔬 Research

### **DTMAP: Digital Twin-Guided AI Path Planning for Connectivity-Aware Mobility**

**IEEE Open Journal of the Communications Society — Accepted 2026**

Multi-objective path-planning framework combining wireless digital twins with a fine-tuned LLM for connectivity-aware navigation in 6G/XR environments.

* **1.9% outage probability** vs. 2.3% for RL baseline
* **312 ms** average inference latency
* Tunable optimization parameter controlling signal strength vs. travel distance
* GPT-4o Mini fine-tuned using Digital Twin-grounded routing data
* Deterministic sanitization improved raw LLM path validity **65% → 100%**

**Stack:** GPT-4o Mini, OpenAI Fine-tuning API, NVIDIA Sionna, OpenStreetMap, Blender, Python, PyTorch

[📖 arXiv](https://arxiv.org/abs/2601.00110)

---

### **CTMap: LLM-Enabled Connectivity-Aware Path Planning in Millimeter-Wave Digital Twin Networks**

**IEEE ICC 2026**

LLM-driven path optimization for next-generation mmWave/6G networks using Digital Twin simulation and connectivity-aware routing.

* Connectivity-aware routing using mmWave signal propagation
* Digital Twin-based network simulation
* Modified Dijkstra routing
* LLM-based path planning
* Practical edge inference considerations

[📖 arXiv](https://arxiv.org/abs/2601.00110)

---

## 📊 Selected Benchmarks

### LLM Inference — NVIDIA A30

| Batch | Hugging Face |        vLLM |   Speedup | TTFT Reduction |
| ----: | -----------: | ----------: | --------: | -------------: |
|     1 |   37.6 tok/s |  49.8 tok/s | **1.32×** |        **17%** |
|     4 |  149.1 tok/s | 190.2 tok/s | **1.28×** |        **13%** |
|     8 |  297.7 tok/s | 368.4 tok/s | **1.24×** |        **12%** |
|    16 |  563.1 tok/s | 697.5 tok/s | **1.24×** |        **10%** |

**Mechanism:** vLLM PagedAttention + CUDA graph capture.

### Quantization — Qwen2.5-7B

| Precision |    TTFT | Throughput |        VRAM |
| --------- | ------: | ---------: | ----------: |
| FP16      | 69.8 ms | 19.4 tok/s |    15.25 GB |
| INT8      | 1392 ms |  1.2 tok/s |     8.82 GB |
| NF4       |  272 ms | 16.2 tok/s | **5.83 GB** |

NF4 reduced VRAM **61.8%** with approximately **16% throughput loss**.

---

## 🛠️ Technical Skills

### ML / LLM

* PyTorch, JAX, Hugging Face Transformers
* LLMs, RAG, Fine-Tuning, LoRA/QLoRA
* SFT, DPO, GRPO, RLVR, Reward Models
* Embeddings, Vector Search, Reranking
* Agentic AI, Tool Calling, Model Evaluation

### ML Systems / GPU

* PyTorch DDP, FSDP, NCCL
* CUDA, FlashAttention-2, vLLM
* TensorRT, ONNX Runtime
* KV Cache, PagedAttention
* Quantization: NF4, INT8
* Distributed Training, Model Serving

### Distributed Systems / Backend

* Go, Java, Python, C++, SQL
* Raft, Replication, Partitioning, MVCC
* Fault Tolerance, High Availability
* Microservices, REST, gRPC
* PostgreSQL, Redis, MySQL

### Cloud / Infrastructure

* AWS: EC2, S3, Lambda, SageMaker
* Kubernetes, Docker
* Jenkins, GitHub Actions, CI/CD
* Prometheus, Grafana
* Oracle Cloud Infrastructure

---

## 🏆 Selected Impact

* **21%** improvement in RAG retrieval relevance
* **30%** reduction in RAG hallucinations
* **78% → 86%** task accuracy improvement
* **1.2s → 420ms** p95 LLM latency reduction
* **3.14×** distributed training throughput improvement
* **21%** per-GPU memory reduction with FSDP
* **1.24–1.32×** vLLM inference throughput improvement
* **61.8%** VRAM reduction with NF4 quantization
* **20 → 50+** production microservices at TCS
* **95% → 99.9%** production SLA improvement
* **40%** backend capacity improvement
* **100+** code reviews
* **5+** engineers mentored
* **1,000+** Digital Twin instruction-tuning samples
* **10K+** routing scenarios
* **100%** valid route generation
* **0 data loss** across 100 LedgerDB failure-recovery cycles

---

## 📚 Certifications

* AWS Certified Data Engineer – Associate
* Microsoft Certified: Data Engineer Associate
* Oracle Cloud Associate Cloud Engineer
* Oracle AI Vector Search Specialist
* Neo4j Certified Associate

---

## 📫 Connect

I'm interested in opportunities across **AI/ML Engineering, ML Systems, LLM Infrastructure, Distributed Systems, and Software Engineering**.

* 💼 [LinkedIn](https://linkedin.com/in/saitejasrivilli)
* 💻 [GitHub](https://github.com/saitejasrivilli)
* 📚 [Google Scholar](https://scholar.google.com/citations?user=StKZohYAAAAJ)
* 🌐 [Portfolio](https://saitejasrivillibhutturu.github.io)

</div>
