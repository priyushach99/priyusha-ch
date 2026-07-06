## 👨‍💻 About Me

# Hi, I'm Priyusha 👋

Data engineer with experience in building batch pipelines that process millions of records daily - the kind where correctness and reliability aren't optional. My day-to-day lives in PySpark, Java, Airflow, Snowflake, and AWS.

After hours, I've been exploring what LLMs can do when wired into real data systems. That curiosity led me to build a RAG-based meeting summarizer - and eventually back to school. I'm currently doing my **MS in Information Studies** to advance my skills on scalable data platforms, and AI-driven data solutions.

---

## What I actually build

| | |
|---|---|
| 🔄 **Batch pipelines** | High-volume PySpark ETL with incremental loads, schema drift handling, and data quality validation gates |
| ⚡ **Streaming** | Kafka + Spark Structured Streaming — micro-batch processing with checkpoint recovery and weighted-merge aggregation |
| 🌿 **Orchestration** | Airflow DAGs with dependency management, retry logic, SLA tracking, and automated archival |
| 🗄️ **Data storage** | Snowflake and PostgreSQL on AWS — analytical and transactional, both at scale |
| 🤖 **LLM integration** | GPT-4o via prompt engineering, RAG with FAISS, rule-engine-as-ground-truth pattern to prevent hallucinated figures |

---

## Featured projects

### 📁 [AI Unified Data Platform](https://github.com/priyushach99/ai-unified-data-platform)
> `PySpark` `Kafka` `Airflow` `PostgreSQL` `GPT-4o` `Docker` `Python`

Built a production-grade data engineering pipeline that processes banking transactions through dual ingestion paths — Spark batch ETL and Kafka streaming — feeding clean data into PostgreSQL, then layering GPT-4o on top for AI-generated financial anomaly summaries, all orchestrated via Airflow. 

The real engineering challenge was LLM prompt design: a naive row-level approach ballooned to 8,500+ tokens and hit rate limits, so I built a rule engine that pre-aggregates transactions into deterministic signals — keeping the prompt fixed at ~800 tokens regardless of whether you're processing 700 or 5 million transactions. The LLM narrates, never recalculates — hallucinated figures in financial output aren't acceptable. 

Includes MD5-keyed caching to skip redundant LLM calls, graceful fallback to rule-based summaries on API failure, and incremental weighted-average merging for Kafka micro-batches so daily totals accumulate correctly across 10-second windows.

---

### 📁 [LLM-Powered Meeting Intelligence System](https://github.com/priyushach99/llm_meeting_summarizer)
> `Python` `LLaMA3` `FAISS` `Whisper` `RAG`

Tired of losing track of decisions and action items after long meetings, I built a fully local AI pipeline that turns raw audio into structured intelligence — transcripts, summaries, owner-assigned action items, and a Q&A interface to interrogate the meeting like a document. 

Chains Whisper → SentenceTransformers → FAISS → LLaMA 3, all running on your machine with zero API costs. 

The interesting engineering challenge was getting RAG retrieval quality right — naive chunking produced weak context, so I tuned chunk size, overlap, and similarity thresholds until results felt genuinely useful. Includes deterministic caching and one-click PDF export.

---

## Technical Skills

**Languages**
`Python` `SQL` `PySpark` `Spark SQL` `Java` `JavaScript` `TypeScript` `Bash` `Linux/Shell`

**Data Engineering & Pipelines**
`Apache Spark` `Apache Kafka` `Apache Airflow` `ETL / ELT` `Spark Structured Streaming`
`Kafka Streaming` `dbt` `Data Quality Frameworks` `Query Optimization`

**Databases**
`Snowflake` `PostgreSQL` `MongoDB` `NoSQL` `Database Design` 

**GenAI / LLM**
`LLaMA 3` `Groq` `OpenAI` `Anthropic` `Model Context Protocol (MCP)` `Agent-to-Agent (A2A)`
`RAG` `FAISS` `Sentence Transformers` `OpenAI Whisper` `Prompt Engineering` `PyDub` `ReportLab` `FPDF`

**Cloud & DevOps**
`AWS S3` `AWS IAM` `Secure Cloud Data Ingestion` `GitLab CI/CD` `Jenkins` `Docker` `Git`

**Data & Visualization**
`Pandas` `NumPy` `Scikit-learn` `Tableau` `PowerBI`

**Frontend & Frameworks**
`React` `Node.js` `Angular` `Streamlit`

---

## Currently

- 🔍 Exploring agentic pipelines that connect LLMs to production data systems
- 💼 Open to **SDE**, **Data engineering** and **AI/ML engineering** roles

---

## 📫 Connect With Me
- LinkedIn: *www.linkedin.com/in/priyusha24*
- GitHub: https://github.com/priyushach99

---

⭐ If you like my work, feel free to star my repositories!
