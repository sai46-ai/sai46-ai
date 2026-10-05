<div align="center">

<img src="./assets/hero.svg" alt="Jaggarapu Venkata Sai - AI, Data, Software Engineering, Cloud" width="100%"/>

<a href="https://github.com/sai46-ai/sai46-ai">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&duration=3000&pause=1000&color=22D3EE&center=true&vCenter=true&width=760&lines=B.Tech+AI+%26+Data+Science+%7C+Class+of+2027;Full-stack+apps+with+AI+services+behind+them;Python+%7C+React+%7C+FastAPI+%7C+Node.js+%7C+PostgreSQL+%7C+MongoDB;Learning+RAG%2C+vector+search+and+MLOps" alt="Typing animation"/>
</a>

<br/>

<p align="center"><a href="#about"><img src="https://img.shields.io/badge/About-06B6D4?style=for-the-badge" alt="About"/></a> <a href="#featured-projects"><img src="https://img.shields.io/badge/Projects-8B5CF6?style=for-the-badge" alt="Projects"/></a> <a href="#tech-stack"><img src="https://img.shields.io/badge/Stack-EC4899?style=for-the-badge" alt="Stack"/></a> <a href="#currently-learning"><img src="https://img.shields.io/badge/Learning-F59E0B?style=for-the-badge" alt="Learning"/></a> <a href="#achievements"><img src="https://img.shields.io/badge/Achievements-22C55E?style=for-the-badge" alt="Achievements"/></a> <a href="#connect"><img src="https://img.shields.io/badge/Connect-3B82F6?style=for-the-badge" alt="Connect"/></a></p>

</div>

---

## About

I'm a final-year B.Tech student in Artificial Intelligence and Data Science at Vasireddy Venkatadri Institute of Technology (VVIT), Andhra Pradesh, graduating in 2027.

I build full-stack applications where a model or an LLM does a specific job inside a normal software system: resume parsing for campus hiring, anomaly detection on cloud bills, bill prediction for household electricity, a chatbot with stored conversation history. Most of my work sits between a React frontend, an API layer (FastAPI, Express or Flask), a database, and a small AI service.

I'm looking for software engineering and AI engineering roles and internships, with full-stack and GenAI application work as the closest fit.

---

## Engineering Profile

```text
┌───────────────────────────────────────────────────────────┐
│                    ENGINEERING PROFILE                    │
├───────────────────────────────────────────────────────────┤
│ Education     : B.Tech, AI & Data Science (2023 - 2027)   │
│ Institution   : VVIT, Andhra Pradesh, India               │
│ CGPA          : 8.95 / 10                                 │
│ Primary focus : Full-stack development with AI services   │
│ AI focus      : NLP, anomaly detection, LLM integration   │
│ Backend       : FastAPI, Node.js / Express, Flask         │
│ Data          : PostgreSQL, MongoDB, SQLAlchemy, Alembic  │
│ Cloud         : AWS (Cost Explorer, EC2), Docker          │
│ Status        : Open to internships and entry-level roles │
└───────────────────────────────────────────────────────────┘
```

| Domain | Current focus |
|---|---|
| Software engineering | Full-stack apps with role-based auth, REST APIs and dashboards |
| AI engineering | Resume NLP, Isolation Forest anomaly detection, LLM chat integration |
| Data | Relational schemas and migrations, cost and usage analytics, forecasting |
| Backend | FastAPI, Express, Flask, Celery and Redis background jobs |
| Cloud | AWS Cost Explorer integration, Docker Compose, Nginx |

---

## Featured Projects

Click a card to open the repository. Open the sections below for features and architecture.

<div align="center">

<a href="https://github.com/sai46-ai/cloud-cost-optimizer"><img src="assets/card-cloudwise.svg" width="48%" alt="CloudWise AI"/></a>
<a href="https://github.com/sai46-ai/AI-Campus-Recruitment-System"><img src="assets/card-recruit.svg" width="48%" alt="AI Campus Recruitment"/></a>
<a href="https://github.com/sai46-ai/Electricity-Billing-and-Budget-Optimization-System"><img src="assets/card-electricity.svg" width="48%" alt="Electricity Billing + Budget"/></a>
<a href="https://github.com/sai46-ai/ai-chatbot-react-flask"><img src="assets/card-chatbot.svg" width="48%" alt="AI Chatbot"/></a>

</div>

<details>
<summary><b>CloudWise AI - Cloud cost optimization and FinOps platform</b></summary>

[Repository](https://github.com/sai46-ai/cloud-cost-optimizer)

**Why it matters:** cloud bills are hard to read and spikes go unnoticed. CloudWise pulls spend data, flags unusual changes and suggests where to cut cost.

**What it does**
- Cost breakdowns by service, region, account and date, with budget thresholds at 50, 80, 90 and 100 percent
- Anomaly detection with scikit-learn's Isolation Forest, scored by severity
- LLM-based assistant that explains anomalies and rightsizing suggestions
- Rightsizing suggestions for EC2, RDS and S3
- PDF, CSV and Excel report export
- JWT auth, role-based access, multi-tenant organizations, audit log API, rate limiting
- Celery and Redis for background jobs, Docker Compose and Nginx for deployment

```text
React + TypeScript (Vite)
        │
        ▼
FastAPI  ──── JWT / RBAC / rate limiting
   │
   ├── PostgreSQL (SQLAlchemy, Alembic)
   ├── Redis ── Celery workers
   ├── Cost Explorer / CloudWatch (AWS provider)
   └── AI layer
        ├── Isolation Forest (anomaly detection)
        └── LLM assistant
```

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)

</details>

<details>
<summary><b>AI Campus Recruitment System</b></summary>

[Repository](https://github.com/sai46-ai/AI-Campus-Recruitment-System)

**Why it matters:** campus hiring means sorting through hundreds of resumes by hand. This system parses resumes, extracts skills and scores candidates with a formula that can be inspected.

**What it does**
- Resume parsing for PDF and DOCX, skill extraction with spaCy and a custom skill list
- Semantic skill matching with sentence-transformers
- Scoring across skills, experience, education and resume quality
- Student, recruiter and admin roles; jobs, applications, interviews and notifications
- Upload validation, auth and rate-limit middleware

```text
React frontend  ◄──►  Node / Express API  ◄──►  Python FastAPI AI service
                              │                        │
                              └────────  MongoDB  ─────┘
```

![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![spaCy](https://img.shields.io/badge/spaCy-09A3D5?style=flat-square&logo=spacy&logoColor=white)

</details>

<details>
<summary><b>Electricity Billing and Budget Optimization System</b></summary>

[Repository](https://github.com/sai46-ai/Electricity-Billing-and-Budget-Optimization-System)

**Why it matters:** households see a bill after the month ends. This app estimates usage from appliances, predicts the bill and shows how to stay inside a budget.

**What it does**
- Slab-tariff billing, bill payment flow, PDF bills, in-app notifications
- Bill and unit prediction with linear regression and random forest, best model chosen by MAE
- Budget advisor that ranks appliances by priority and suggests usage hours
- Admin analytics and monthly reports
- JWT roles (admin, customer), Helmet, rate limiting
- ML code runs as a separate Node.js service with a retraining endpoint

![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)

</details>

<details>
<summary><b>AI Chatbot (React and Flask)</b></summary>

[Repository](https://github.com/sai46-ai/ai-chatbot-react-flask)

A chat app that sends the last 10 exchanges as context to LLaMA 3.3 70B through the Groq API and stores every conversation in MongoDB. Includes a `/health` endpoint that checks the server and the database.

![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![Groq](https://img.shields.io/badge/Groq-F55036?style=flat-square)

</details>

---

## Tech Stack

### Building with
Technologies I've used in the projects above.

![Python](https://skillicons.dev/icons?i=python,js,ts,react,nodejs,express,fastapi,flask,vite&theme=dark)

![Data](https://skillicons.dev/icons?i=postgres,mongodb,redis,sklearn,docker,nginx,git,github&theme=dark)

| Area | Tools |
|---|---|
| Languages | Python, JavaScript, TypeScript, SQL |
| Frontend | React, Vite, Recharts, Tailwind CSS |
| Backend | FastAPI, Express, Flask, Celery, JWT auth |
| Databases | PostgreSQL, MongoDB, SQLAlchemy, Alembic, Mongoose |
| AI / ML | scikit-learn (Isolation Forest, random forest, regression), spaCy, sentence-transformers, LLM APIs (Groq, Gemini) |
| Infra | Docker, Docker Compose, Nginx, AWS |

### Working knowledge
Java, MySQL, Linux, HTML, CSS, Bootstrap, Postman

### Currently learning
RAG, vector databases, LangChain, LlamaIndex, MLOps, system design

---

## Currently Learning

<details>
<summary>Open the list</summary>

<br/>

- **RAG pipelines:** chunking, embeddings, retrieval and evaluation
- **Vector databases** and where they fit in an LLM application
- **LLM tooling:** LangChain and LlamaIndex
- **MLOps and deployment:** packaging, serving and monitoring models
- **System design:** scaling APIs, caching and queues
- **SQL:** deeper query work on PostgreSQL

</details>

---

## Open to Work

No internship or full-time experience yet. My experience so far comes from the projects above, and I'm looking for an internship or entry-level role in software or AI engineering.

---

## Achievements

<!-- TODO: add proof links (certificate URL, SIH result page, CodeChef username) before publishing -->

| Area | Detail |
|---|---|
| Hackathon | Smart India Hackathon 2025, national top 7 |
| Competitive programming | 500+ problems solved on CodeChef |
| Certification | Oracle Cloud Infrastructure AI Foundations |
| Academics | CGPA 8.95 / 10, B.Tech AI & Data Science |

---

## Roadmap

```text
2026
│
├── RAG and LLM application projects
├── Production habits: tests, CI, deployment, monitoring
├── Internship or entry-level role
└── Advanced SQL and PostgreSQL

2027
│
├── Graduate (B.Tech AI & Data Science)
├── MLOps and model serving
└── System design for scalable backends
```

---

## GitHub Analytics

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=sai46-ai&show_icons=true&theme=tokyonight&hide_border=true" alt="GitHub stats"/>
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=sai46-ai&layout=compact&theme=tokyonight&hide_border=true" alt="Top languages"/>

<img src="https://streak-stats.demolab.com?user=sai46-ai&theme=tokyonight&hide_border=true" alt="Contribution streak"/>

</div>

---

## Connect

<div align="center">

[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:jaggarapuvenkatasai@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/venkata-sai-jaggarapu/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/sai46-ai)

</div>
