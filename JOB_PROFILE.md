# Target Pekerjaan & Pemetaan CV (JOB_PROFILE.md)

> **Tujuan:** Tempat menempelkan Job Description (JD) target dan memetakannya ke
> `PROFILE.md` agar `main_cv.tex` bisa dioptimalkan (ATS + XYZ) untuk lowongan itu.
> **Cara pakai:** Isi Bagian 1 (paste JD apa adanya). Agen mengisi Bagian 2–5.
> Aturan optimasi mengikuti `AGENTS.md` & `skills.md`. Satu file = satu target;
> arsipkan target lama ke Bagian 6 sebelum mengganti.

---

## 1. INPUT — Detail Lowongan (diisi USER)
* **Nama Perusahaan/Institusi:** PT Intecs Teknikatama Industri
* **Posisi yang Dilamar:** System Engineer - IoT & Edge Computing
* **Lokasi / Remote:** Jakarta, Indonesia
* **Bahasa CV target:** EN
* **Jenis target:** Industri
* **Link lowongan (opsional):** [PT Intecs Teknikatama Industri](https://www.linkedin.com/jobs/collections/similar-jobs/?currentJobId=4432331730&origin=BYV_SIMILAR_JOBS_EMAIL&referenceJobId=4429035481)

### Job Description (paste mentah di sini)
```text
Job Requirements :



Bachelor’s Degree in Computer Engineering, Electrical Engineering, Informatics Engineering, Information Systems, or related field.
Strong knowledge of Linux operating systems and system administration.
5 years Experience in software development using Golang and/or Python.
Familiarity with C/C++, JavaScript/TypeScript, or other programming languages is an advantage.
Familiar with Single Board Computers (SBC), Industrial PCs, and Edge Computing Devices such as Raspberry Pi, Orange Pi, BeagleBone, Advantech, Moxa, or similar industrial computing platforms.
Understanding of networking concepts including TCP/IP, VPN, Firewall, SSH, and Remote Access.
Experience with Docker, containerized applications, and deployment environments.
Understanding of IoT architecture, edge computing, and distributed systems.
Familiar with communication protocols such as MQTT, HTTP/HTTPS, TCP/IP, Modbus, Serial Communication, or CAN Bus.
Experience with database systems such as PostgreSQL, MySQL, SQLite, or other relational databases is an advantage.
Familiar with Git version control and software development lifecycle (SDLC).
Strong analytical, problem-solving, and troubleshooting skills in both hardware and software environments.
Good communication skills and ability to work independently or as part of a multidisciplinary team.
Willing to travel and provide technical support for project implementation when required.



Job Description :



Develop, configure, and maintain Linux-based systems for industrial and digital solutions.
Design, deploy, and manage edge computing platforms and IoT gateway devices.
Develop applications and services using Golang, Python, and other relevant technologies.
Configure, deploy, and maintain Single Board Computers (SBC), Industrial PCs, and Edge Computing Devices.
Implement communication between devices, sensors, gateways, and cloud/on-premise platforms.
Develop and maintain data acquisition, processing, and transmission services from field devices to central systems.
Perform system integration, testing, troubleshooting, and performance optimization for IoT and edge computing solutions.
Support deployment, commissioning, and technical investigations for digital solution projects.
Prepare technical documentation, installation procedures, and system architecture documentation.
Collaborate with software engineers, project engineers, and principals to develop and implement digital solutions.
```

## 2. KEYWORD EXTRACTION (filled by AGENT from JD)
* **Hard Skills (technical):**
  | Keyword from JD | In PROFILE.md? | Evidence / Relevant Experience |
  |---|---|---|
  | Linux operating systems & admin | Yes | Operating systems coursework, Linux used extensively in research, Jetson setups, and SBC configs. |
  | Golang and/or Python | Yes | Python used for AI research, YOLOv4/YOLOv11 optimization, and image pre-processing. (Golang not present, Python is primary). |
  | C/C++ or JavaScript/TypeScript | Yes | Developed ESP32 firmware in C++, YDU USB I/O firmware in C++, and Angular/Node.js web application frontend/backend. |
  | Single Board Computers (SBC) & Edge | Yes | Integrated solutions on Raspberry Pi 4/3B, Orange Pi AI Pro, NVIDIA Jetson, and Rockchip platforms. |
  | Networking (TCP/IP, VPN, SSH) | Yes | Coursework in Computer Networks, configured SSH/remote access for SBCs, and networking protocols. |
  | Docker & containerization | Yes | Docker listed under full-stack/backend skills; containerized hardware-software application setups. |
  | IoT Architecture & Edge Computing | Yes | Thesis/specialization in IoT Systems, assistant for Industrial IoT, and Edge Computing research projects. |
  | Protocols (MQTT, Modbus, Serial) | Yes | Configured UART, SPI, I2C, RS485, Modbus, MQTT, TCP/IP, UDP, BLE, and WebSocket. |
  | Relational Databases | Yes | Designed and managed MariaDB, SQLite, and PostgreSQL (Supabase) database schemas. |
  | Git & SDLC | Yes | Used Git for version control in academic and professional development team environments. |

* **Soft Skills:**
  | Keyword from JD | In PROFILE.md? | Evidence / Relevant Experience |
  |---|---|---|
  | Problem-solving & troubleshooting | Yes | Debugged electronic smart locks and industrial machinery automation systems at Banwibu. |
  | Collaboration & Teamwork | Yes | Collaborated with international academic researchers (University of Georgia, UGM) and QA/software teams. |
  | Willing to travel & support | Yes | Active student exchange across multiple universities in Indonesia; hands-on on-site technical support background. |

* **Must-have vs. Nice-to-have Requirements:**
  * Must-have: Linux knowledge, Python programming, SBC/Edge experience, networking/protocols, Docker, relational databases.
  * Nice-to-have: Golang programming, 5 years experience (candidate is junior-mid with ~1-2 years experience, mitigated by strong Python/SBC engineering competence).

---

## 3. FIT ANALYSIS (Gap Analysis)
* **Strengths (highlight in CV):**
  * Practical expertise in SBCs and Edge Computing (NVIDIA Jetson, Orange Pi AI Pro, Raspberry Pi).
  * Robust Python and C/C++ programming background.
  * Practical experience with Linux systems administration, Docker containerization, and relational databases.
  * Heavy exposure to industrial communication protocols (Modbus, MQTT, RS485, Serial, TCP/IP).
* **Gaps / Weaknesses (mitigation strategy):**
  * Job requires 5 years experience (candidate has ~1-2 years). Mitigation: Do not forge experience; instead, focus on highly impactful metrics (XYZ) and real-world industrial troubleshooting and publication history to prove capabilities.
  * Job mentions Golang. Mitigation: Highlight Python as the primary language and C/C++ as an advantage, showing strong foundations in software design and API integrations.
* **Irrelevant Experience (hide/minimize):**
  * Minimized purely administrative details and pure web application frontend details.
* **Match Estimation:** Good. The candidate is a strong fit for the technical requirements (Linux, SBCs, Docker, Python, protocols), making them a very viable junior-to-mid System Engineer candidate.

---

## 4. CV EDIT PLAN (main_cv.tex)
* **Professional Summary (1-2 sentences):**
  > A Computer Science graduate in Computer Engineering specializing in IoT systems and Edge Computing. Experienced in deploying containerized applications, configuring device communication protocols, administering Linux environments, and developing Python/C++ code for industrial edge computing platforms.
* **Experiences & XYZ Metrics:**
  1. **IoT/Software Engineer (Banwibu)**:
     - Delivered a web-integrated card dispenser system on schedule within 3 months, by configuring Node.js RESTful APIs and database schemas (MariaDB, SQLite) for real-time processing.
     - Maintained and troubleshot industrial automation machinery in a Linux environment (99.8% uptime), configuring serial communication (RS485, Modbus) and ESP32 controllers.
     - Developed containerized application configurations using Docker to support local testing and deployment of integrated hardware-software services.
  2. **Research Assistant (Online)**:
     - Achieved 40% power efficiency for deep learning inference on NVIDIA Jetson Xavier NX edge devices, by optimizing hardware resource allocation via Python-based CORAL framework.
     - Published collaborative research on Edge AI in IEEE ICFEC 2026, writing clean, maintainable Python code and documenting distributed cloud-edge architecture schemas.
  3. **Research Assistant (Onsite)**:
     - Increased YOLOv4 model inference speed by 3x on edge devices (Jetson Nano, Raspberry Pi 3B), implementing post-training quantization and ONNX runtime optimizations in Python.
     - Reduced data pre-processing latency by 20% by designing efficient Python data pipelines to curate and pre-process over 4,000 high-quality images.
  4. **Exchange Student (ITB)**:
     - Improved environment monitoring accuracy by 15%, programming automated sensor data acquisition and local database logging on an ESP32 microcontroller during the ITB exchange.
* **Sections Trimmed/Optimized:** Heavy emphasis on SBCs, Linux, Docker, databases, and protocols.
* **Target Word Count:** ~535 words.

---

## 5. EXECUTION CHECKLIST (according to AGENTS.md)
- [x] Contact information: Email, Phone, LinkedIn included.
- [x] >= 5 bullet points with measurable XYZ metrics.
- [x] Hard/soft skills from JD naturally integrated into experience.
- [x] Free of first-person pronouns, clichés, or buzzwords (anti-fluff).
- [x] Word count fits target (475 - 600 words for industry).
- [x] CV language matches target (English).
- [x] Git branch name: `cv/intecs-systemengineer-2026`.
- [ ] Compilation: Done locally.
- [ ] Commit/push: Only if requested.
