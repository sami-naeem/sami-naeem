## Hi there, I'm Sami! 👋


- Design Multi Agent AI systems that reason and execute, orchestrated across tools
- Apply RAG, LLMs, MCPs and Embeddings for intelligent AI systems
- Productionize 

- 🧠 Focused on **[AREA OF FOCUS]**
- 💬 Ask me about **[TOPIC]**

---

## 🔭 My Work

### 🤖 Autonomous Quantitative Investment Research with Agentic AI

🏆 **2nd Place, UChicago MS Applied Data Science Capstone Showcase (2026)**

Built a multi-agent AI system that **autonomously reads quantitative finance research papers and replicates their investment strategies**, automating a process that typically requires a highly trained human analyst.

**Key Capabilities**

- Six specialized agents orchestrated with LangGraph to read, reason over, and implement trading strategies from academic papers.
- LLaMA fine-tuned with QLoRA on ~3,000 finance academic research papers.
- RAG pipeline over a Qdrant vector store for grounded retrieval of quantitative finance domain knowledge.
- GPU training and inference infrastructure on GCP and Lambda AI.

**Impact**

- Nearly **doubled accuracy over the out-of-the-box model** — 43% vs. 23% win rate in blind evaluations against 50 expert-verified benchmarks.
- Outperformed leading AI models from OpenAI, Anthropic, and Google in **55% of head-to-head comparisons**.
- Delivered a **10× productivity gain at 1/3 the cost** of a human researcher.

**Stack** Python · LangGraph · LLaMA/QLoRA · RAG (Qdrant) · GCP/GPU Infrastructure · Lambda AI

---

### 🎲 [Bayesian MCMC Hierarchical Portfolio Construction Model](https://github.com/sami-naeem/Bayesian-Investment-Portfolio-Construction)

Built a proprietary Bayesian Hierarchical MCMC portfolio construction model — **unavailable in any commercial robo-advisor** — that samples the full probability distribution of returns and correlations across 9 asset classes, embedding investment uncertainty directly into the allocation.

**Key Capabilities**

- MCMC sampling of the joint posterior of returns and covariance with PyMC (4 chains × 4,000 iterations).
- Hierarchical asset grouping (9 asset classes → 4 groups) to reduce overfitting.
- LKJ-Cholesky priors that encode investor views directly on cross-asset correlations, extending Black-Litterman beyond expected returns into the full covariance structure.
- Student-t distribution to capture market crashes and fat-tailed return behavior.
- Three optimizers run over the sampled posterior: Mean-Variance, Maximum Sharpe, and CVaR (direct tail-risk targeting) via CVXPY.

**Impact**

- Backtested over 6 years (2019–2024) against Morningstar static and Monte Carlo benchmarks.
- The Bayesian CVaR portfolio returned **26.87% — nearly 4× the Monte Carlo equivalent** and ahead of Morningstar's conservative benchmark (23.89%).

**Stack** Python · PyMC · CVXPY · ArviZ · NumPy/SciPy · yfinance

---

### 📷 [BMI Estimation from Facial Images](https://github.com/sami-naeem/BMI-Estimation-From-Facial-Images-CompVision)

Replicated and extended a 2017 computer vision research paper, predicting **Body Mass Index directly from facial photographs** for non-invasive health screening.

**Key Capabilities**

- Two-stage architecture: fine-tuned EfficientNetB3 feature extractor (1,536-dim embeddings) feeding a regression ensemble of Random Forest, Ridge, and CatBoost.
- Screened all eight EfficientNet variants (B0–B7) and selected B3 as the best accuracy-vs-compute trade-off.
- Trained on the VisualBMI dataset (3,962 facial images) with augmentation and a subject-disjoint train/test protocol.
- Exported an 11.7 MB TensorFlow Lite model for lightweight deployment.

**Impact**

- Achieved a **Pearson r of 0.67 (MAE 4.72), surpassing the reference paper's best result (0.65)**.
- Reduced the original paper's gender performance gap — 0.69/0.65 male/female correlation vs. the original 0.71/0.57.

**Stack** TensorFlow/Keras · EfficientNet · scikit-learn · CatBoost · XGBoost · LightGBM · TensorFlow Lite

---

## 🛠️ Tech Stack

### Languages

![Python](https://img.shields.io/badge/Python-0D1117?style=for-the-badge&logo=python) ![SQL](https://img.shields.io/badge/SQL-0D1117?style=for-the-badge&logo=postgresql) ![MySQL](https://img.shields.io/badge/MySQL-0D1117?style=for-the-badge&logo=mysql) ![CUDA](https://img.shields.io/badge/CUDA-0D1117?style=for-the-badge&logo=nvidia) ![Bash](https://img.shields.io/badge/Bash-0D1117?style=for-the-badge&logo=gnubash) ![R](https://img.shields.io/badge/R-0D1117?style=for-the-badge&logo=r)

### ML & AI

- **Agent Frameworks** ![LangChain](https://img.shields.io/badge/LangChain-0D1117?style=for-the-badge&logo=langchain&logoColor=white) ![LangGraph](https://img.shields.io/badge/LangGraph-0D1117?style=for-the-badge) ![LangSmith](https://img.shields.io/badge/LangSmith-0D1117?style=for-the-badge&logo=langchain&logoColor=white)
- **Deep Learning** ![PyTorch](https://img.shields.io/badge/PyTorch-0D1117?style=for-the-badge&logo=pytorch) ![TensorFlow](https://img.shields.io/badge/TensorFlow-0D1117?style=for-the-badge&logo=tensorflow) ![Keras](https://img.shields.io/badge/Keras-0D1117?style=for-the-badge&logo=keras) ![JAX](https://img.shields.io/badge/JAX-0D1117?style=for-the-badge)
- **NLP** ![Hugging Face](https://img.shields.io/badge/Hugging%20Face-0D1117?style=for-the-badge&logo=huggingface) ![sentence-transformers](https://img.shields.io/badge/sentence--transformers-0D1117?style=for-the-badge&logo=huggingface) ![rank-bm25](https://img.shields.io/badge/rank--bm25-0D1117?style=for-the-badge)
- **Time Series & Financial Modeling** ![statsmodels](https://img.shields.io/badge/statsmodels-0D1117?style=for-the-badge) ![arch/GARCH](https://img.shields.io/badge/arch%2FGARCH-0D1117?style=for-the-badge) ![TimeGPT](https://img.shields.io/badge/TimeGPT-0D1117?style=for-the-badge) ![Mamba](https://img.shields.io/badge/Mamba-0D1117?style=for-the-badge)
- **Data Manipulation & Machine Learning** ![Pandas](https://img.shields.io/badge/Pandas-0D1117?style=for-the-badge&logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/NumPy-0D1117?style=for-the-badge&logo=numpy&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-0D1117?style=for-the-badge&logo=scikitlearn) ![LightGBM](https://img.shields.io/badge/LightGBM-0D1117?style=for-the-badge) ![FLAML](https://img.shields.io/badge/FLAML-0D1117?style=for-the-badge)
- **Computer Vision** ![OpenCV](https://img.shields.io/badge/OpenCV-0D1117?style=for-the-badge&logo=opencv)

### Cloud & Platform

![AWS](https://img.shields.io/badge/AWS-0D1117?style=for-the-badge&logo=amazonwebservices&logoColor=white) ![GCP](https://img.shields.io/badge/GCP-0D1117?style=for-the-badge&logo=googlecloud) ![Vertex AI](https://img.shields.io/badge/Vertex%20AI-0D1117?style=for-the-badge&logo=googlecloud) ![Azure](https://img.shields.io/badge/Azure-0D1117?style=for-the-badge) ![Snowflake](https://img.shields.io/badge/Snowflake-0D1117?style=for-the-badge&logo=snowflake) ![Databricks](https://img.shields.io/badge/Databricks-0D1117?style=for-the-badge&logo=databricks) ![MongoDB](https://img.shields.io/badge/MongoDB-0D1117?style=for-the-badge&logo=mongodb) ![Neo4j](https://img.shields.io/badge/Neo4j-0D1117?style=for-the-badge&logo=neo4j)

### ML Ops

![Docker](https://img.shields.io/badge/Docker-0D1117?style=for-the-badge&logo=docker) ![Kubernetes](https://img.shields.io/badge/Kubernetes-0D1117?style=for-the-badge&logo=kubernetes) ![MLflow](https://img.shields.io/badge/MLflow-0D1117?style=for-the-badge&logo=mlflow) ![Git](https://img.shields.io/badge/Git-0D1117?style=for-the-badge&logo=git) ![GitHub](https://img.shields.io/badge/GitHub-0D1117?style=for-the-badge&logo=github&logoColor=white) ![DVC](https://img.shields.io/badge/DVC-0D1117?style=for-the-badge&logo=dvc) ![Qdrant](https://img.shields.io/badge/Qdrant-0D1117?style=for-the-badge) ![Evidently](https://img.shields.io/badge/Evidently-0D1117?style=for-the-badge) ![joblib](https://img.shields.io/badge/joblib-0D1117?style=for-the-badge)

### Web App & API Frameworks

![Streamlit](https://img.shields.io/badge/Streamlit-0D1117?style=for-the-badge&logo=streamlit) ![FastAPI](https://img.shields.io/badge/FastAPI-0D1117?style=for-the-badge&logo=fastapi) ![Pydantic](https://img.shields.io/badge/Pydantic-0D1117?style=for-the-badge&logo=pydantic) ![Uvicorn](https://img.shields.io/badge/Uvicorn-0D1117?style=for-the-badge&logo=gunicorn) ![React](https://img.shields.io/badge/React-0D1117?style=for-the-badge&logo=react)