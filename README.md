<!-- Header --><p align="center">  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=170&section=header&text=Ali%20Fardaev&fontSize=42&fontColor=ffffff&fontAlignY=38&desc=AI%2FML%20Engineer%20%C2%B7%20San%20Francisco&descSize=18&descAlignY=60" alt="Ali Fardaev" /></p> <p align="center">  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=18&duration=3500&pause=900&color=2C9CDB&center=true&vCenter=true&width=620&lines=Building+RAG+and+LLM+systems+that+run+in+production;Retrieval+%C2%B7+Agents+%C2%B7+Backend+%C2%B7+MLOps" alt="Typing intro" /></p> <p align="center">  <a href="https://alifa.dev"><img src="https://img.shields.io/badge/Portfolio-alifa.dev-0f2027?style=for-the-badge&logo=googlechrome&logoColor=white" /></a>  <a href="https://www.linkedin.com/in/ali-fardaev"><img src="https://img.shields.io/badge/LinkedIn-ali--fardaev-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>  <a href="mailto:fardaevali@gmail.com"><img src="https://img.shields.io/badge/Email-fardaevali%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a></p>

---

### About me

-  **UC Berkeley MIDS** (Master of Information and Data Science), GPA 3.97
-  **2+ years of production ML engineering**, with a backend and full-stack foundation on AWS
-  **Focus:** RAG and hybrid retrieval, tool-calling LLM agents, evaluation, and deploying ML services that stay reliable after launch
-  **How I work:** keep the model out of anything that must be exactly right. Retrieval grounds answers, deterministic code does the math and the decisions, and tests cover both.

---

### Featured projects

| Project | What it does | Stack |
|---|---|---|
| **[MedCoverage](https://github.com/fardaevm/MedCoverage)** | Medi-Cal eligibility assistant. I built the RAG system, the LLM question-planning agent, the decision-tree logic, Redis caching, and the full AWS deployment. Hybrid retrieval grounds answers in policy documents, and a deterministic decision engine keeps outcomes auditable. | `FastAPI` `FAISS` `BM25` `Cohere` `LanceDB` `Redis` `AWS` |
| **[Ledger](https://github.com/fardaevm/ledger-app)** · [Live ↗](https://ledger-app-mocha-nine.vercel.app) | Shared household finance app in daily use. A hand-built tool-calling agent answers questions using only unit-tested Python functions (the model never does arithmetic), Plaid bank sync lands in a human-review queue before anything reaches the ledger, and Postgres row-level security is the authorization boundary. | `Claude API` `FastAPI` `Supabase` `Postgres` `Plaid` `Vercel` |
| **[Leazard](https://github.com/fardaevm/leazard)** | Lease risk analysis over San Francisco housing ordinances, with clause-level risk flags and tenant recommendations. | `LangGraph` `RAG` `Python` |
| **[Vizomaly](https://github.com/fardaevm/Vizomaly)** | Unsupervised industrial anomaly detection with pixel-level defect localization. | `PyTorch` `DINOv2` `ViT` |
| **[IgnisAI](https://github.com/fardaevm/Ignis-AI-WildFire)** | California wildfire risk modeling from satellite and weather data. | `scikit-learn` `SMOTE` `Geospatial` |

<details>
<summary><b> How MedCoverage works</b></summary>

```mermaid
flowchart LR
    U[User] --> A[LLM question-planning agent]
    A --> R[Hybrid retrieval<br/>FAISS + BM25]
    R --> C[Cohere reranking]
    C --> A
    A --> D[Deterministic<br/>decision engine]
    D --> O[Eligibility result]
    subgraph Infra[FastAPI · Redis · AWS]
    A
    R
    C
    D
    end
```

</details>

<details>
<summary><b>How Ledger's agent works</b></summary>

```mermaid
flowchart LR
    U[User question] --> M[Claude<br/>tool-calling loop]
    M -->|requests tool| T[Tested Python tools<br/>spending · debts · goals]
    T -->|RLS-scoped query| DB[(Supabase Postgres)]
    DB --> T
    T -->|exact numbers| M
    M --> A[Grounded answer]
    P[Plaid sync] --> Q[Review queue]
    Q -->|human approval| DB
```

Every number the assistant states comes from a tool call, not from the model. The agent queries with the user's own JWT, so it can never see more than the user can.

</details>

---

### Skills

**ML & Data:** Python · SQL · PyTorch · TensorFlow · scikit-learn · PySpark · Pandas · Hugging Face · Vision Transformers

**LLM & Retrieval:** RAG · hybrid search (FAISS, BM25) · reranking (Cohere) · LanceDB · LangChain · LangGraph · tool-calling agents · OpenAI and Anthropic APIs · LLM evaluation

**Backend & MLOps:** FastAPI · PostgreSQL · Redis · Docker · Kubernetes · AWS · GCP · GitHub Actions · Grafana · CI/CD · Vercel

<p>
  <img src="https://skillicons.dev/icons?i=python,pytorch,tensorflow,sklearn,postgres,fastapi,redis,docker,kubernetes,aws,gcp,githubactions&perline=12" />
</p>

---

### Let's talk

I'm actively interviewing for ML, AI, and MLOps engineering roles. The fastest way to reach me is [LinkedIn](https://www.linkedin.com/in/ali-fardaev) or [fardaevali@gmail.com](mailto:fardaevali@gmail.com).

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:2c5364,50:203a43,100:0f2027&height=90&section=footer" />
</p>
