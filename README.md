<div align="center">

**Mohamed Borhen Khlifi** · AI & Software Engineering

[Systems](#selected-systems) · [Architecture Deep-Dives](#architecture-deep-dives) · [Tech Stack](#tech-stack) · [Experience](#experience) · [Contact](#contact)

</div>

---

Third-year Computer Science Engineering student at **ENSI**, specializing in **Agentic AI, LLMs, Deep Learning, and modular backend systems**.  
Currently engineering multi-agent LLM workflows, explainable ML pipelines, and domain-generalization vision models.  
Seeking a **4–6 month PFE internship (starting early 2027)** in AI Engineering, ML Engineering, or GenAI — **[LinkedIn](https://www.linkedin.com/in/mohamed-borhen-khlifi-b07626325/)** · **[Email](mailto:your.email@example.com)** · **[Resume (PDF)](https://link-to-your-cv)**

> [!TIP]
> **Interactive profile:** Click any project drawer under **Architecture Deep-Dives** below to inspect system flows, design decisions, and native diagrams without leaving this page.

---

## Selected Systems

| Project | Focus | Core Stack | Key Highlight |
| :--- | :--- | :--- | :--- |
| **[code-review-agent](https://github.com/mohamedborhen/code-review-agent)** | Multi-Agent LLM System | Python, FastAPI, DeepAgents, MCP, Git, SQLite, Docker | Automated PR & diff review using Model Context Protocol (MCP) and Code Review Graphs |
| **[credit-risk-analysis](https://github.com/mohamedborhen/credit-risk-analysis)** | Explainable FinTech ML | XGBoost, Random Forest, SHAP, FastAPI, React.js | Stacked meta-learner credit scoring with per-decision SHAP explanations & interactive chatbot |
| **[CLIP-DRDG](https://github.com/mohamedborhen/CLIP-DRDG)** | Vision & Domain Generalization | PyTorch, CLIP, ViT, CoOpLVT, DomainBed | Cross-domain diabetic retinopathy benchmark across APTOS, EyePACS, Messidor & Messidor-2 |
| **[fraud_detection_app](https://github.com/mohamedborhen/fraud_detection_app)** | Real-Time Fraud Detection | Python, Scikit-learn, `[FastAPI / Streamlit]` | End-to-end anomaly & fraud scoring pipeline `[add key metric, e.g., PR-AUC / F1]` |

---

## Architecture Deep-Dives

<details>
<summary><b>1. code-review-agent</b> — Multi-Agent AI Code Reviewer (Click to expand)</summary>
<br>

Designed to automate contextual code reviews by combining repository graph traversal with multi-agent LLM reasoning.

```mermaid
flowchart LR
    A[Git Diff / PR] --> B[Code Review Graph]
    B --> C[MCP Server Context]
    C --> D[DeepAgents Orchestrator]
    D --> E[FastAPI Service + SQLite]
    E --> F[Structured Review Output]
