

# Hi There, I'm Megha Shyam 👋

Ex-Samsung SWE, now building ML systems from scratch.

2+ years building production systems at Samsung. I build from scratch because abstractions hide the interesting parts.

## What I'm building

 
### [RezRAG](https://github.com/your-username/rezrag) — Production RAG on the Yelp dataset
Raw JSON to deployed API, end to end from scratch with zero RAG frameworks (no LangChain,
no LlamaIndex)

- **Hybrid retrieval**: E5-large-v2 dense embeddings + BM25Okapi sparse + Reciprocal Rank Fusion
- **Reranking**: CrossEncoder reranking, confirmed live in production
- **Inference**: Groq (gpt-oss-20b) in prod, local Qwen2.5-3B NF4 quantization for dev (2.2GB VRAM, RTX 3060, ~11.8 tok/sec)
- **Stack**: FastAPI microservices, Next.js + Leaflet frontend, Qdrant Cloud, deployed on Modal + Vercel

**Eval**: 47 human-labeled queries across 12 US cities.

| Strategy | MRR@5 | 95% CI | Hit@3 | Hit@5 | P@5 |
|:---|:---|:---|:---|:---|:---|
| Hybrid + Rerank | 0.760 | [0.678, 0.841] | 0.979 | 1.000 | 0.413 |
| Hybrid (no rerank) | 0.639 | [0.524, 0.753] | 0.745 | 0.830 | 0.349 |

**Live**: [yelp-restaurant-rag.vercel.app](https://yelp-restaurant-rag.vercel.app)


---
 
### [PitchPulse FIFA2026](https://github.com/your-username/pitchpulse-worldcup2026) — Match intelligence for the 2026 FIFA World Cup
Real-time tournament simulation and tactical analysis, built for the World Cup
2026 group stage through knockout rounds.
 
- **Tournament simulation**: vectorized Monte Carlo (50k sims in 0.70s) using Common Random
  Numbers for counterfactual variance reduction
- **Live modeling**: EWMA momentum tracking, Poisson-based in-play outcome modeling,
  IsolationForest for narrative spike detection
- **RAG**: Weaviate hybrid retrieval (dense + BM25) for tactical briefings
- **Inference**: local-first via Ollama (Mistral 7B), Groq 70B fallback
- **Architecture**: 4 independent async background workers polling Redis (counterfactual,
  intel, momentum, narrative), FastAPI + Redis + Weaviate backend, Next.js frontend

 
---
 
## Currently open to full-time ML/AI engineering roles

Feel free to reach me at: [megh2k18@gmail.com](megh2k18@gmail.com)


<h3 align="left">Languages and Tools:</h3>
<p align="left">

<!-- Languages -->
<img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white"/>
<img src="https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white"/>

<!-- LLM Stack -->
<img src="https://img.shields.io/badge/HuggingFace-FFD21E?style=flat&logo=huggingface&logoColor=black"/>
<img src="https://img.shields.io/badge/Transformers-FFD21E?style=flat&logo=huggingface&logoColor=black"/>
<img src="https://img.shields.io/badge/PEFT-FFD21E?style=flat&logo=huggingface&logoColor=black"/>
<img src="https://img.shields.io/badge/BitsAndBytes-FF6F00?style=flat&logoColor=white"/>
<img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat&logo=langchain&logoColor=white"/>
<img src="https://img.shields.io/badge/FAISS-00599C?style=flat&logoColor=white"/>
<img src="https://img.shields.io/badge/Weights_%26_Biases-FFBE00?style=flat&logo=weightsandbiases&logoColor=black"/>

<!-- AI Models / APIs -->
<img src="https://img.shields.io/badge/OpenAI-412991?style=flat&logo=openai&logoColor=white"/>
<img src="https://img.shields.io/badge/Claude-D97757?style=flat&logo=anthropic&logoColor=white"/>
<img src="https://img.shields.io/badge/Gemini-8E75B2?style=flat&logo=googlegemini&logoColor=white"/>

<!-- Infra -->
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white"/>
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white"/>
<img src="https://img.shields.io/badge/Modal-000000?style=flat&logoColor=white"/>
<img src="https://img.shields.io/badge/Qdrant-FF4154?style=flat&logoColor=white"/>
<img src="https://img.shields.io/badge/Next.js-000000?style=flat&logo=nextdotjs&logoColor=white"/>

<img src="https://img.shields.io/badge/Sentence_Transformers-FFD21E?style=flat&logo=huggingface&logoColor=black"/>
<img src="https://img.shields.io/badge/Groq-F55036?style=flat&logoColor=white"/>
<img src="https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white"/>
<img src="https://img.shields.io/badge/Scikit--learn-F7931E?style=flat&logo=scikitlearn&logoColor=white"/>
<img src="https://img.shields.io/badge/Weaviate-00B5A3?style=flat&logoColor=white"/>
<img src="https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white"/>
<img src="https://img.shields.io/badge/Ollama-000000?style=flat&logoColor=white"/>

<img src="https://img.shields.io/badge/Accelerate-FFD21E?style=flat&logo=huggingface&logoColor=black"/>
<img src="https://img.shields.io/badge/MLflow-0194E2?style=flat&logo=mlflow&logoColor=white"/>
<img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=githubactions&logoColor=white"/>
<img src="https://img.shields.io/badge/Ragas-FF4154?style=flat&logoColor=white"/>

<img src="https://img.shields.io/badge/AWS-232F3E?style=flat&logo=amazonaws&logoColor=white"/>
<img src="https://img.shields.io/badge/Kubernetes-326CE5?style=flat&logo=kubernetes&logoColor=white"/>
<img src="https://img.shields.io/badge/LangSmith-1C3C3C?style=flat&logo=langchain&logoColor=white"/>
<img src="https://img.shields.io/badge/Apache_Airflow-017CEE?style=flat&logo=apacheairflow&logoColor=white"/>
</p>
