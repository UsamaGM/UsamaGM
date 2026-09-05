<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0d1117&height=200&section=header&text=Usama%20Mangi&fontSize=60&animation=fadeIn&fontAlignY=35&desc=Full%20Stack%20Engineer%20%7C%20AI%20%26%20LLM%20Integrations&descAlignY=55&descAlign=50" />
</div>

<p align="center">
  <a href="https://usama-mangi.tech"><img src="https://img.shields.io/badge/Location-Lahore%2C%20Pakistan-0d1117?style=flat-square&logo=googlemaps&logoColor=white" alt="Location: Lahore, Pakistan" /></a>
  &nbsp;•&nbsp;
  <a href="https://usama-mangi.tech"><img src="https://img.shields.io/badge/Portfolio-usama--mangi.tech-0d1117?style=flat-square&logo=googlechrome&logoColor=white" alt="Portfolio" /></a>
  &nbsp;•&nbsp;
  <a href="https://linkedin.com/in/usama-mangi"><img src="https://img.shields.io/badge/LinkedIn-Usama%20Mangi-0d1117?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  &nbsp;•&nbsp;
  <a href="mailto:usamamangi.tech@gmail.com"><img src="https://img.shields.io/badge/Email-usamamangi.tech%40gmail.com-0d1117?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
</p>

---

<p align="left">
  <img src="https://img.shields.io/badge/About%20Me-Developer%20Profile-0d1117?style=for-the-badge&logo=aboutdotme&logoColor=white" alt="About Me" />
</p>

Full Stack Engineer with ~18 months of production experience shipping full-stack, AI-powered products with React, Node.js, NestJS, and TypeScript, integrated with OpenAI and other LLM APIs. I've built an AI resume analyzer that scores unstructured PDFs at 92% accuracy, an automated LLM-based code review bot, and multiple production-ready SaaS platforms. My current focus is on **applied AI and computer vision** — self-supervised learning for geospatial imagery and generative pipelines for image restoration — alongside backend performance work in TypeScript.

- **[BUILD]** Currently building **Interviewer AI** — an AI-powered technical interview platform (dynamic question generation + response scoring)
- **[LEARN]** Learning: edge-runtime backend performance (Hono vs Node/Express), diffusion-based image editing, self-supervised pretraining for segmentation
- **[STACK]** Comfortable across the stack: React/TypeScript/NestJS on the frontend and backend, Python/PyTorch for ML, Docker + Linux for deployment
- **[WRITE]** Published: an open-source Hono-vs-Express benchmark on Bun (8.2x throughput, 53x lower latency) — see project below
- **[OPEN]** Open to collaborating on applied CV or LLM-integration projects
- **[NOTE]** Fun fact: my Neovim config has had more commits than some of my class projects

---

<p align="left">
  <img src="https://img.shields.io/badge/Featured%20Projects-Selected%20Work-0d1117?style=for-the-badge&logo=github&logoColor=white" alt="Featured Projects" />
</p>

### Eco Restoration AI
Generative pipeline for digitally restoring images of polluted or degraded landscapes. A multi-stage architecture: **YOLOv8** for initial object detection, **SAM** for refined mask generation with IoU-based fallback, **DeepLabV3+ (EfficientNet-B4)** and **CLIPSeg** for semantic segmentation, and **Stable Diffusion inpainting** for realistic scene restoration. Includes CLIP-based scene classification for context-aware prompts (grass, road, beach, etc.). Ships with dataset preparation tools (TACO, UAV, ZeroWaste downloads), model training scripts, and a FastAPI server with server-sent events for real-time processing feedback.

`Python` `PyTorch` `YOLOv8` `SAM` `CLIPSeg` `Stable Diffusion` `DeepLabV3+` `FastAPI`

<a href="https://github.com/usama-mangi/eco-restoration"><img src="https://img.shields.io/badge/Repo-eco--restoration-0d1117?style=flat-square&logo=github&logoColor=white" alt="eco-restoration" /></a>

---

### Solar Segmentation — Self-Supervised Learning
Geospatial segmentation system for solar panel detection from satellite imagery using self-supervised pretraining to reduce reliance on large labeled datasets. Implements both **SimCLR** and **MoCo** SSL methods to pretrain ResNet50 encoders on unlabeled satellite images, then fine-tunes a custom U-Net decoder for binary segmentation. Includes distributed data-parallel (DDP) training with AMP and gradient checkpointing, a Gradio-based interactive annotation app using SAM, and inference comparison scripts for evaluating MoCo vs SimCLR pretrained models.

`Python` `PyTorch` `SimCLR` `MoCo` `ResNet50` `U-Net` `SAM` `OpenCV` `Gradio`

<a href="https://github.com/usama-mangi/solar-segmentation-annotation-ssl"><img src="https://img.shields.io/badge/Repo-solar--segmentation--annotation--ssl-0d1117?style=flat-square&logo=github&logoColor=white" alt="solar-segmentation-annotation-ssl" /></a>

---

### Hono vs Express — Edge Runtime Benchmark
Performance benchmark comparing Hono and Express.js web frameworks under identical conditions. Both implementations feature the same MVC-structured REST API for video CRUD with MongoDB/Mongoose integration. Results from Autocannon load tests:

| Metric | Hono (Bun) | Express 5 (Bun) | Delta |
|---|---|---|---|
| Throughput (req/sec) | **30,995** | 3,776 | **8.2x** |
| Latency (avg) | **0.04 ms** | 2.13 ms | **53.25x lower** |
| Throughput (MB/s) | **4.25** | 1.55 | **2.7x** |

`TypeScript` `Hono` `Express 5` `Bun` `MongoDB` `Autocannon`

<a href="https://github.com/usama-mangi/hono-vs-express"><img src="https://img.shields.io/badge/Repo-hono--vs--express-0d1117?style=flat-square&logo=github&logoColor=white" alt="hono-vs-express" /></a>

---

### Interviewer AI
AI-powered technical interview platform that streamlines the hiring workflow. Generates dynamic technical questions and scores candidate responses via an LLM pipeline (OpenRouter routing to DeepSeek Chat). Includes AI-based candidate assessments, quick AI feedback on answers, interview scheduling with timezone handling, multi-role user management (candidates, recruiters, admins), and JWT-secured authentication. The scoring pipeline checks correctness, depth, and communication quality of candidate answers.

`React 19` `TypeScript` `Express` `MongoDB` `OpenRouter API` `DeepSeek` `JWT` `MUI`

<a href="https://github.com/usama-mangi/interview-ai"><img src="https://img.shields.io/badge/Repo-interview--ai-0d1117?style=flat-square&logo=github&logoColor=white" alt="interview-ai" /></a>

---

### Neovim Config
Personal Lua-based Neovim configuration — LSP, custom keymaps, Treesitter, and plugin setup tuned for daily development speed. Built on lazy.nvim with Mason-managed LSP servers.

`Lua` `Neovim` `LSP` `Treesitter` `lazy.nvim`

<a href="https://github.com/usama-mangi/neovim-setup"><img src="https://img.shields.io/badge/Repo-neovim--setup-0d1117?style=flat-square&logo=github&logoColor=white" alt="neovim-setup" /></a>

---

<p align="left">
  <img src="https://img.shields.io/badge/Tech%20Stack-Tools%20%26%20Languages-0d1117?style=for-the-badge&logo=stackshare&logoColor=white" alt="Tech Stack" />
</p>

**Core**
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=next.js&logoColor=white)
![React Native](https://img.shields.io/badge/React%20Native-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![Hono](https://img.shields.io/badge/Hono-E36002?style=flat-square&logo=hono&logoColor=white)
![Bun](https://img.shields.io/badge/Bun-000000?style=flat-square&logo=bun&logoColor=white)

**AI / Data**
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white)

**Databases & Infrastructure**
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white)

**Systems & Tools**
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Neovim](https://img.shields.io/badge/Neovim-57A143?style=flat-square&logo=neovim&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05033?style=flat-square&logo=git&logoColor=white)

---

<p align="left">
  <img src="https://img.shields.io/badge/Background-Education%20%26%20Experience-0d1117?style=for-the-badge&logo=googlescholar&logoColor=white" alt="Background" />
</p>

**Full-Stack AI Engineer** at **ZynSols** · Aug 2025 – May 2026 · Sukkur, Pakistan

**Bachelor of Science — Computer Science**, Sukkur IBA University · Sep 2022 – May 2026 · GPA 3.2

Previously: React Native App Developer Intern at Indus Tech Nexus (Jun–Jul 2026); Open-Source Contributor at GirlScript Summer of Code (Oct–Nov 2024).

---

<p align="left">
  <img src="https://img.shields.io/badge/GitHub-Stats%20%26%20Activity-0d1117?style=for-the-badge&logo=github&logoColor=white" alt="GitHub Stats" />
</p>

<p align="center">
  <a href="https://github.com/usama-mangi"><img src="https://img.shields.io/badge/GitHub-usama--mangi-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub Profile" /></a>
  <a href="https://github.com/usama-mangi?tab=repositories"><img src="https://img.shields.io/badge/Projects-30%2B-0d1117?style=for-the-badge&logo=github&logoColor=white" alt="Projects" /></a>
  <a href="https://github.com/usama-mangi"><img src="https://img.shields.io/badge/Open%20Source-Contributor-0d1117?style=for-the-badge&logo=opensourceinitiative&logoColor=white" alt="Open Source" /></a>
</p>

<p align="center"><sub>Live GitHub stats widgets (github-readme-stats / streak-stats) are omitted intentionally — the public instances return 503 intermittently and there is no reliable public mirror. Self-host anuraghazra/github-readme-stats if you want the live widgets back.</sub></p>

---

<p align="left">
  <img src="https://img.shields.io/badge/Connect-Get%20in%20Touch-0d1117?style=for-the-badge&logo=probot&logoColor=white" alt="Connect" />
</p>

<p align="center">
  <a href="https://usama-mangi.tech">Portfolio</a> &nbsp;•&nbsp;
  <a href="https://linkedin.com/in/usama-mangi">LinkedIn</a> &nbsp;•&nbsp;
  <a href="mailto:usamamangi.tech@gmail.com">Email</a>
</p>

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0d1117&height=100&section=footer" width="100%"/>
</div>
