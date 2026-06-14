<p align="center">
<img src="https://github.com/sami-naeem/Images_For_ReadMe/blob/main/readme_header.jpg" alt="Header" />
</p>

<p align="center">
<a href="https://git.io/typing-svg"><img src="https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1000&center=true&random=false&width=825&lines=Hey+there%2C+welcome+to+my+GitHub" alt="Typing SVG" /></a>
</p>

# Hi, I'm Sami 👋

**AI Product Manager.** 8+ years of experience building the **#2 robo-advisor in the US** ($190B+ AUM/AUA · 1.7M+ investors) at Morningstar, now pairing that domain depth with an **MS in Applied Data Science (University of Chicago, 2026)** to build agentic AI for wealth management.

<h3 align="left">Connect with me:</h3>
<p align="left">
<a href="https://linkedin.com/in/saminaeem" target="blank"><img align="center" src="https://github.com/sami-naeem/Images_For_ReadMe/blob/main/linkedin.png" alt="saminaeem" height="40" width="40" /></a>
</p>

---

## 👤 About Me

I'm a product manager who refuses the usual trade between domain expertise and technical depth:

- 🏦 **Wealth management, end to end.** 6 roles and 4 promotions at Morningstar: from operations to building $3B+ institutional portfolios to product.
- 🤖 **AI I build myself.** Multi-agent systems (LangGraph), LLM fine-tuning (QLoRA), RAG pipelines (Qdrant). Implemented and evaluated, not just scoped.
- 📊 **PM operating record.** Led teams of 9 to 11 engineers, shipped products zero to one, and drove ML initiatives that cut churn 8.9% and lifted engagement 27.8%.

---

## 🔭 Featured Work

### 🤖 Autonomous Quantitative Investment Research with Agentic AI

🏆 **2nd Place, UChicago MS Applied Data Science Capstone Showcase (2026)**

At quantitative hedge funds, finding new investment strategies means reading hundreds of academic papers, extracting the key ideas, building the underlying signals, and backtesting them. It is the most labor-intensive part of a quant researcher's job. We built an AI system that does it autonomously.

**How it works:** Seven specialized AI agents work in sequence — one reads and classifies the paper, the next extracts the investment logic, the next maps it to real financial data, and the final agents write executable code and run a backtest. The agents are built with LangGraph and powered by a custom version of LLaMA we fine-tuned on ~3,000 quantitative finance papers.

**Results across 150 blind evaluations on 50 expert-curated papers:**

- The multi-agent pipeline **outperformed single-pass calls to GPT-4o, Claude, and Gemini in 55% of head-to-head matchups** — winning on quality of output, not just speed
- Our fine-tuned LLaMA **nearly doubled the base model's accuracy** on extracting investment logic (43% win rate vs. 23% for the base model)
- The system replicates ~2 papers per day vs. a human baseline of 2 per week — an estimated **10× productivity gain at 1/3 the cost** (~$50K/yr vs. ~$150K/yr for an entry-level quant researcher)

**Stack:** Python · LangGraph · LLaMA 3.1-8B · QLoRA · RAG (Qdrant) · GCP · Lambda AI

---

### 🎲 [Bayesian Hierarchical MCMC Portfolio Construction](https://github.com/sami-naeem/Bayesian-Investment-Portfolio-Construction)

Built a proprietary Bayesian Hierarchical MCMC portfolio construction model — unavailable in any commercial robo-advisor — that samples the full probability distribution of returns and correlations across 9 asset classes, embedding investment uncertainty directly into the allocation.

**How it works:** Instead of a single point estimate, the model runs MCMC sampling (4 chains × 4,000 iterations) to generate thousands of plausible futures for returns and cross-asset correlations. LKJ-Cholesky priors let investors encode their own views directly on those correlations — extending the classic Black-Litterman framework beyond expected returns into the full covariance structure. Student-t return distributions capture fat tails, so the model accounts for crashes rather than being blindsided by them. Assets are grouped hierarchically (9 classes → 4 groups) to reduce overfitting.

**Three optimizers run over the sampled posterior:**
- **Mean-Variance (MVO):** Maximize expected return for a given level of risk
- **Maximum Sharpe Ratio:** Maximize return per unit of risk taken
- **CVaR (Conditional Value at Risk):** Minimize expected loss in the worst-case scenarios — the strategy built to hold up in bad markets

**Backtested 2019 to 2024 against Morningstar benchmarks:**

- The CVaR portfolio returned **26.87%**, nearly 4× Morningstar's comparable benchmark (7.3%) and ahead of their conservative model (23.89%)
- The investor tilt feature — encoding views via LKJ-Cholesky priors — allows the model to reflect active conviction without abandoning probabilistic discipline

**Stack:** Python · PyMC · CVXPY · ArviZ · NumPy/SciPy · yfinance

---

### 📷 [BMI Estimation from Facial Images](https://github.com/sami-naeem/BMI-Estimation-From-Facial-Images-CompVision)

A non-invasive health screening tool: given a single photo of someone's face, the model estimates their Body Mass Index. Built to replicate and improve on a 2017 peer-reviewed paper from AAAI.

**How it works:** A deep learning model first extracts facial features from the image (using EfficientNetB3, selected after testing all eight variants for the best accuracy-to-compute trade-off). Those features are then passed to an ensemble of three regression models that produce the final BMI estimate. The whole model is compressed to 11.7 MB for lightweight deployment on mobile or edge devices.

**Results on 3,962 facial images:**

- Correlation of **r = 0.67**, beating the original paper's best result of 0.65
- Narrowed the gender performance gap the original paper left open: 0.69/0.65 (male/female) vs. the paper's 0.71/0.57
- Average prediction error of 4.72 BMI points

**Stack:** TensorFlow/Keras · EfficientNet · scikit-learn · CatBoost · TensorFlow Lite

---

## 🗂️ More Projects

| Project | What it is | Stack |
|---|---|---|
| [Market Fear & Greed Classifier](https://github.com/sami-naeem/Market-Fear-Greed-Indicator) | Production-grade MLOps pipeline classifying market sentiment (Fear / Stable / Greed) from VIX with 91.4% accuracy: feature store, AutoML, cloud deployment, and drift monitoring | GCP Vertex AI · FLAML · DVC · Evidently |
| [KSE-100 Equity Forecasting](https://github.com/sami-naeem/Pakistan_Stock_Market_Prediction) | Decoupled Signal + Risk engine for 30-day index forecasting on the Pakistan Stock Exchange | Mamba · TimeGPT · SARIMAX · GARCH |
| [Headline Sentiment Analysis](https://github.com/sami-naeem/Newspaper-Headline-Sentiment-Analysis-Model) | Full-stack NLP classifier shipping three interfaces: Streamlit UI, FastAPI REST API, and CLI batch scoring | sentence-transformers · SVM · FastAPI · Streamlit |

---

## 🛠️ Tech Stack

**Languages**

![Python](https://img.shields.io/badge/Python-0D1117?style=for-the-badge&logo=python) ![SQL](https://img.shields.io/badge/SQL-0D1117?style=for-the-badge&logo=postgresql) ![MySQL](https://img.shields.io/badge/MySQL-0D1117?style=for-the-badge&logo=mysql) ![CUDA](https://img.shields.io/badge/CUDA-0D1117?style=for-the-badge&logo=nvidia) ![Bash](https://img.shields.io/badge/Bash-0D1117?style=for-the-badge&logo=gnubash)

**Agentic AI & NLP**

![LangGraph](https://img.shields.io/badge/LangGraph-0D1117?style=for-the-badge) ![LangChain](https://img.shields.io/badge/LangChain-0D1117?style=for-the-badge&logo=langchain&logoColor=white) ![LangSmith](https://img.shields.io/badge/LangSmith-0D1117?style=for-the-badge&logo=langchain&logoColor=white) ![Hugging Face](https://img.shields.io/badge/Hugging%20Face-0D1117?style=for-the-badge&logo=huggingface) ![sentence-transformers](https://img.shields.io/badge/sentence--transformers-0D1117?style=for-the-badge&logo=huggingface) ![Qdrant](https://img.shields.io/badge/Qdrant-0D1117?style=for-the-badge) ![rank-bm25](https://img.shields.io/badge/rank--bm25-0D1117?style=for-the-badge)

**ML & Deep Learning**

![PyTorch](https://img.shields.io/badge/PyTorch-0D1117?style=for-the-badge&logo=pytorch) ![TensorFlow](https://img.shields.io/badge/TensorFlow-0D1117?style=for-the-badge&logo=tensorflow) ![Keras](https://img.shields.io/badge/Keras-0D1117?style=for-the-badge&logo=keras) ![JAX](https://img.shields.io/badge/JAX-0D1117?style=for-the-badge) ![scikit-learn](https://img.shields.io/badge/scikit--learn-0D1117?style=for-the-badge&logo=scikitlearn) ![LightGBM](https://img.shields.io/badge/LightGBM-0D1117?style=for-the-badge) ![FLAML](https://img.shields.io/badge/FLAML-0D1117?style=for-the-badge) ![OpenCV](https://img.shields.io/badge/OpenCV-0D1117?style=for-the-badge&logo=opencv)

**Quant & Time Series**

![PyMC](https://img.shields.io/badge/PyMC-0D1117?style=for-the-badge) ![CVXPY](https://img.shields.io/badge/CVXPY-0D1117?style=for-the-badge) ![statsmodels](https://img.shields.io/badge/statsmodels-0D1117?style=for-the-badge) ![arch/GARCH](https://img.shields.io/badge/arch%2FGARCH-0D1117?style=for-the-badge) ![TimeGPT](https://img.shields.io/badge/TimeGPT-0D1117?style=for-the-badge) ![Mamba](https://img.shields.io/badge/Mamba-0D1117?style=for-the-badge)

**Cloud, Data & MLOps**

![GCP](https://img.shields.io/badge/GCP-0D1117?style=for-the-badge&logo=googlecloud) ![Vertex AI](https://img.shields.io/badge/Vertex%20AI-0D1117?style=for-the-badge&logo=googlecloud) ![AWS](https://img.shields.io/badge/AWS-0D1117?style=for-the-badge&logo=amazonwebservices&logoColor=white) ![Azure](https://img.shields.io/badge/Azure-0D1117?style=for-the-badge) ![Docker](https://img.shields.io/badge/Docker-0D1117?style=for-the-badge&logo=docker) ![Git](https://img.shields.io/badge/Git-0D1117?style=for-the-badge&logo=git) ![DVC](https://img.shields.io/badge/DVC-0D1117?style=for-the-badge&logo=dvc) ![Evidently](https://img.shields.io/badge/Evidently-0D1117?style=for-the-badge) ![Snowflake](https://img.shields.io/badge/Snowflake-0D1117?style=for-the-badge&logo=snowflake) ![Databricks](https://img.shields.io/badge/Databricks-0D1117?style=for-the-badge&logo=databricks) ![MongoDB](https://img.shields.io/badge/MongoDB-0D1117?style=for-the-badge&logo=mongodb)

**Apps & APIs**

![FastAPI](https://img.shields.io/badge/FastAPI-0D1117?style=for-the-badge&logo=fastapi) ![Pydantic](https://img.shields.io/badge/Pydantic-0D1117?style=for-the-badge&logo=pydantic) ![Streamlit](https://img.shields.io/badge/Streamlit-0D1117?style=for-the-badge&logo=streamlit) ![Uvicorn](https://img.shields.io/badge/Uvicorn-0D1117?style=for-the-badge&logo=gunicorn)

**Product & Certifications**

![CSPO](https://img.shields.io/badge/Certified%20Scrum%20Product%20Owner-0D1117?style=for-the-badge) ![CSM](https://img.shields.io/badge/Certified%20ScrumMaster-0D1117?style=for-the-badge) ![CFA](https://img.shields.io/badge/CFA%20Level%201-0D1117?style=for-the-badge)
