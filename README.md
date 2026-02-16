### Hi, I'm Michal Roubalík.

**Quant Developer | Mathematical Optimization (MILP) | PhD in Power Engineering**

I specialize in building high-performance optimization engines and data pipelines for the energy and financial sectors. My work focuses on translating complex mathematical formulations (MILP, Stochastic Modeling, ODE/PDE) into production-grade software using **Python** and **C++**.

Currently bridging the gap between **Scientific Computing** and **DevOps** (Docker, OpenShift).

---

### 🛠️ Core Engineering Stack
* **Languages:** Python (Advanced), C++, SQL
* **Quant & Math:** NumPy, SciPy, Pandas, PyMC, Scikit-learn, XGBoost
* **Optimization:** PuLP (MILP), CVaR Constraints, Dynamic Programming
* **Infrastructure:** Docker, Kubernetes/OpenShift, CI/CD (GitHub Actions), Parquet/Snappy

---

### 🚀 Quantitative Research

#### 📈 [OptiAlpha: Bayesian Stochastic Portfolio Optimization](https://github.com/michal-roubalik/OptiAlpha)
![Status](https://img.shields.io/badge/Status-Research_Prototype-orange?style=flat-square)
* **What:** A framework for constructing **Market Neutral** portfolios by bridging probabilistic modeling with constrained optimization. It generates alpha distributions rather than point estimates to manage tail risk.
* **Methodology:**
    * **Alpha Generation:** Analytical Bayesian Linear Regression (`BayesianRidge`) on rolling momentum signals.
    * **Optimization:** Stochastic MILP solver maximizing expected alpha subject to **CVaR (95%)** constraints.
* **Key Result:** Achieves robust risk-adjusted returns by dynamically shifting exposure between Long/Short based on posterior uncertainty width.
* **Tech:** `yfinance`, `PyMC`, `PuLP`, `BayesianRidge`.

#### 📊 [LOB-Alpha-ML: High-Frequency Order Book Forecasting](https://github.com/michal-roubalik/LOB-Alpha-ML)
![Status](https://img.shields.io/badge/Status-ML_Research-blue?style=flat-square)
* **What:** An event-driven research framework predicting directional price movements in crypto markets using **Limit Order Book (LOB)** microstructure features.
* **Microstructure Theory:**
    * **Order Book Imbalance (OBI):** $OBI_t = (V^b_t - V^a_t) / (V^b_t + V^a_t)$
    * **Micro-Price:** Volume-weighted price estimates that adjust for liquidity asymmetries.
* **Key Result:** A weighted **XGBoost** classifier validated via Walk-Forward splitting demonstrated a statistically significant predictive edge over random walk benchmarks.
* **Tech:** `XGBoost`, `Parquet` (Snappy), `Pandas`.

---

### ⚡ Engineering & Optimization

#### 🔋 [Volt-Optimizer: BESS Arbitrage Framework](https://github.com/michal-roubalik/Volt-Optimizer)
[![Live Demo](https://img.shields.io/badge/Render-Live_Demo-00d1b2?style=flat-square&logo=render)](https://volt-frontend-f95q.onrender.com/)
* **What:** A full-stack MILP dispatch engine for Battery Energy Storage Systems (BESS) that optimizes arbitrage against Day-Ahead market prices and local solar generation.
* **Architecture:** Microservices pattern with **NDJSON streaming** for real-time solver telemetry.
* **Key Feature:** Solves high-dimensional constraints (round-trip efficiency $\eta$, degradation) in real-time.
* **Tech:** `FastAPI`, `Docker`, `PuLP`, `Plotly.js`.

#### 📡 [SignalParallel: High-Throughput Processing Engine](https://github.com/michal-roubalik/SignalParallel)
![Status](https://img.shields.io/badge/Status-Complete-green?style=flat-square)
* **What:** A benchmarking pipeline for parallel signal processing (FFT, Butterworth filtering) designed to measure Python's multiprocessing overhead.
* **Key Finding:** Identified the **"Windows Tax"**—a ~2.0s fixed startup cost for process pools. Parallelization only yields efficiency gains for signal batches exceeding **500 seconds** in duration.
* **Tech:** `Multiprocessing`, `SciPy Signal`, `Welch’s Method`.

---

[<img src="https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin">](https://www.linkedin.com/in/michal-roubalik/)
