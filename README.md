# Hi, I'm Xiaorui Zhang

**M.S. Electrical Engineering @ Columbia University | Software Engineering · Systems · ML Infrastructure**

Seeking Summer 2027 Software Engineering / Software Development internships in the United States. Based in New York City.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/xiaoruizhang12345)
[![Email](https://img.shields.io/badge/Email-Contact-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:xz3569@columbia.edu)

## About Me

- Pursuing an M.S. in Electrical Engineering at Columbia University.
- Earned a B.S. in Computer Engineering with Honors from the University of Illinois Urbana-Champaign, with an engineering foundation through the ZJU-UIUC Institute at Zhejiang University.
- Focused on software engineering, with additional interests in systems and ML infrastructure.
- Build end-to-end software systems, data pipelines, developer tools, and engineering-oriented ML workflows.
- Seeking Summer 2027 SWE/SDE internship opportunities.

## Tech Stack

**Languages**  
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat&logo=go&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat&logo=c&logoColor=111111)
![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=flat&logo=cplusplus&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=111111)

**Backend & Web**  
![gRPC](https://img.shields.io/badge/gRPC-244C5A?style=flat)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=flat&logo=sqlalchemy&logoColor=white)
![REST APIs](https://img.shields.io/badge/REST_APIs-005571?style=flat)

**ML, Data & Numerical Computing**  
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=flat&logo=pandas&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat&logo=scikitlearn&logoColor=white)
![Numba](https://img.shields.io/badge/Numba-00A3E0?style=flat&logo=numba&logoColor=white)

**Systems & Tools**  
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat&logo=kubernetes&logoColor=white)
![MinIO](https://img.shields.io/badge/MinIO-C72E49?style=flat)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=111111)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat&logo=pytest&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=githubactions&logoColor=white)
![Ruff](https://img.shields.io/badge/Ruff-D7FF64?style=flat&logo=ruff&logoColor=111111)
![mypy](https://img.shields.io/badge/mypy-2A6DB2?style=flat)

## Featured Projects

### [RAE — Feature Compression & Sharded Retrieval](https://github.com/xiaorui7/rae-feature-compression-benchmark)

Python feature-compression pipeline and Go retrieval service with replicated gRPC shards and an HTTP coordinator. Offline representations come from the official frozen RAE encoder.

- Implemented exact cosine search across shards with deterministic global top-k merging and checksum-verified vector exports.
- Added deadline propagation, bounded retries, explicit partial-result handling, health checks, Prometheus metrics, and replica routing on local Kubernetes.
- Verified 72,000 query checks with zero ID mismatches; measured 1,026 QPS at 31 ms p99 on a local synthetic 50k × 64 FP32 workload with two shards and two replicas each.

`Go` `gRPC` `Python` `PyTorch` `Kubernetes` `Docker` `Prometheus`

### [StepWise — Wearable Sensor Analytics Platform](https://github.com/xiaorui7/StepWise-Wearable-Sensor-Analytics-Platform)

Asynchronous gait-analysis platform that processes wearable sensor recordings and delivers reports through a FastAPI backend and React dashboard.

- Implemented PostgreSQL-backed job state, Redis/RQ workers, idempotent submissions, bounded retries, and execution-token checks that prevent stale workers from publishing results.
- Added S3-compatible MinIO storage with checksum-verified artifacts; deployed two API replicas and two workers on a local kind Kubernetes cluster without shared application filesystems.
- Passed 106 tests with no skips against PostgreSQL, Redis/RQ, and MinIO; verified interrupted publication and cross-replica report consistency through integration and local cluster checks.

`Python` `FastAPI` `PostgreSQL` `Redis/RQ` `React` `Kubernetes` `MinIO` `Docker` `pytest`

### [RISC-V Storage Systems Lab](https://github.com/xiaorui7/riscv-storage-lab)

C and RISC-V teaching operating system running under QEMU, focused on storage correctness, reproducible builds, and measurable block-cache behavior.

- Built source-generated KTFS images, an out-of-source build, a bounded Python test runner, and a matching GitHub Actions workflow.
- Improved cache consistency and failure handling across dirty reads, partial transfers, victim replacement, write retries, and referenced-block flushing.
- Added 20 QEMU storage regression cases, per-cache instrumentation, and deterministic workloads spanning KTFS, the cache layer, I/O abstraction, and VirtIO.

`C` `Linux` `QEMU` `VirtIO` `Python` `Make` `GitHub Actions`

### [High-Performance Telemetry Processing Engine](https://github.com/xiaorui7/high-performance-telemetry-engine)

High-performance processing engine for validating, aligning, and analyzing heterogeneous industrial-equipment telemetry with bounded memory and reproducible benchmarks.

- Built a CLI pipeline that ingests public UCI and deterministic synthetic cycles, validates malformed data, aligns multi-rate sensors, applies configurable diagnostic rules, and writes CSV/JSON artifacts.
- Designed interchangeable reference Python, vectorized NumPy, and parallel Numba backends; four-thread Numba reached 21,789 cycles/second and 27.34× reference throughput with ≤4.62e-14 maximum absolute error.
- Measured the complete file-to-output path at 391.5 cycles/second across 1,000 five-channel cycles; verified batch-memory trade-offs with 41 tests, 78% coverage, and Windows/Linux CI.

`Python` `NumPy` `Numba` `PyYAML` `pytest` `GitHub Actions`

## Education

**Columbia University**  
M.S. in Electrical Engineering

**University of Illinois Urbana-Champaign**  
B.S. in Computer Engineering, with Honors

**Zhejiang University**  
Engineering background through the ZJU-UIUC Institute

## Connect

[LinkedIn](https://linkedin.com/in/xiaoruizhang12345) · [Email](mailto:xz3569@columbia.edu)
