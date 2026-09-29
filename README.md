<!--
  Profile README for github.com/kartikey05
  STABLE sections: header, intro, focus areas, how I build   -> review yearly
  EVOLVING sections: now, selected work, writing, open source -> review every 6 months
  Placeholders are written as ALL_CAPS or live inside HTML comments. Search for "TODO" before publishing.
-->

<h1 align="center">Kartikey Agarwal</h1>

<p align="center">
  <b>Applied AI and ML engineering, from models to production systems</b>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/kartikeyagarwal08/">LinkedIn</a>
  <!-- TODO: uncomment the links you actually have -->
  <!-- · <a href="https://PORTFOLIO_URL">Portfolio</a> -->
  <!-- · <a href="https://BLOG_URL">Writing</a> -->
  <!-- · <a href="mailto:YOUR_EMAIL">Email</a> -->
</p>

---

I build AI systems that turn messy, unstructured data into output other software can rely on. My work sits where machine learning meets software engineering: adapting and evaluating models, building retrieval and agent workflows, and running them behind services that are fast, observable and safe to operate.

Much of my work so far has been in healthcare, extracting structured clinical information from documents. In that domain a wrong answer is expensive, so I care about evaluation, validation and failure handling as much as model quality.

### What I work on

| Area | Focus |
|---|---|
| **Language model systems** | Fine-tuning (LoRA / PEFT), structured generation, evaluation |
| **Retrieval and knowledge** | Embeddings, vector search, entity and terminology mapping, knowledge graphs |
| **Agentic workflows** | Multi-step reasoning, orchestration, validation layers, human-in-the-loop review |
| **Serving and systems** | Efficient inference, async APIs, task queues, observability |
| **ML foundations** | NLP, deep learning, classical ML, data pipelines |

### Now
<!-- EVOLVING: update every 6 months. Keep to 2–3 lines. -->
- Building LLM systems for clinical document understanding and medical coding in industry
- Exploring: <!-- TODO: e.g. inference optimisation, evaluation methods, agent protocols -->

### Toolbox
<!-- Add or remove one badge per line. Logos come from simpleicons.org; if a slug doesn't exist the badge still renders, just without a logo. -->

**Core** &nbsp;
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)

**LLMs and NLP** &nbsp;
![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![PEFT / LoRA](https://img.shields.io/badge/PEFT%20%2F%20LoRA-555555?style=flat-square)
![vLLM](https://img.shields.io/badge/vLLM-555555?style=flat-square)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![spaCy](https://img.shields.io/badge/spaCy-09A3D5?style=flat-square&logo=spacy&logoColor=white)

**Backend and data** &nbsp;
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Celery](https://img.shields.io/badge/Celery-37814A?style=flat-square&logo=celery&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![Milvus](https://img.shields.io/badge/Milvus-00A1EA?style=flat-square&logo=milvus&logoColor=white)

**Infrastructure and MLOps** &nbsp;
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square)
![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=flat-square&logo=mlflow&logoColor=white)
![Temporal](https://img.shields.io/badge/Temporal-000000?style=flat-square&logo=temporal&logoColor=white)

### Selected work
<!-- EVOLVING: keep 3–5 rows, strongest first. Replace a row when a better repo exists; never pad. -->

| Project | Problem it addresses | Stack |
|---|---|---|
| [**REPO_NAME: Medical knowledge graph builder**](https://github.com/kartikey05/Knowledge-graph-builder) <!-- TODO: only if public, personal and IP-clean --> | A single LLM's medical relationships are unreliable. Three models extract in parallel, agreements are accepted, and disagreements go to a verification step. | Python, LangGraph, FastAPI |
| [**Machine-Learning**](https://github.com/kartikey05/Machine-Learning) | End-to-end solution for the IIT Madras ML project on Kaggle, finishing in the top 10%. <!-- TODO: link the leaderboard in the repo README --> | Python, scikit-learn, pandas |
| [**TiccBoo**](https://github.com/kartikey05/TICCBOO_REPO) <!-- TODO: confirm repo name --> | Full-stack ticket-booking app with token auth and Redis caching | Flask, SQLAlchemy, Redis, Vue.js |

<details>
<summary><b>Professional work</b> (proprietary, so described without internal details)</summary>
<br>

- **Clinical document understanding:** OCR with vision models, section-aware chunking, LLM entity extraction, and mapping to standard terminologies (ICD-10, CPT, RxNorm)
- **Model adaptation and serving:** parameter-efficient fine-tuning of large open models, and serving them for low-latency inference
- **Multi-agent workflows:** orchestrated agents with structured outputs, rule-based validation and human review before any result is used

</details>

### Writing
<!-- TODO: keep only papers where your name is in the byline -->
- [Multi-tier Adaptive Evaluation for Clinical NER Systems](https://innovaccer.com/resources/white-papers/multi-tier-adaptive-evaluation-for-clinical-ner-systems) · author, white paper
- [Taming LLMs in Production: Control Patterns for Coding Agents and Clinical Text Generation](https://innovaccer.com/resources/white-papers/taming-llms-in-production-control-patterns-for-coding-agents-and-clinical-text-generation) · author, white paper

### How I build

- **Define "correct" first.** Decide how a system will be evaluated before choosing a model.
- **Use the simplest thing that meets the bar.** A prompt, a retriever, a fine-tune or plain code.
- **Treat model output as untrusted input.** Validate structure, check it against rules, and keep a trace back to the source.
- **Design for failure.** Timeouts, retries, isolation between stages, and logs you can read at 2 a.m.
- **Leave it runnable.** Clear READMEs, reproducible setup, and tests where they matter.

<!-- OPTIONAL: activate when you have real contributions. Merged PRs only.
### Open source
- [project](https://github.com/ORG/REPO/pull/NUMBER): what you changed and why
-->

<!-- OPTIONAL: stats card. Only use a self-hosted instance; see the setup guide.
<img src="https://YOUR-INSTANCE.vercel.app/api/top-langs/?username=kartikey05&layout=compact&hide_border=true" alt="Top languages" height="140">
-->
