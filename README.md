<!-- Header -->
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=170&section=header&text=Ali%20Fardaev&fontSize=42&fontColor=ffffff&fontAlignY=38&desc=AI%2FML%20Engineer%20%C2%B7%20San%20Francisco&descSize=18&descAlignY=60" alt="Ali Fardaev" />
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=18&duration=3500&pause=900&color=2C9CDB&center=true&vCenter=true&width=620&lines=Building+RAG+and+LLM+systems+that+run+in+production;Retrieval+%C2%B7+Agents+%C2%B7+Backend+%C2%B7+MLOps" alt="Typing intro" />
</p>

<p align="center">
  <a href="https://alifa.dev"><img src="https://img.shields.io/badge/Portfolio-alifa.dev-0f2027?style=for-the-badge&logo=googlechrome&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/ali-fardaev"><img src="https://img.shields.io/badge/LinkedIn-ali--fardaev-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
  <a href="mailto:fardaevali@gmail.com"><img src="https://img.shields.io/badge/Email-fardaevali%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a>
</p>

---

### 👋 About me

I'm an AI/ML engineer in San Francisco and a UC Berkeley MIDS grad. I build LLM and retrieval systems, and the backend and infrastructure that make them reliable in production.

- 🔍 **Focus:** RAG, LLM agents, evaluation, and production ML services
- 🛠️ **Background:** full stack and backend engineering on AWS
- 📷 **Off the keyboard:** landscape photography around California

---

### 🚀 Featured projects

| Project | What it does | Stack |
|---|---|---|
| **[MedCoverage](https://github.com/fardaevm/MedCoverage)** | Medi-Cal eligibility assistant: an LLM agent gathers user details, hybrid retrieval grounds answers in policy documents, and a deterministic decision engine keeps outcomes auditable | `FastAPI` `FAISS` `BM25` `Cohere` `LanceDB` `Redis` `Kubernetes` `Grafana` |
| **[Leazeard](https://github.com/fardaevm/leazeard)** | Lease risk analysis over San Francisco housing ordinances with clause-level risk flags and tenant recommendations | `LangGraph` `RAG` `Python` |
| **[SkyPredict]** | Flight delay prediction on 840M+ weather and aviation records; AUC 0.61 → 0.79 | `PySpark` `Spark ML` `SQL` |
| **[Vizomaly](https://github.com/fardaevm/Vizomaly)** | Unsupervised industrial anomaly detection with pixel-level defect localization | `PyTorch` `DINOv2` `ViT` |
| **[IgnisAI](https://github.com/fardaevm/ignisai)** | California wildfire risk modeling from satellite and weather data | `scikit-learn` `SMOTE` `Geospatial` |

<details>
<summary><b>🧭 How MedCoverage works</b> (click to expand)</summary>

```mermaid
flowchart LR
    U[User] --> A[LLM question-planning agent]
    A --> R[Hybrid retrieval<br/>FAISS + BM25]
    R --> C[Cohere reranking]
    C --> A
    A --> D[Deterministic<br/>decision engine]
    D --> O[Eligibility result]
    subgraph Infra[FastAPI · Redis · Kubernetes on AWS · Grafana]
    A
    R
    C
    D
    end
```

</details>

---

### 🧰 Tech stack

**Languages & ML**
<p>
  <img src="https://skillicons.dev/icons?i=python,ts,postgres,pytorch,tensorflow,sklearn&perline=10" />
</p>

**LLM & AI**
<p>
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white" />
  <img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white" />
  <img src="https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black" />
  <img src="https://img.shields.io/badge/OpenAI%20API-412991?style=flat-square&logo=openai&logoColor=white" />
  <img src="https://img.shields.io/badge/RAG-2C5364?style=flat-square" />
  <img src="https://img.shields.io/badge/FAISS-0467DF?style=flat-square&logo=meta&logoColor=white" />
  <img src="https://img.shields.io/badge/Apache%20Spark-E25A1C?style=flat-square&logo=apachespark&logoColor=white" />
</p>

**Backend, Cloud & MLOps**
<p>
  <img src="https://skillicons.dev/icons?i=fastapi,react,redis,mongodb,docker,kubernetes,aws,gcp,githubactions,grafana&perline=10" />
</p>

---

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:2c5364,50:203a43,100:0f2027&height=90&section=footer" />
</p>
