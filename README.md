![name_github.gif](https://github.com/toshikdkar9/toshikdkar9/blob/main/name_github.gif)

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=toshikdkar9&label=Profile%20views&color=0e75b6&style=flat" alt="toshikdkar9" />
</p>

<p align="center">
  <a href="https://linkedin.com/in/toshikd/"><img src="https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin"></a>
  <a href="https://scholar.google.co.in/citations?user=CNQaJEUAAAAJ&hl=en"><img src="https://img.shields.io/badge/Google%20Scholar-Research-blueviolet?style=for-the-badge&logo=google-scholar"></a>
  <a href="https://toshikdhanurkar.com"><img src="https://img.shields.io/badge/Blog-toshikdhanurkar.com-orange?style=for-the-badge&logo=rss"></a>
</p>

---

Senior Data Scientist building production AI systems at an industrial manufacturing group. Sole architect and developer — from requirements through deployment and LLMOps. M.Tech from IISc Bangalore, published in *Science of the Total Environment* (Q1, IF 8.1), Rank 1 at SciML Bootcamp 2026 with MIT & Purdue PhD mentorship.

I transitioned from Civil Engineering to AI — the future should be built with both concrete and code.

---

## 🏗️ Production Systems

> These are deployed, maintained, and serving real users. End-to-end sole ownership on each.

<details>
<summary><b>🔩 Industrial Drawing Intelligence Pipeline</b> — Computer Vision · OCR · LLM · MLOps</summary>
<br>

End-to-end CV pipeline extracting structured instrument data from multi-page P&ID engineering drawings. Replaced a fully manual process (8–16 hours per PDF) → under 30 minutes of human review.

- Custom YOLOv11s (1920px, ~10K annotated symbols) — **98.37% recall, 98.68% mAP@0.5** across 25+ MLflow-tracked experiments over 7 architectures (GFL, Faster R-CNN, RetinaNet, FCOS, ATSS, VarifocalNet)
- Multi-stage OCR: PaddleOCR (DBNet + CRNN) + OpenCV preprocessing + domain rule-based post-processing + spatial symbol-to-tag linking
- LLM-powered contextual metadata extraction; ISA 5.1 classification engine (11 structured columns, confidence-gated Green/Yellow/Red triage)
- ONNX FP16/INT8 quantization; containerized FastAPI on Azure Container Apps; DVC + Blob versioning; Azure Pipelines CI/CD; air-gapped annotation for data compliance

`YOLOv11` `PaddleOCR` `GPT-5` `ONNX Runtime` `FastAPI` `Azure Container Apps` `MLflow` `DVC`

</details>

<details>
<summary><b>💬 Engineering Knowledge RAG System</b> — RAG · Hybrid Search · LLMOps</summary>
<br>

Production RAG system that surfaces relevant historical annotations when engineers highlight text in specification PDFs — replacing blank comment boxes with institutional knowledge. Saves ~10 min per requirement across hundreds per project.

- 100K+ engineering rows processed through GPT-5 mini for extraction, cleaning, and embedding (text-embedding-3-large)
- Hybrid search: pgvector dense retrieval + PostgreSQL FTS + Reciprocal Rank Fusion — **zero LLM calls at inference** for cost-efficient serving
- LLMOps: YAML prompt versioning + MLflow Registry, LLM-as-judge eval (faithfulness, completeness, clarity), offline eval gates; 45 search configs tuned on MRR@5 and NDCG@5
- Embedding drift detection with weekly alerting; Azure Functions for daily SQL Server → PostgreSQL sync; Application Insights observability

`pgvector` `PostgreSQL FTS` `GPT-5 mini` `FastAPI` `Azure Functions` `MLflow` `LLM-as-Judge`

</details>

<details>
<summary><b>🔍 Enterprise Document Intelligence Platform</b> — RAG · Multimodal · Evaluation</summary>
<br>

AI backend for enterprise search over 100K+ documents. Systematic evaluation: 8 PDF extractors × 6 chunking strategies × embedding model comparisons × GPT-based reranking — benchmarked on 100 manually curated Q&A pairs across 12 metrics.

- Multimodal pipeline: PaddleOCR + Tesseract + CLIP embeddings, HNSW ANN search, embedding quantization — **sub-200ms inference latency**
- Selected Docling + semantic chunking (HuggingFace) as optimal config through rigorous ablation on MRR, NDCG, Precision, RAGAS, PDF/Page Accuracy

`CLIP` `FAISS` `Docling` `HuggingFace` `Azure OpenAI` `RAGAS`

</details>

<details>
<summary><b>🤖 Agentic AI & GenAI Applied Research</b> — LLMs · Fine-Tuning · Agents</summary>
<br>

Led company-wide AI enablement: 20+ workshops → 7 proof-of-concepts adopted. Delivered in 5-week sprints:

- **Multilingual Translation:** Fine-tuned seq2seq (LoRA/QLoRA) for instruction manuals; BLEU evaluation with DVC versioning
- **IT Ticket Resolution:** Agentic LLM (LangGraph + RAG/FAISS + GPT-4o) for automated classification; benchmarked 5 prompt strategies on accuracy and token efficiency
- **Compliance Automation:** LLM pipeline for supplier email analysis against RoHS/REACH using parallel LangChain processing

`LangGraph` `LangChain` `GPT-4o` `LoRA` `QLoRA` `FAISS` `DVC`

</details>


---

## 🛠️ Stack

<p>
  <img src="https://skillicons.dev/icons?i=python,pytorch,tensorflow,fastapi,docker,kubernetes,azure,postgresql,git,linux,opencv,redis,mongodb,rust" />
</p>

**Gen AI:** LLMs (OpenAI, HuggingFace), RAG, Multimodal RAG, Agentic AI, LangChain, LangGraph, Fine-Tuning (LoRA, PEFT), LLM Evaluation (RAGAS, LLM-as-Judge)  
**ML & Vision:** PyTorch, TensorFlow, YOLOv11, PaddleOCR, CLIP, SAM, ONNX Runtime, Diffusion Models  
**MLOps:** MLflow, DVC, Azure DevOps, CI/CD, Docker, Kubernetes, Vector DBs (pgvector, FAISS, Chroma), Drift Detection  
**Cloud:** Azure (Container Apps, Function Apps, Blob Storage, AI Foundry, OpenAI), Databricks, PySpark  
**Data & BI:** Power BI, Tableau, Pandas, NumPy, Scikit-learn, Plotly

---

## 📄 Publication

**Dhanurkar, Budamala & Bhowmik (2024)** — *Understanding the association between global forest fire products and hydrometeorological variables.*  
Science of the Total Environment · Impact Factor: 8.1 · Q1

---

## 🏆 Honors

- 🥇 **Rank 1** — SciML Bootcamp Challenge 2026 · Physics-constrained Neural ODE proposal · MIT & Purdue PhD mentorship
- 🎓 M.Tech, IISc Bangalore (CGPA: 8.10) · B.E., YCCE Nagpur (CGPA: 8.30)

---

## 📚 Certifications

- Introduction to Large Language Models — NPTEL (IIT Delhi & IIT Bombay)
- Azure AI & Cloud Fundamentals — AZ-900 & AI-100
- Generative AI Specialization — deeplearning.ai
- MLOps Specialization — Duke University

---

## 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=toshikdkar9&show_icons=true&theme=tokyonight&hide_border=true" alt="GitHub Stats" />
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=toshikdkar9&theme=tokyonight&hide_border=true" alt="GitHub Streak" />
</p>
