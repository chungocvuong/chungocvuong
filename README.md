<h1 align="center">
  <img src="https://user-images.githubusercontent.com/18350557/176309783-0785949b-9127-417c-8b55-ab5a4333674e.gif" width="28" />
  Hi, I'm Chu Ngoc Vuong
</h1>

<p align="center">
  <b>AI Engineer</b> at NTQ Solution · Hanoi, Vietnam 🇻🇳<br/>
  I build production LLM systems — retrieval, multi-agent pipelines, and the infrastructure that serves them.<br/>
  Researching AI for health, focused on dementia and Alzheimer's disease.
</p>

<p align="center">
  <a href="mailto:chungocvuong3@gmail.com"><img src="https://img.shields.io/badge/Email-chungocvuong3%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
  <a href="https://www.linkedin.com/in/cnv921"><img src="https://img.shields.io/badge/LinkedIn-cnv921-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://aclanthology.org/2025.vlsp-1.45/"><img src="https://img.shields.io/badge/Paper-VLSP%202025%20(ACL)-B31B1B?style=flat-square&logo=googlescholar&logoColor=white" alt="Publication" /></a>
</p>

---

## 👋 About me

I'm an AI engineer with 2 years of production experience, currently at NTQ Solution
in Hanoi. Most of my work sits at the seam between a model and a real system: getting
a model to be *useful* usually has less to do with the model than with the retrieval
layer, the evaluation loop, and the deployment story around it.

- 🔎 Day job: retrieval and tariff-resolution for a US customs classification product
- 🧬 Research: genome-wide association analysis over ADNI Alzheimer's cohorts
- 🇩🇰 Delivered onsite to a Danish client in Copenhagen, then 6 months of direct client work from Vietnam
- 🎓 B.Sc. Computer Science, University of Engineering and Technology — VNU (GPA 3.74/4.00)
- ✉️ **[chungocvuong3@gmail.com](mailto:chungocvuong3@gmail.com)** — open to collaboration on applied AI and AI-for-health work

---

## 📄 Publication

**[Vietnamese–English Medical Domain Machine Translation with LLMs and GRPO Optimization Using Verified Rewards](https://aclanthology.org/2025.vlsp-1.45/)**
Dang Sy Duy, Nguyen Duy Chien, **Chu Ngoc Vuong**
*11th International Workshop on Vietnamese Language and Speech Processing (VLSP 2025)*,
Association for Computational Linguistics, Hanoi, pp. 377–387

Adapted compact open-source LLMs (Qwen 2.5 / Qwen 3, ≤3B params) for English–Vietnamese
medical translation under tight resource constraints — comparing QLoRA continued
pretraining against supervised fine-tuning with GRPO preference alignment, plus
back-translation and a length penalty.

---

## 🔬 Research — AI for health

My research interest is dementia and Alzheimer's disease. Currently building:

- **ADNI GWAS pipeline** — a reproducible genome-wide association workflow over ADNI
  genotype and clinical data: PLINK2 QC → population-structure PCA → logistic/linear
  association → inverse-variance-weighted meta-analysis across cohorts.
- **Data-integrity auditing** — before trusting any result: found that ADNI1 sits on
  genome build hg18 while ADNI2/ADNI3 are hg19 (which quietly invalidates naive
  cross-cohort position matching), and that ~46% of ADNI3 variant IDs are chip-manifest
  names rather than rsIDs.
- **Cohort acquisition tooling** — an ingestion and reporting pipeline for LONI IDA
  neuroimaging cohorts (ADNI, ADNIDOD, ABIDE, ABVIB, AIBL).

Earlier: real-time action classification from live RTSP surveillance streams, with
semi-supervised cross-model pseudo-labeling — Human-Machine Interface Lab, UET.

---

## 🛠️ What I've built

Client and employer work, so the repositories are private — but this is the shape of it.

| System | What it does |
| --- | --- |
| **HTS code search & classification** | Classifies free-text product descriptions into 10-digit US tariff codes. Hybrid BM25 + kNN over OpenSearch merged by weighted RRF, an LLM chapter pre-selector at ~99% top-3 recall, and country-of-origin duty resolution across GSP/AGOA/CAFTA-DR/USMCA preference programs. |
| **Agentic business documentation** | Replaced a hand-written BA documentation process with a 12-agent pipeline turning user stories or source code into structured business and API docs — with quality gates, conflict detection, and a bounded revision loop before human escalation. |
| **AI knowledge management (RAG)** | The platform that won its client engagement. Multi-format document ingestion, Celery/RabbitMQ async processing, hybrid search with reranking over Qdrant, and multilingual prompting across EN/JA/KO/VI. |
| **GraphRAG for technical docs** | Owned the data layer end to end — chunking, AI summaries, embeddings, and the linkage between a Neo4j knowledge graph and its Elasticsearch vector chunks, so retrieval could follow entity relationships rather than text similarity alone. |

---

## 🧰 Tech stack

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)

**LLM & ML**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)

`RAG` · `GraphRAG` · `hybrid search (BM25 + kNN, RRF)` · `reranking` · `multi-agent pipelines` · `QLoRA` · `SFT` · `GRPO / preference alignment` · `evaluation harnesses`

**Search & data**

![OpenSearch](https://img.shields.io/badge/OpenSearch-005EB8?style=flat-square&logo=opensearch&logoColor=white)
![Elasticsearch](https://img.shields.io/badge/Elasticsearch-005571?style=flat-square&logo=elasticsearch&logoColor=white)
![Qdrant](https://img.shields.io/badge/Qdrant-DC244C?style=flat-square&logo=qdrant&logoColor=white)
![Neo4j](https://img.shields.io/badge/Neo4j-4581C3?style=flat-square&logo=neo4j&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)

**Backend & infra**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Celery](https://img.shields.io/badge/Celery-37814A?style=flat-square&logo=celery&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=flat-square&logo=rabbitmq&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![GitLab CI](https://img.shields.io/badge/GitLab%20CI-FC6D26?style=flat-square&logo=gitlab&logoColor=white)

---

## 🏆 Achievements

- 🥇 **1st Place** — ImageCLEFmed MEDIQA-CORE 2026, Brain Tumor Subtype Classification
- 🥇 **1st Place** — Robotics Challenge 2023, Chiba Institute of Technology, Japan
- 🎖️ **Vietcombank Scholarship** for outstanding academic achievement
- 🎖️ **University Scholarship** for academic excellence — semesters II, VI, VIII

---

## 📊 GitHub activity

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=chungocvuong&show_icons=true&hide_border=true&include_all_commits=true&count_private=true&theme=transparent" alt="GitHub stats" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=chungocvuong&layout=compact&hide_border=true&langs_count=8&theme=transparent" alt="Top languages" />
</p>

---

## 🤝 Get in touch

<p align="left">
  <a href="mailto:chungocvuong3@gmail.com" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/socials/gmail.svg" width="32" height="32" alt="Email" /></a>
  <a href="https://www.linkedin.com/in/cnv921" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/socials/linkedin.svg" width="32" height="32" alt="LinkedIn" /></a>
  <a href="https://www.facebook.com/chuvuong2910" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/socials/facebook.svg" width="32" height="32" alt="Facebook" /></a>
  <a href="http://www.instagram.com/du.trg" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/socials/instagram.svg" width="32" height="32" alt="Instagram" /></a>
</p>
