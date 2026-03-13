<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=180&section=header&text=Abderrahman%20ES-SEBYITY&fontSize=42&fontAlignY=32&desc=AI/ML%20Engineer%20%7C%20LLM%20Fine-Tuning%20%7C%20RAG%20Pipelines%20%7C%20Full-Stack%20Deployment&descSize=16&descAlignY=51&animation=twinkling" width="100%"/>

</div>

<div align="center">

[![Portfolio](https://img.shields.io/badge/🌐_Portfolio-Visit-blue?style=for-the-badge)](https://abderrahman-essebyity.vercel.app/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/abderrahman-essebyity/)
[![Email](https://img.shields.io/badge/Email-Contact-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:abderrahman.essebyity@gmail.com)
[![Dataset](https://img.shields.io/badge/Zenodo-Published%20Dataset-blue?style=for-the-badge)](https://doi.org/10.5281/zenodo.18642248)

📍 Morocco 🇲🇦 &nbsp;·&nbsp; Open to PFE Internships & AI/ML Roles

<img src="https://komarev.com/ghpvc/?username=abdrahmanES1&label=Profile%20Views&color=0e75b6&style=flat" />

</div>

---

## About

I build AI systems end-to-end — from model training to production deployment. I specialize in LLM fine-tuning, RAG pipelines, and generative models, and I can ship the full stack around them (FastAPI, Docker, React).

**Three things I've built that actually work:**

- Fine-tuned **Mistral-Nemo 12B** on a custom dataset → **91% quality vs Gemini at 7x lower cost**
- Built a **CVAE + Latent DDPM** for medical image synthesis → **22% better FID** than CVAE-only
- Deployed a **distributed MAS** with 20+ agents and online ML → **<200ms consensus**, survives 30% node failure

---

## Projects

### 🔬 [fact-checking-slm](https://github.com/abdrahmanES1/fact-checking-slm)
**Fine-tuned Mistral-Nemo 12B + multi-agent RAG pipeline**

Built a synthetic training dataset via knowledge distillation from Gemini 2.5 Pro (1,096 samples, published on [Zenodo](https://doi.org/10.5281/zenodo.18642248)). Fine-tuned with QLoRA, achieving 0.92 training loss. RAG pipeline uses LangChain + ChromaDB with Tavily web search fallback for low-confidence retrievals. Ships with 3 production-ready n8n workflows (ingestion, retrieval, fact-checking).

| | Gemini 2.5 Pro | Fine-Tuned SLM |
|---|---|---|
| Overall quality | 97.4% | **91.0%** |
| NLI faithfulness | 0.778 | **0.789** |
| Cost / 1k docs | $3.49 | **$0.47** |
| Win rate vs base model | — | **88%** |

`PyTorch` `QLoRA` `Unsloth` `LangChain` `ChromaDB` `Ollama` `n8n` `Supabase` `Tavily`

---

### 🧬 [CVAE-DDPM-Hybrid-Generative-Model-for-Medical-Image-Synthesis](https://github.com/abdrahmanES1/CVAE-DDPM-Hybrid-Generative-Model-for-Medical-Image-Synthesis)
**Two-stage liver MRI synthesis across 5 cancer classes**

CVAE learns a class-conditioned latent space (val PSNR 24.49 dB, SSIM 0.742). Latent DDPM then refines samples in that space — skipping pixel-space diffusion cost while improving perceptual quality. β-VAE warmup prevents posterior collapse on the small medical dataset.

| | CVAE-only | CVAE+DDPM |
|---|---|---|
| Avg FID ↓ | 1043.2 | **814.1 (−22%)** |
| Avg SSIM ↑ | 0.257 | **0.264** |
| Val PSNR | — | **24.49 dB** |

`PyTorch` `Diffusers` `LPIPS` `BERTScore` `Kaggle T4`

---

### 🤖 [Distributed-Anomaly-Detection-MAS](https://github.com/abdrahmanES1/Distributed-Anomaly-Detection-MAS)
**20+ agent distributed system with online ML and chaos engineering**

Each agent runs HalfSpaceTrees (River) for incremental anomaly detection on streaming sensor data. Agents communicate over XMPP with a trust-based reputation protocol — dead nodes are pruned via heartbeat, low-trust nodes auto-isolated. Chaos mode simulates random failures. Streamlit War Room dashboard for live topology monitoring.

- **<200ms** consensus latency · **30% node loss** with full operational integrity

`Python` `River` `SPADE` `XMPP` `Prosody` `Docker` `Streamlit`

---

### 🧠 Brain Tumor Classification & Segmentation
Comparative study on 24,169 MRI images: classical ML (LBP+SVM, XGBoost) vs deep learning (ResNet50, VGG16, U-Net). ResNet50 hit **92.1% accuracy** vs 82.3% best classical baseline. U-Net segmentation DSC 0.88 vs 0.41 for XGBoost.

`PyTorch` `TensorFlow` `Transfer Learning` `U-Net` `Computer Vision`

---

### 🌐 Web & Open Source

**[EsteQuiz](https://github.com/abdrahmanES1/Quiz)** — University exam platform with student and admin panels &nbsp;·&nbsp; `React` `Express` `MongoDB` `Zustand` `ChakraUI`

**[Magic UI](https://github.com/magicuidesign/magicui)** — Open source contributor · components, linting system, docs &nbsp;·&nbsp; `React` `Next.js` `Shadcn` `TailwindCSS`

**[express-api-initializer](https://www.npmjs.com/package/express-api-initializer)** — npm CLI tool for scaffolding Express.js apps &nbsp;·&nbsp; `TypeScript` `Node.js` `Commander`

---

## Stack

**AI/ML** &nbsp;·&nbsp; `PyTorch` `TensorFlow` `HuggingFace` `QLoRA` `LangChain` `ChromaDB` `Ollama` `River` `Scikit-learn` `Diffusers` `Unsloth`

**Generative AI** &nbsp;·&nbsp; `Mistral` `Gemini API` `OpenAI API` `n8n` `Tavily` `Supabase`

**Deployment** &nbsp;·&nbsp; `FastAPI` `Docker` `Streamlit` `Vercel` `XMPP`

**Full-Stack** &nbsp;·&nbsp; `Python` `TypeScript` `React` `Next.js` `Node.js` `MongoDB` `PostgreSQL`

---

## GitHub Stats

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=abdrahmanES1&theme=radical&hide_border=true" alt="GitHub Streak" />
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=abdrahmanES1&theme=react-dark&hide_border=true&area=true" width="95%" alt="Contribution Graph" />
</p>

---

## Background

🎓 Master's in Data Science & Analytics — Cadi Ayyad University *(2024–2026)*

💼 Front-End Developer — Integral Progress Technology *(Apr–Aug 2024)* · React · TypeScript · Redux Toolkit

🌍 Arabic (Native) · French (Professional) · English (Professional)

---

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=100&section=footer" width="100%"/>
</div>
