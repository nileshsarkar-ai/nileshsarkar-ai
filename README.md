<div align="center">

# Nilesh Sarkar

**AI Researcher — Knowledge Distillation · Mechanistic Interpretability · World Models**

[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=githubpages&logoColor=white)](https://nileshsarkar-ai.github.io/)
[![Erdős AI Lab](https://img.shields.io/badge/Erdős_AI_Lab-059669?style=for-the-badge&logoColor=white)](https://www.erdoslab.org/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/nileshsarkar-ai/)
[![Hugging Face](https://img.shields.io/badge/🤗_Hugging_Face-FFD21E?style=for-the-badge&logoColor=black)](https://huggingface.co/nileshsarkar-ai)
[![Scholar](https://img.shields.io/badge/Scholar-4285F4?style=for-the-badge&logo=googlescholar&logoColor=white)](https://scholar.google.com/citations?user=9mnmA5YAAAAJ&hl=en)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:nileshsarkar.cs@gmail.com)

*AI Researcher · Erdős AI Lab · 2026–Present*
*B.Tech Artificial Intelligence & Robotics · Dayananda Sagar University · 2023–2027*

</div>

---

## About

AI Researcher at **Erdős AI Lab**, working on the boundary between how language models compress information and how that information is mechanistically structured inside the network.

I treat **knowledge distillation, sparse autoencoders, pruning, and quantization** as analytical probes rather than just engineering optimizations — using compression to surface what models actually represent, and using interpretability to figure out what we can or cannot afford to compress.

```
Current threads: Knowledge distillation · Sparse autoencoders (SAEs) · World models
                 LLM architecture & compression · Protein structure prediction
                 Medical imaging · Agentic RAG · Indic NLP
```

---

## Research & Projects

### Knowledge Distillation: A Minimum-Width Theorem
> *First-author · Under review at COLM 2026 · Erdős AI Lab*

A theoretical and empirical study on the dictionary width at which a sparse autoencoder's reconstruction loss bottoms out, given a target sparsity. Toy-model validation followed by three real-LM trials on Pythia-410M (24 layers × 6 token checkpoints each).

Checkpoints on Hugging Face:
- [`colm-run-exp-2-t1`](https://huggingface.co/nileshsarkar-ai/colm-run-exp-2-t1) (L1 = 3e-4 fixed, dense regime)
- [`colm-run-exp-2-t2`](https://huggingface.co/nileshsarkar-ai/colm-run-exp-2-t2) (L1 = 8e-5 fixed, paper-exact)
- [`colm-run-trial-2`](https://huggingface.co/nileshsarkar-ai/colm-run-trial-2) (L1 = 5e-4 adaptive, target L0 ≈ 150)

`PyTorch` `Pythia` `SAE` `Mechanistic Interpretability`

---

### Mechanistic Interpretability Experiments
> *Active · Erdős AI Lab*

Probing transformer internals with sparse autoencoders, attention-circuit analysis, and feature-attribution studies. Extending to attention-circuit analysis on IOI / induction heads, feature-attribution probes on reasoning benchmarks, and cross-model generalisation (Pythia-410M → 1.4B → 2.8B).

Adjacent thread: a framework for better generalisation on low-sample medical imaging without generative deepfake augmentation.

`PyTorch` `SAEs` `Probing` `Activation Patching`

---

### Medical AI: PCOS Detection
> *Published in journal · Erdős AI Lab*

"A Systematic Deep Learning Framework for PCOS Detection Using Deduplicated Ultrasound Images: Comparative Analysis of CNN and Vision Transformer Models." A novel three-stage deduplication pipeline (MD5 + perceptual hashing + cross-class removal) cleaned the PCOS-XAI dataset from 11,784 to 3,490 images (70.4% removed). Systematic benchmark of **18 architectures** (13 CNNs + 5 ViTs) under identical conditions for 200 epochs.

**Top result:** EfficientFormer-L1 and MobileViT-Small (hybrid CNN-Transformer) tied at **99.81%** test accuracy with AUC up to 1.0. Pure ViT-Base and Swin Transformer Base failed to converge on this dataset size.

**Compute:** NVIDIA A100 (80 GB VRAM) · 64 GB system RAM · Intel Xeon 42-core CPU.

`PyTorch` `Vision Transformers` `CNNs` `Medical Imaging`

---

### Protein Folding Experiments
> *Active · Erdős AI Lab*

Structure-prediction studies on small proteins — pLDDT-style confidence calibration, folding-trajectory dynamics (Q, Cα RMSD, R_g, Q–RMSD landscape), and head-to-head comparisons between transformer folding stacks and classical MD baselines.

`PyTorch` `ESMFold` `Computational Biology`

---

### LLM Architecture & Compression
> *Active · 2025–Present*

Compression and deployment experiments across 0.5B–7B parameter models. Teacher–student distillation for Hindi and Kannada low-resource instruction datasets. Deployed a Gemma 3 1B model on NVIDIA Jetson Nano for real-time on-device inference. Now exploring diffusion-based language models for Indic text generation.

`QLoRA` `LoRA` `Quantization` `NVIDIA Jetson` `Indic NLP`

---

### Agentic RAG for Safety-Critical Engineering Docs
> *Industry research · Moog India Technology Centre*

Agentic retrieval systems for multi-step reasoning over large structured aerospace engineering corpora. Query-aware routing, citation-grounded retrieval, structured reasoning pipelines. Improved document retrieval accuracy from **~70% to 90%+**. Includes an MCP (Model Context Protocol) server for tool integration.

`LangChain` `LangGraph` `n8n` `RAG` `MCP` `Vector Databases`

---

### Autonomous Drone Perception
> *Active · Sep 2025–Present*

Vision-based navigation pipelines for all-terrain UAVs — real-time obstacle detection, monocular depth estimation, and sensor fusion for autonomous flight in unstructured environments.

`OpenCV` `ROS2` `Depth Estimation` `Sensor Fusion`

---

### Humanoid Robotic Prosthetic Arm
> *Active · Jun 2025–Present*

Perception-driven servo control and actuation systems for humanoid prosthetic arm prototypes, integrating real-time visual feedback for adaptive grasping.

`ROS2` `Servo Control` `Computer Vision` `Hardware-in-the-Loop`

---

## Tech Stack

**Research & Modeling**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![CUDA](https://img.shields.io/badge/CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![Hugging Face](https://img.shields.io/badge/🤗_Hugging_Face-FFD21E?style=flat-square&logoColor=black)

**LLM & Agent Systems**

![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-F2A007?style=flat-square&logoColor=white)
![n8n](https://img.shields.io/badge/n8n-EA4B71?style=flat-square&logo=n8n&logoColor=white)
![MCP](https://img.shields.io/badge/MCP_Server-412991?style=flat-square&logoColor=white)
![RAG](https://img.shields.io/badge/RAG_·_Vector_DBs-3E5BE1?style=flat-square&logoColor=white)

**Compression & Interpretability**

![SAE](https://img.shields.io/badge/Sparse_Autoencoders-059669?style=flat-square&logoColor=white)
![QLoRA](https://img.shields.io/badge/LoRA_·_QLoRA-2563EB?style=flat-square&logoColor=white)
![Quantization](https://img.shields.io/badge/Quantization-0EA5E9?style=flat-square&logoColor=white)
![Distillation](https://img.shields.io/badge/Knowledge_Distillation-10B981?style=flat-square&logoColor=white)

**Robotics & Edge**

![ROS](https://img.shields.io/badge/ROS2-22314E?style=flat-square&logo=ros&logoColor=white)
![Raspberry Pi](https://img.shields.io/badge/Raspberry_Pi-A22846?style=flat-square&logo=raspberrypi&logoColor=white)
![NVIDIA](https://img.shields.io/badge/Jetson_Nano-76B900?style=flat-square&logo=nvidia&logoColor=white)

**Tools & Infra**

![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GCP](https://img.shields.io/badge/GCP-4285F4?style=flat-square&logo=googlecloud&logoColor=white)
![Azure](https://img.shields.io/badge/Azure_AI-0089D6?style=flat-square&logo=microsoftazure&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)

**Languages**

![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)

---

## Recognition

- **First-author paper under review at COLM 2026** — Knowledge Distillation: A Minimum-Width Theorem (Erdős AI Lab)
- **Published journal paper** — A Systematic Deep Learning Framework for PCOS Detection Using Deduplicated Ultrasound Images
- **India AI Impact Summit 2026** — Represented Dayananda Sagar University; presented on LLM architectures, medical AI, and autonomous drones
- **Exceptional Volunteering & Community Service Award** — IEEE RAS & CIS (2025)
- **Kaggle Machine Learning Certification** (2025)
- **RapidMiner Certified Data Science Professional** (2024)

---

## Community

**AI Researcher, Erdős AI Lab** — Founding research lab focused on knowledge distillation, mechanistic interpretability, and world models. Student-founded, incubated at IIT Bombay.

**Co-Founder, RoboVerse Club** — Built a 100+ member robotics & AI community at DSU; organized 30+ technical workshops on LLMs, robotics, and edge AI.

**Tech Lead, E-Cell DSU** — Leading technology initiatives for the university startup ecosystem.

**Executive Committee Member, IEEE RAS & IEEE CIS** — Organized 5+ technical events and student research programs.

---

<div align="center">

*Always open to research collaborations, interesting problems, and good conversations about AI.*

[Portfolio](https://nileshsarkar-ai.github.io/) · [Hugging Face](https://huggingface.co/nileshsarkar-ai) · [Erdős AI Lab](https://www.erdoslab.org/)

</div>
