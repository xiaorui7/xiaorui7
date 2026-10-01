# Hi, I'm Xiaorui Zhang

**M.S. Electrical Engineering @ Columbia University | Software Engineering · Systems · ML Infrastructure**

Seeking Summer 2027 Software Engineering / Software Development internships in the United States. Based in New York City.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat&logo=linkedin&logoColor=white)](YOUR_LINKEDIN_URL)
[![Email](https://img.shields.io/badge/Email-Contact-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:YOUR_EMAIL)
[![Resume](https://img.shields.io/badge/Resume-View-4B5563?style=flat&logo=readthedocs&logoColor=white)](YOUR_RESUME_URL)

## About Me

- Pursuing an M.S. in Electrical Engineering at Columbia University.
- Earned a B.S. in Computer Engineering with Honors from the University of Illinois Urbana-Champaign, with an engineering foundation through the ZJU-UIUC Institute at Zhejiang University.
- Focused on software engineering, with additional interests in systems and ML infrastructure.
- Build end-to-end software systems, data pipelines, developer tools, and engineering-oriented ML workflows.
- Seeking Summer 2027 SWE/SDE internship opportunities.

## Tech Stack

**Languages**  
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat&logo=c&logoColor=111111)
![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=flat&logo=cplusplus&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=111111)

**Backend & Web**  
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
![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?style=flat&logo=scipy&logoColor=white)
![Numba](https://img.shields.io/badge/Numba-00A3E0?style=flat&logo=numba&logoColor=white)

**Systems & Tools**  
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=111111)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat&logo=pytest&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=githubactions&logoColor=white)
![Ruff](https://img.shields.io/badge/Ruff-D7FF64?style=flat&logo=ruff&logoColor=111111)
![mypy](https://img.shields.io/badge/mypy-2A6DB2?style=flat)

## Featured Projects

### [StepWise — Wearable Sensor Analytics Platform](https://github.com/xiaorui7/StepWise-Wearable-Sensor-Analytics-Platform)

End-to-end platform that converts plantar-pressure and foot-mounted IMU recordings into structured gait-analysis results, charts, and non-diagnostic HTML reports.

- Implemented a modular pipeline for parsing, calibration, contact detection, stance segmentation, feature extraction, data-quality checks, and explainable rule evaluation.
- Built an asynchronous FastAPI backend with PostgreSQL-backed job state, Redis/RQ workers, persistent artifacts, a React dashboard, and an optional WeChat Mini Program client.
- Added defensive upload handling, deterministic synthetic fixtures, integration and end-to-end tests, and a reproducible five-service Docker Compose environment.

`Python` `FastAPI` `PostgreSQL` `Redis/RQ` `React` `TypeScript` `Docker` `pytest`

### [RISC-V Storage Systems Lab](https://github.com/xiaorui7/riscv-storage-lab)

C and RISC-V teaching operating system running under QEMU, focused on storage correctness, reproducible builds, and measurable block-cache behavior.

- Built source-generated KTFS images, an out-of-source build, a bounded Python test runner, and a matching GitHub Actions workflow.
- Improved cache consistency and failure handling across dirty reads, partial transfers, victim replacement, write retries, and referenced-block flushing.
- Added 20 QEMU storage regression cases, per-cache instrumentation, and deterministic workloads spanning KTFS, the cache layer, I/O abstraction, and VirtIO.

`C` `RISC-V Assembly` `Linux` `QEMU` `VirtIO` `Python` `Make` `GitHub Actions`

### [RAE Feature Compression Benchmark](https://github.com/xiaorui7/rae-feature-compression-benchmark)

Config-driven toolkit for compressing high-dimensional vision representations and evaluating quality, storage, and exact-search trade-offs.

- Built a staged, resumable CLI that extracts pooled features from the official frozen RAE Stage-1 model, then evaluates FP16 storage, PCA, and trainable linear adapters.
- Implemented exact block-wise cosine search, logistic-probe and reconstruction evaluation, validation-only selection, and held-out test auditing.
- Added content-addressed runs, atomic artifacts, manifest validation, provenance hashes, deterministic sample handling, reports, tests, and CPU CI. The upstream RAE model and weights remain external components.

`Python` `PyTorch` `NumPy` `scikit-learn` `matplotlib` `pytest`

### [Accelerated FMCW-SAR Imaging](https://github.com/xiaorui7/accelerated-fmcw-sar)

CPU-based numerical pipeline for simulating FMCW radar sweeps, applying FFT range processing, and reconstructing synthetic-aperture radar images.

- Implemented scalar-reference, chunked NumPy, and parallel Numba back-projection paths with agreement and independent numerical checks.
- Built validated YAML/NPZ interfaces, CLI workflows, controlled motion-error experiments, and isolated-process runtime and memory benchmarks.
- Added unit and integration tests plus cross-platform GitHub Actions coverage for Python 3.11 and 3.13.

`Python` `NumPy` `SciPy` `Numba` `PyYAML` `pytest`

## Education

**Columbia University**  
M.S. in Electrical Engineering

**University of Illinois Urbana-Champaign**  
B.S. in Computer Engineering, with Honors

**Zhejiang University**  
Engineering background through the ZJU-UIUC Institute

## Connect

[LinkedIn](YOUR_LINKEDIN_URL) · [Email](mailto:YOUR_EMAIL) · [Resume](YOUR_RESUME_URL)
