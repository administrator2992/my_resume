# Target Pekerjaan & Pemetaan CV (JOB_PROFILE.md)

> **Tujuan:** Tempat menempelkan Job Description (JD) target dan memetakannya ke
> `PROFILE.md` agar `main_cv.tex` bisa dioptimalkan (ATS + XYZ) untuk lowongan itu.
> **Cara pakai:** Isi Bagian 1 (paste JD apa adanya). Agen mengisi Bagian 2–5.
> Aturan optimasi mengikuti `AGENTS.md` & `skills.md`. Satu file = satu target;
> arsipkan target lama ke Bagian 6 sebelum mengganti.

---

## 1. INPUT — Detail Lowongan (diisi USER)
* **Nama Perusahaan/Institusi:** AI.DECE
* **Posisi yang Dilamar:** Senior AI Engineer
* **Lokasi / Remote:** Jakarta, Indonesia
* **Bahasa CV target:** EN
* **Jenis target:** Industri
* **Link lowongan (opsional):** [AI.DECE](https://glints.com/id/opportunities/jobs/senior-ai-engineer/1133c720-36b6-474e-972f-e679227751e9?shareId=15efa2ba-aa60-4df0-80fb-e4899921ac2a)

### Job Description (paste mentah di sini)
```text
AI.DECE (AI Development Center) is looking for a talented Senior AI Engineer to join our growing team. If you are passionate about Artificial Intelligence, Large Language Models, and building scalable AI solutions, we would love to hear from you.

Responsibilities
Lead AI solution development and implementation.
Design and build scalable AI systems.
Develop and optimize LLM-powered applications.
Fine-tune AI models and improve model performance.
Design AI architecture and deployment pipelines.
Mentor junior AI engineers.
Collaborate with product and business teams.
Research and implement the latest AI technologies.
Ensure AI systems are scalable, secure, and production-ready.
Qualifications
Bachelor’s Degree in Computer Science, AI, Software Engineering, or related fields.
Strong Python Programming Skills.
Minimum 1+ Year Experience in AI / Machine Learning Development.
Experience with TensorFlow, PyTorch, and Hugging Face.
Experience with Large Language Models (GPT, Claude, Gemini, Llama).
Experience with RAG, Vector Database, LangChain, and LangGraph.
Strong Backend Development Skills (FastAPI, Flask, Django).
Experience deploying AI applications into production environments.
Strong Leadership and Problem-Solving Skills.
```

## 2. KEYWORD EXTRACTION (filled by AGENT from JD)
* **Hard Skills (technical):**
  | Keyword from JD | In PROFILE.md? | Evidence / Relevant Experience |
  |---|---|---|
  | Python Programming | Yes | Python used for deep learning research, model optimization, web backend, and scraping scripts. |
  | TensorFlow & PyTorch | Yes | Used for model building, quantization, and RA Edge AI research. |
  | Large Language Models (LLM) | Yes | Engineered scheduling agents using Ollama (Ministral-3B) and designed vector semantic cache using OpenRouter (GPT-4o-mini/Llama-3). |
  | RAG, Vector DB, LangChain | Yes | Designed Supabase Vector Memory (pgvector cosine similarity) and designed agentic scheduling flows. |
  | Backend (FastAPI, Flask, Django)| Yes | Designed Python/Flask backend APIs (Teaching Assistant) and Node.js/Express APIs (IoT Engineer). |
  | Deployment & Production | Yes | Developed containerized services using Docker for local testing and remote web deployment. |
  | Machine Learning & Deep Learning | Yes | RA at AMIKOM on YOLOv4 quantization and edge AI inference optimizations. |
  | Redis | Yes | Configured Redis cache under work experience / skills profile. |

* **Soft Skills:**
  | Keyword from JD | In PROFILE.md? | Evidence / Relevant Experience |
  |---|---|---|
  | Leadership & Mentoring | Yes | Teaching Assistant at AMIKOM instructing 40+ students; Secretary of CE student community managing workshops. |
  | Problem-solving & Troubleshooting | Yes | Maintained industrial automation machinery at Banwibu; resolved hardware resource constraints on Jetson devices. |
  | Collaboration | Yes | Collaborated with international academic researchers (University of Georgia, UGM) and product engineers. |

* **Must-have vs. Nice-to-have Requirements:**
  * Must-have: Python programming, 1+ year AI/ML experience, TensorFlow/PyTorch, LLMs, RAG, Backend development, Docker deployment.
  * Nice-to-have: Mentorship, FastAPI/Flask/Django expertise.

---

## 3. FIT ANALYSIS (Gap Analysis)
* **Strengths (highlight in CV):**
  * Strong AI/ML and Deep Learning credentials (RA at AMIKOM, publications in IEEE ICFEC 2026/CCGrid).
  * Direct LLM application engineering (AI-LINE scheduling agent using Ollama, POLL Smart Inventory using OpenRouter + pgvector).
  * Backend developer capabilities (API development, database design, Redis caching, Docker).
  * Secondary jobdesk at Banwibu as an AI Engineer, directly bridging IoT and Machine Learning.
* **Gaps / Weaknesses (mitigation strategy):**
  * The position title is "Senior AI Engineer". The candidate is junior-to-mid, but satisfies the qualifications requirement of "Minimum 1+ Year Experience" and strong Python/LLM background. Mitigation: Showcase highly technical metrics (XYZ) and leadership (TA, community secretary) to prove readiness for mid-to-senior responsibilities.
* **Irrelevant Experience (hide/minimize):**
  * Minimized purely administrative details and pure hardware PCB details to focus on Python, Redis, ML, DL, and Backend/API development.
* **Match Estimation:** Very Good. The candidate has direct, hands-on experience building, optimizing, and deploying LLM applications, matching the core qualifications of the role.

---

## 4. CV EDIT PLAN (main_cv.tex)
* **Professional Summary (1-2 sentences):**
  > A Computer Science graduate in Computer Engineering specializing in Artificial Intelligence and Machine Learning. Experienced in building and deploying scalable AI pipelines, engineering LLM-powered applications, and designing backend API services using Python and C/C++.
* **Experiences & XYZ Metrics:**
  1. **IoT & AI Engineer (Banwibu)**:
     - Delivered Node.js backend API gateways and configured relational database schemas (MariaDB, SQLite, Redis) for real-time transaction processing.
     - Developed containerized application configurations using Docker to streamline testing and deployment of integrated hardware-software services.
     - Maintained and troubleshot industrial automation machinery in a Linux environment (99.8% uptime), configuring serial communication and ESP32 controllers.
  2. **Research Assistant (Online)**:
     - Achieved 40% power efficiency for deep learning inference on NVIDIA Jetson Xavier NX edge devices, by optimizing hardware resource allocation via Python-based CORAL framework.
     - Published collaborative research on Edge AI in IEEE ICFEC 2026, writing clean, maintainable Python code and documenting distributed cloud-edge architecture schemas.
  3. **Research Assistant (Onsite)**:
     - Increased YOLOv4 model inference speed by 3x on edge devices (Jetson/Raspberry Pi), implementing post-training quantization and ONNX runtime optimizations in Python.
     - Reduced data pre-processing latency by 20% by designing efficient Python pipelines to curate over 4,000 high-quality images.
  4. **Exchange Student (ITB)**:
     - Improved poultry environment monitoring accuracy by 15%, programming automated sensor data acquisition and local SQL logging on an ESP32 microcontroller during the ITB exchange.
* **Projects (Highlighting LLMs, scraping, and Edge AI):**
  - **POLL Smart Inventory (Ongoing)**: Designing an AI-powered smart inventory system integrating OpenRouter (GPT-4o-mini/Llama-3-8B-Instruct) and Supabase Vector Memory (pgvector) to implement semantic caching for auto-categorization.
  - **AI-LINE (Intelligent Scheduling Agent)**: Developed an LLM-based intelligent scheduling agent integrating LINE Messenger API, Ollama (Ministral-3B), and Supabase, implementing strict prompt safety rules to eliminate hallucinations and UTC conversion.
  - **Lulabid (Japanese Product Search Engine)**: Designed a multi-site parallel data extraction pipeline (Lulabid) using Node.js for Japanese e-commerce data extraction, implementing anti-bot bypass mechanisms and HTML sanitization.
* **Sections Trimmed/Optimized:** Removed JIRA, Confluence, and Puppeteer from skills. Word count targeted: 600 words.

---

## 5. EXECUTION CHECKLIST (according to AGENTS.md)
- [x] Contact information: Email, Phone, LinkedIn included.
- [x] >= 5 bullet points with measurable XYZ metrics.
- [x] Hard/soft skills from JD naturally integrated into experience.
- [x] Free of first-person pronouns, clichés, or buzzwords (anti-fluff).
- [x] Word count fits target (475 - 600 words for industry).
- [x] CV language matches target (English).
- [x] Git branch name: `cv/aidece-seniorai-2026`.
- [ ] Compilation: Done locally.
- [ ] Commit/push: Only if requested.
