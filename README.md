<div align="center">

# Avikal Singh

### AI Engineer · AWS Certified Data Engineer · MS Information Science (ML)

*Building production AI systems on top of battle-tested data infrastructure*

[![Portfolio](https://img.shields.io/badge/Portfolio-avikalsingh.vercel.app-black?style=flat-square&logo=vercel)](https://avikalsingh.vercel.app/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-avikal--singh-0A66C2?style=flat-square&logo=linkedin)](https://linkedin.com/in/avikal-singh-079ab8184)
[![AWS Certified](https://img.shields.io/badge/AWS-Data%20Engineer%20Associate-FF9900?style=flat-square&logo=amazon-aws)](https://cp.certmetrics.com/amazon/en/public/verify/credential/6abbddad866a45fa92a00e21605a4ceb)
[![Email](https://img.shields.io/badge/Email-avikalgangwar1@gmail.com-EA4335?style=flat-square&logo=gmail)](mailto:avikalgangwar1@gmail.com)

</div>

---

## About

I build AI systems end-to-end — from raw data ingestion to model inference to agentic workflows — and I care about what happens to the data before it reaches the model.

Most AI engineers treat infrastructure as someone else's problem. I don't. My background spans multimodal ML (published at SPIE Medical Imaging), real-time streaming pipelines (Azure EventHub → Databricks → Delta Lake), and LLM-powered agentic systems — all built on production-grade data foundations.

**Current focus:** Healthcare AI, agentic systems with RAG + tool calling, and LLM fine-tuning under resource constraints (PEFT/LoRA, 4-bit quantization).

---

## Featured Projects

### 🫁 Multimodal Chest X-Ray AI — Radiology Report Generation & Pathology Classification
*PyTorch · Hugging Face · BiomedCLIP · Meditron-7B · Clinical-T5 · MedLLaMA · PEFT/LoRA · CUDA/DDP*

Production-scale multimodal AI system on 119,533 MIMIC-CXR records. Built for two simultaneous clinical tasks: generate free-text radiology reports from chest X-rays, and classify 14-label pathology findings under severe class imbalance.

**What makes this non-trivial:**
- Designed a CLS-conditioned cross-attention abstractor that compresses 197 ViT tokens → 32 query tokens, enabling efficient vision-language fusion while training only 73M of 3.6B parameters
- Applied PEFT/LoRA + 4-bit NF4 quantization + CUDA/DDP — full-scale training on constrained hardware without sacrificing model capability
- Engineered clinical preprocessing with OpenCV CLAHE, schema validation, deduplication, label normalization, and patient-stratified splits to prevent data leakage across train/val/test
- Built threshold-tuning workflows with AUROC, F1, BLEU-4, METEOR, and ROUGE-L; achieved **0.830 micro-AUROC** and improved rare-class sensitivity by **70.88%**

**Research output:** Accepted abstract at SPIE Medical Imaging (peer-reviewed)

---

### 🚖 Agentic Ride-Hailing Analytics Assistant — Real-Time AI + Streaming Infrastructure
*Gemini APIs · LangChain · RAG · Azure EventHub/Kafka · Databricks DLT · Spark/PySpark · Delta Lake · Unity Catalog · Streamlit*

[![GitHub](https://img.shields.io/badge/GitHub-Repo-181717?style=flat-square&logo=github)](https://github.com/avikalsingh/Uber-Data-Engineering-Project-with-Azure-Databricks)

A natural-language analytics assistant built on top of a production real-time streaming pipeline. Ask questions about pricing, demand, city-level KPIs — the agent retrieves, reasons, and answers against live data.

**Pipeline architecture:**
- Real-time ingestion of ride events across 40 US cities via **Azure EventHub** (Kafka-compatible)
- **Databricks Delta Live Tables** with Medallion Architecture (Bronze → Silver → Gold), Star Schema, SCD Type 1/2, Unity Catalog
- Partition tuning cut DLT execution from 6–8 min → **75 seconds** (85% reduction)
- Azure Key Vault for SAS key rotation; Python SDK for automated EventHub lifecycle management

**Agentic layer:**
- Gemini APIs + LangChain-style orchestration with RAG, tool calling, and MCP-style tool interfaces
- Structured JSON outputs, prompt validation, and self-healing pipeline checks for schema drift and failed transformations
- Streamlit dashboard with KPIs, Plotly visualizations, and Folium heatmap for city-level demand

---

### 🏠 Airbnb Analytics Pipeline — AWS · Snowflake · dbt
*AWS S3 · Snowflake · dbt Core · Streamlit*

[![GitHub](https://img.shields.io/badge/GitHub-Repo-181717?style=flat-square&logo=github)](https://github.com/avikalsingh/AirBnb_Data_Engineer_Project_with_Snowflake_DBT)
[![Live App](https://img.shields.io/badge/Live-Streamlit%20App-FF4B4B?style=flat-square&logo=streamlit)](https://airbnbwithdbt.streamlit.app/)

ELT pipeline with IAM-authenticated S3 → Snowflake external stages, dbt Core transformations (Jinja macros, SCD Type 2 snapshots, schema tests), and Medallion Architecture (Bronze → Silver → Gold). Live Streamlit dashboard covering pricing, occupancy, and host metrics.

---

## Stack

```
AI / ML         PyTorch · Hugging Face · BiomedCLIP · Meditron-7B · Clinical-T5 · MedLLaMA
                PEFT/LoRA · 4-bit NF4 · CUDA/DDP · scikit-learn · XGBoost · OpenCV

Agentic / LLM   LangChain · RAG · Tool Calling · MCP-style Interfaces · Gemini/GPT APIs
                Structured JSON Outputs · Agent Routing · Self-Healing Workflows

Data Eng        Apache Spark/PySpark · Databricks DLT · Delta Lake · Unity Catalog
                dbt Core (Jinja macros, SCD Type 2, schema tests) · Apache Airflow
                Snowflake · AWS (S3, Redshift, Glue) · Azure (EventHub, Data Factory, Key Vault)
                Medallion Architecture · Dimensional Modeling

Backend         FastAPI · Flask · REST APIs · PostgreSQL · MySQL · Docker · GitHub Actions CI/CD

Visualization   Streamlit · Plotly · Folium · Tableau · Power BI

Languages       Python (pandas, NumPy, PySpark) · SQL · R · Bash
```

---

## Experience Highlights

**AI Engineer — Vision Systems & Intelligence Labs** *(Jan 2025 – Present)*
Multimodal healthcare AI on 119,533 MIMIC-CXR records. Fine-tuned medical LLMs under hardware constraints. Published at SPIE Medical Imaging.

**Data Engineer — Center for Railways Information System** *(Dec 2021 – Jul 2023)*
ETL pipelines over 1M+ records. 45% query latency reduction via MySQL rewrites, composite indexing, and table partitioning. Eliminated 8 hrs/week manual reconciliation. Docker + GitHub Actions CI/CD cut deployment from 2–3 weeks to under 2 days.

---

## Certification

**[AWS Certified Data Engineer – Associate (DEA-C01)](https://cp.certmetrics.com/amazon/en/public/verify/credential/6abbddad866a45fa92a00e21605a4ceb)** — Amazon Web Services · June 2025

---

## Education

**MS, Information Science – Machine Learning** · University of Arizona · 3.89 GPA · 2023–2025

---

<div align="center">

*San Antonio, TX · Open to AI Engineer, ML Engineer, and Data Engineering roles*
*Requires H-1B sponsorship*

</div>
