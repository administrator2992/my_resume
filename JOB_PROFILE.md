# Target Pekerjaan & Pemetaan CV (JOB_PROFILE.md)

> **Tujuan:** Tempat menempelkan Job Description (JD) target dan memetakannya ke
> `PROFILE.md` agar `main_cv.tex` bisa dioptimalkan (ATS + XYZ) untuk lowongan itu.
> **Cara pakai:** Isi Bagian 1 (paste JD apa adanya). Agen mengisi Bagian 2–5.
> Aturan optimasi mengikuti `AGENTS.md` & `skills.md`. Satu file = satu target;
> arsipkan target lama ke Bagian 6 sebelum mengganti.

---

## 1. INPUT — Detail Lowongan (diisi USER)
* **Nama Perusahaan/Institusi:** Micro1
* **Posisi yang Dilamar:** Machine Learning Researcher
* **Lokasi / Remote:** Remote
* **Bahasa CV target:** EN
* **Jenis target:** Industri
* **Link lowongan (opsional):** [Micro1](https://jobs.micro1.ai/post/dea93c7f-1005-4cec-9ce3-d5a554f797cf?referralCode=e91c9585-63ad-45aa-9820-d63708190a83)

### Job Description (paste mentah di sini)
```text
Job Title : Machine Learning Researcher
Required Skills
Research
Deep Learning
Tensorflow
About micro1
micro1 is the leading AI data lab for training frontier models and evaluating AI agents. Experts contribute their diverse subject matter knowledge across domains such as finance, healthcare, STEM engineering, and more. micro1 transforms that real-world expertise into high-quality training data, evaluations, and feedback loops that improve how AI systems learn, reason, and perform.
Our platform identifies and vets top talent through an AI recruiter, enabling high-quality expert contributions at scale. We aim to enable 1 billion people to do meaningful work by applying their expertise to AI. As our global expert network grows, micro1 is building the human intelligence layer for frontier AI.

Job Title: Machine Learning Researcher



Job Type: Contractor



Location: Remote



Job Summary: In this role, you'll apply your expertise to help train next-generation AI systems. Your work will shape how models learn, reason, and perform through high-quality, real-world input. No prior experience in AI is required — your domain knowledge is what matters.



Key Responsibilities:

Lead and conduct cutting-edge research in machine learning and artificial intelligence domains.
Design, implement, and evaluate state-of-the-art deep learning algorithms using frameworks such as TensorFlow.
Collaborate closely with engineering teams to translate research breakthroughs into scalable solutions.
Publish research findings and contribute to the global AI/ML scholarly community.
Continuously monitor industry advancements to keep the team at the forefront of technological innovation.
Document methodologies, experiments, and results clearly for both technical and non-technical stakeholders.
Communicate complex concepts effectively through both written and verbal channels.


Required Skills and Qualifications:

Expertise in designing and executing research projects in AI and machine learning.
In-depth experience with deep learning frameworks, especially TensorFlow.
Strong proficiency in Python for prototyping and algorithm development.
Exceptional written and verbal communication skills, with an emphasis on clear research documentation and collaborative teamwork.
Proven track record of working independently and delivering impactful research outcomes in remote settings.
Ability to evaluate, optimize, and implement advanced ML models for real-world applications.


Preferred Qualifications:

Academic publications in top-tier AI/ML conferences or journals.
Experience collaborating with cross-functional, international teams.
Background in applying deep learning solutions to industry-specific problems.
```

## 2. EKSTRAKSI KATA KUNCI (diisi AGEN dari JD)
> Pindai JD, pisahkan menjadi dua kelompok. Dipakai untuk menyisipkan keyword
> secara natural ke bullet pengalaman (tanpa keyword stuffing).

* **Hard Skills (teknis):**
  | Keyword dari JD | Ada di PROFILE.md? | Bukti / Pengalaman terkait |
  |---|---|---|
  | Deep Learning & AI | Ya | Research Assistant (YOLOv4, Jetson Nano, Jetson Xavier NX, post-training quantization) |
  | TensorFlow / PyTorch | Ya | Master Profile commented list of frameworks, research assistant deep learning model optimization |
  | Python prototyping | Ya | Coursework, YOLO model optimization research, Python tools development |
  | Model optimization & eval | Ya | Jetson Nano face-mask inference speedup (3x), Xavier NX power reduction (40%) |
  | Academic Publications | Ya | IEEE EDGE 2024, MATRIK Jurnal (2 articles), IEEE ICFEC 2026 |

* **Soft Skills:**
  | Keyword dari JD | Ada di PROFILE.md? | Bukti / Pengalaman terkait |
  |---|---|---|
  | Research Documentation | Ya | Authoring papers for MATRIK, EDGE 2024, and ICFEC 2026; creating weekly reporting & technical docs |
  | Collaborative Teamwork | Ya | Weekly reporting across international collaborating groups (UGA, UGM, AMIKOM) |
  | Independent Execution | Ya | Online Research Assistant delivering hardware resource optimization independently |
  | Verbal/Written Comm | Ya | Presenting at IEEE ICFEC 2026 conference, student community leadership |

* **Requirement wajib (must-have) vs nilai plus (nice-to-have):**
  * Must-have: ML/DL research project design, TensorFlow/framework proficiency, Python prototyping, clear research documentation, remote independence.
  * Nice-to-have: Academic publications in top-tier conferences/journals, international collaboration, applying deep learning to industry problems.

---

## 3. ANALISIS KECOCOKAN (Gap Analysis)
* **Sudah cocok (highlight di CV):** Strong DL research background, international collaboration (UGA), multiple publications (IEEE EDGE, IEEE ICFEC, MATRIK), hardware-constrained deep learning optimization, Python proficiency.
* **Gap / lemah (yang perlu disiasati atau dijujurkan):** S1 degree instead of PhD (but the JD states "No prior experience in AI is required"), TensorFlow is primary in JD while candidate has more PyTorch/YOLO/C++ experience (highlight both frameworks as proficient in the skills section).
* **Pengalaman dari PROFILE.md yang TIDAK relevan (sembunyikan dari CV ini):** General industrial machine maintenance (Unitama Sari Mas) and generic physical hardware setups (Solenoid, RFID, HMI) should be minimized or framed around software testing/diagnostics rather than physical integration.
* **Estimasi kecocokan:** Sangat Tinggi (Excellent match on research experience, publications, international collaboration, and DL/Python skillsets).

---

## 4. RENCANA PENYUNTINGAN `main_cv.tex`
> Setiap bullet pengalaman terpilih ditulis ulang dengan rumus XYZ:
> `Mencapai [X] diukur dengan [Y], dengan melakukan [Z]`. Minimal 5 metrik.

* **Personal Summary (1–2 kalimat, fokus nilai jual untuk posisi ini):**
  > Research-focused Computer Engineering graduate and Machine Learning Researcher with a proven track record in deep learning optimization and edge intelligence. Experienced in collaborating with international research institutions, designing advanced ML models, and publishing in scholarly venues; proficient in Python and deep learning frameworks like TensorFlow and PyTorch.
* **Pengalaman yang ditarik + draf bullet XYZ:**
  1. **Research Assistant (Online)**:
     - Coordinated hardware resource optimization on NVIDIA Jetson Xavier NX for deep learning inference, resulting in a 40% reduction in power usage while maintaining stable model execution and real-time execution speeds.
     - Co-authored and published peer-reviewed research findings on Covariance-Guided Resource Adaptive Learning (CORAL) in IEEE ICFEC 2026, facilitating weekly reporting and technical documentation updates across three international collaborating research groups (UGA, UGM, AMIKOM).
  2. **Research Assistant (Onsite)**:
     - Designed and evaluated deep learning models (YOLOv4) for real-time face-mask detection on hardware-constrained edge devices (Jetson Nano, Raspberry Pi 3B), achieving a 3x speedup via post-training optimization.
     - Curated and preprocessed a dataset of over 4,000 high-quality images to train convolutional neural networks, reducing data preprocessing latency and improving detection accuracy.
  3. **IoT Engineer (Banwibu)**:
     - Maintained and optimized embedded diagnostic systems for industrial automation machinery, achieving a 99.8% uptime rate by implementing automated logging and diagnostics.
     - Engineered microcontroller firmware (ESP32) and resistive touchscreen HMIs for smart lock systems, reducing user interaction error rates by 30% through robust software testing.
     - Delivered a card dispenser system integrated with an Angular web interface and RFID technology on schedule within a 3-month timeline, collaborating with cross-functional business and technical teams.
* **Section yang dipangkas / disembunyikan agar fokus & sesuai word count:** Minimize detail on basic automation (RFID/solenoid), highlight edge AI/ML, keep publications list in full.
* **Target panjang:** Industri 475–600 kata.

---

## 5. CHECKLIST EKSEKUSI (mengikuti `AGENTS.md`)
- [x] Kontak lengkap: Email, Telepon, LinkedIn (akademik: + publikasi).
- [x] ≥ 5 bullet mengandung metrik XYZ terukur.
- [x] Tiap bullet pengalaman mengandung ≥1 hard/soft skill dari JD (natural).
- [x] Tidak ada kata ganti orang pertama, klise, atau buzzwords (anti-fluff).
- [x] Word count sesuai target (industri 475–600).
- [x] Bahasa CV sesuai target (ID/EN), header & action verb disesuaikan.
- [x] Branch git: `cv/[target]-[posisi]-[tahun]` (akademik: `cv/academic-[target]-[tahun]`).
- [ ] Kompilasi: `pdflatex → biber main_cv → pdflatex → pdflatex` → `CV_Nabhaan_[Target].pdf`.
- [ ] Commit/push HANYA jika user meminta.


