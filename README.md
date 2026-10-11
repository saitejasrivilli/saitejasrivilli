<div align="center">

# Sai Teja Srivillibhutturu

### ML Systems & LLM Inference Engineer
**GPU Optimization · LLM Training & Serving · Distributed Systems · Backend Engineering**

[LinkedIn](https://linkedin.com/in/saitejasrivilli) · [GitHub](https://github.com/saitejasrivilli) · [Portfolio](https://saitejasrivilli.github.io) · [Google Scholar](https://scholar.google.com/citations?user=StKZohYAAAAJ)

</div>

---

## About

I build and evaluate machine-learning systems from model training through inference, performance analysis, and deployment. My work spans LLM fine-tuning and retrieval, GPU kernels and compiler optimization, distributed training, and fault-tolerant backend systems.

## Experience

### Oracle — Software Engineer, AI/ML
**Jun 2025 – Present**

- Engineer production ML/LLM systems across data processing, retrieval, ranking, evaluation, and inference services using Python and PyTorch.
- Internal evaluation work reported a **21% retrieval-relevance improvement** and **30% fewer hallucinations**; model/task tuning improved measured accuracy from **78% to 86%**, while a serving optimization reduced p95 latency from **1.2 s to 420 ms**.
- Support deployment validation, model/version management, monitoring, and reliable inference operation.

### The University of Texas at Arlington — Graduate Research Assistant & Graduate Teaching Assistant
**Aug 2024 – May 2025 · Arlington, Texas**

- Built **TopGPT**, fine-tuned on 3+ textbooks and paired with retrieval-augmented generation over 1,000+ research-paper chunks stored in Pinecone.
- Researched **CTMap/DTMAP**, combining LLM-enabled path planning, Dijkstra-generated routes, OpenStreetMap, digital twins, and NVIDIA Sionna for connectivity-aware mmWave/6G mobility.
- Supported Numerical Methods instruction for 50+ students using Python and MATLAB.

### Tata Consultancy Services — Assistant System Engineer / Software Engineer
**Jun 2019 – May 2023**

- Built and operated Java/Spring Boot services across development, staging, and production, scaling the service footprint from **20 to 50+ services**.
- Resolved 20+ critical incidents and improved reported SLA compliance from **95% to 99.9%**; backend capacity increased **40%** while infrastructure overhead fell **20%** through service, database, and connection-pool optimization.
- Conducted 100+ code reviews and mentored 5+ engineers.

---

## Featured Projects

| Project | What it demonstrates | Reported benchmark / evidence |
|---|---|---|
| [metal-inference-server](https://github.com/saitejasrivilli/metal-inference-server) | Continuous-batching LLM inference for Apple Silicon, paged KV cache, streaming, cancellation, metrics, and traces | About 1.5× throughput improvement from continuous batching in the documented M-series Mac setup; negative quantization results are also documented |
| [LLMBoost](https://github.com/saitejasrivilli/LLMBoost) | MLIR compiler pass for RMSNorm → Linear fusion | 2.20× FP16 and 1.55× BF16 speedup for the measured workload on a 4× NVIDIA A30 cluster |
| [flash-attn-from-scratch](https://github.com/saitejasrivilli/flash-attn-from-scratch) | Triton FlashAttention, int8 GEMM with fused dequantization, and fused CUDA kernels | NVIDIA A30 measurements with per-sequence-length comparisons against PyTorch SDPA |
| [distributed-training-models](https://github.com/saitejasrivilli/distributed-training-models) | PyTorch DDP/FSDP, mixed precision, and pipeline-parallel training | 3.14× AMP throughput versus FP32 in the reported single-A30 setup; FSDP memory results documented by configuration |
| [search-engine-rs](https://github.com/saitejasrivilli/search-engine-rs) | Rust tokenizer, inverted index, BM25, sharded query execution, and HTTP control plane | Median 1.55× postings-intersection speedup and 4.35× batch-query speedup across five runs on 82,360 MS MARCO passages |
| [ledgerdb](https://github.com/saitejasrivilli/ledgerdb) | Go distributed commit log/document store with Raft, MVCC, WAL, TCP transport, MinIO, and fault injection | Benchmark artifacts and network-failure scenarios are committed with the project |

More projects: [all public repositories](https://github.com/saitejasrivilli?tab=repositories).

## Research

- **DTMAP — Digital Twin-Guided AI Path Planning for Connectivity-Aware Mobility.** *IEEE Open Journal of the Communications Society, 2026.* [DOI](https://doi.org/10.1109/OJCOMS.2026.3683886)
- **CTMap — LLM-Enabled Connectivity-Aware Path Planning for mmWave 6G Networks.** *IEEE ICC 2026.* [arXiv preprint](https://arxiv.org/abs/2601.00110)
- **Efficiency–Equity Trade-Off Characterization in Hierarchical Traffic Congestion Pricing.** *IEEE ITSC 2026.* [Paper PDF](https://dipupo.github.io/pdf/ITSC26_1413_FI.pdf)

## Technical Areas

- **ML / LLM:** PyTorch, JAX, Hugging Face Transformers, RAG, SFT, LoRA/QLoRA, model evaluation, embeddings, reranking
- **Inference / GPU:** CUDA C++, Triton, FlashAttention, vLLM, KV cache, quantization, kernel fusion, ONNX Runtime, TensorRT
- **Distributed systems:** Go, Java, Rust, Raft, replication, MVCC, WAL, sharding, fault injection, microservices
- **Infrastructure:** AWS, Docker, Kubernetes, CI/CD, Prometheus, OpenTelemetry, PostgreSQL, Redis

## Contact

- [LinkedIn](https://linkedin.com/in/saitejasrivilli)
- [Email](mailto:saiteja.srivillibhutturu@gmail.com)
- [Portfolio](https://saitejasrivilli.github.io)
