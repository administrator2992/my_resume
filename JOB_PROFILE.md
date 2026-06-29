# Target Pekerjaan & Pemetaan CV (JOB_PROFILE.md)

> **Tujuan:** Tempat menempelkan Job Description (JD) target dan memetakannya ke
> `PROFILE.md` agar `main_cv.tex` bisa dioptimalkan (ATS + XYZ) untuk lowongan itu.
> **Cara pakai:** Isi Bagian 1 (paste JD apa adanya). Agen mengisi Bagian 2–5.
> Aturan optimasi mengikuti `AGENTS.md` & `skills.md`. Satu file = satu target;
> arsipkan target lama ke Bagian 6 sebelum mengganti.

---

## 1. INPUT — Detail Lowongan (diisi USER)
* **Nama Perusahaan/Institusi:** PT Mitech
* **Posisi yang Dilamar:** IoT Engineer
* **Lokasi / Remote:** Jakarta, Indonesia
* **Bahasa CV target:** EN
* **Jenis target:** Industri
* **Link lowongan (opsional):** [kalibrr](https://jobseeker.kalibrr.com/c/mitech/jobs/269039/iot-engineer)

### Job Description (paste mentah di sini)
```text
Develop, implement, and maintain IoT applications for embedded systems using programming languages such as Python, C, C++, JavaScript, and Assembly.
Design and develop backend services using Node.js and APIs to enable seamless communication between IoT devices and cloud platforms.
Design, integrate, configure, and troubleshoot IoT hardware components, including microcontrollers, microprocessors, sensors, actuators, and communication modules.
Develop and optimize firmware/software for embedded devices to ensure high performance and reliability.
Implement and manage IoT communication protocols such as Wi-Fi, Bluetooth, BLE, Zigbee, LoRaWAN, RF, HTTP, MQTT, and CoAP to support secure and efficient device connectivity.
Build and maintain real-time data acquisition, synchronization, and communication between IoT devices and cloud platforms.
Design and manage SQL and NoSQL databases for IoT data storage, processing, and retrieval.
Analyze IoT-generated data to identify trends, optimize system performance, and support predictive maintenance and business insights.
Collaborate with data engineers and data scientists to implement machine learning models for intelligent IoT solutions.
Ensure IoT systems comply with cybersecurity best practices by implementing encryption, authentication, access control, and secure communication protocols.
Perform testing, debugging, performance optimization, and troubleshooting of IoT hardware and software solutions.
Collaborate with cross-functional teams, including hardware engineers, software developers, QA engineers, and business stakeholders, to deliver end-to-end IoT solutions.
Prepare technical documentation, including system architecture, integration design, API documentation, and deployment guides.
Minimum Qualifications
Programming and Software Development: Proficiency in languages such as Python, C, C++, JavaScript, and Assembly is essential for developing IoT applications and embedded systems, Knowledge of Node.js and APIs is also valuable for backend development and device communication
Hardware: Understanding microcontrollers, microprocessors, sensors, actuators, and IoT hardware components is critical. Engineers must know how to integrate and configure these devices for efficient data collection and processing. Designing and integrating sensors, processors, and network modules.
Protocols: IoT engineers should be skilled in designing and managing networks using Wi-Fi, Bluetooth, BLE, Zigbee, LoRaWAN, RF, HTTP, MQTT, and CoAP to ensure reliable device connectivity
Data Analytics: Ability to analyze large datasets from IoT devices, implement machine learning models, and extract actionable insights is crucial for predictive maintenance, operational efficiency, and smart decision-making .
Database : Familiarity with cloud services, SQL, and NoSQL databases is necessary for real-time data storage, synchronization, and IoT platform management
Cybersecurity: Knowledge of encryption, access control, and security protocols is essential to protect IoT devices and networks from unauthorized access and cyber threats
Jobs Summary
Job Level
Associate / Supervisor
Job Category
IT and Software
Educational Requirement
Bachelor's degree graduate
Office Address
2, Jalan Letjen M T Haryono, Tebet Barat Kel., Tebet
Industry
Information Technology / IT
Vacancy
1 opening
Website
https://www.mitech.co.id/
```

## 2. KEYWORD EXTRACTION (filled by AGENT from JD)
* **Hard Skills (technical):**
  | Keyword from JD | In PROFILE.md? | Evidence / Relevant Experience |
  |---|---|---|
  | Embedded Systems (C/C++, Python) | Yes | IoT Engineer at Banwibu (ESP32 firmware), Research Assistant (Jetson Nano, Raspberry Pi, Python), ITB exchange (ESP32). |
  | Backend & Node.js / APIs | Yes | Main Technical Skills: Node.js, RESTful APIs, Angular Web App integration at Banwibu. |
  | Microcontrollers (ESP32, Arduino, STM32) | Yes | Prototyped ESP32-based smart lock at Banwibu, basic understanding of STM32. |
  | Data Communication & Protocols (UART, SPI, I2C, MQTT) | Yes | Prototyped RFID dispenser at Banwibu (UART/SPI), environmental sensor (I2C) at ITB, and MQTT integration. |
  | Databases (SQL & NoSQL) | Yes | Main Technical Skills: SQLite, MariaDB, Redis, MongoDB, Firebase. |
  | Cybersecurity (Encryption, Access Control) | Yes | Technical Skills: Encryption, Access Control, secure IoT communication protocols. |
  | Hardware Integration & Troubleshooting | Yes | Troubleshooting industrial machinery at Banwibu (99.8% uptime), sensor/actuator integration. |
  | Technical Documentation | Yes | Compiling architecture documentation for ICFEC 2026, research reports, and deployment guides. |

* **Soft Skills:**
  | Keyword from JD | In PROFILE.md? | Evidence / Relevant Experience |
  |---|---|---|
  | Collaboration / Teamwork | Yes | Worked with cross-functional teams (software, hardware, QA) at Banwibu and international research groups. |
  | Problem-solving & Troubleshooting | Yes | Resolved hardware/firmware bugs at Banwibu (reducing failures by 20%), edge inference optimization. |

* **Must-have vs. Nice-to-have Requirements:**
  * Must-have: Bachelor's degree in Computer Engineering (or related), proficiency in Python/C/C++/JavaScript, understanding of microcontrollers, IoT communication protocols (MQTT, Wi-Fi, BLE, etc.), databases (SQL/NoSQL).
  * Nice-to-have: Node.js backend development, data analytics/ML, cybersecurity best practices.

---

## 3. FIT ANALYSIS (Gap Analysis)
* **Strengths (highlight in CV):**
  * Bachelor's degree in Computer Engineering with 3.88 GPA.
  * Professional experience as an IoT Engineer at Banwibu designing PCB circuits, ESP32 firmware, HMI, and integrating Node.js backends.
  * Hands-on knowledge of protocols (UART, SPI, I2C, MQTT, TCP/IP, BLE) and hardware (ESP32, Jetson, Raspberry Pi).
  * Academic publication track record in Edge AI and resource optimization.
* **Gaps / Weaknesses (mitigation strategy):**
  * STM32 knowledge is basic. Mitigation: Emphasize broad microcontroller proficiency (ESP32, Arduino, Jetson, Raspberry Pi) and list STM32 as basic under skills.
  * Assembly language is basic. Mitigation: Focus on high-level languages (C/C++, Python, JS/TS) which are more commonly used for modern IoT/backend, while keeping Assembly under programming skills.
* **Irrelevant Experience (hide/minimize):**
  * Purely theoretical deep learning research or community organizer tasks that don't involve hardware engineering/IoT backend are minimized to make space for core IoT/embedded engineering metrics.
* **Match Estimation:** Excellent (candidate satisfies the core requirements for programming, hardware integration, protocols, backend/Node.js, and databases).

---

## 4. CV EDIT PLAN (main_cv.tex)
* **Professional Summary (1-2 sentences):**
  > A Computer Engineering graduate specializing in the Internet of Things (IoT) with professional experience in designing electronic hardware prototypes, engineering high-performance firmware, and integrating backend Node.js APIs and databases to establish secure and efficient device communication.
* **Experiences & XYZ Metrics:**
  1. **IoT Engineer (Banwibu)**:
     - Reduced actuator reading failure rate by 20% through precise PCB circuit design, by prototyping and developing smart hardware circuits for ESP32-based electronic smart locks using EasyEDA.
     - Decreased user interaction error rates by 30% as measured by usability testing, by engineering custom ESP32 firmware and a resistive touchscreen HMI.
     - Delivered a web-integrated card dispenser project on schedule within 3 months, by configuring Node.js backend APIs and database schemas to manage real-time RFID data acquisition.
  2. **Research Assistant (Online)**:
     - Achieved 40% power efficiency on NVIDIA Jetson Xavier NX for deep learning inference without performance loss, by optimizing hardware resource allocation using the CORAL framework.
     - Published collaborative research on Edge AI in IEEE ICFEC 2026 proceedings, by compiling comprehensive system architecture documentation and facilitating weekly progress reviews with international research groups.
  3. **Research Assistant (Onsite)**:
     - Increased YOLOv4 model inference speed by 3x on resource-constrained edge devices (Jetson Nano, Raspberry Pi 3B), by applying post-training quantization techniques for real-time face mask detection.
     - Reduced data pre-processing latency by 20% as measured by image load times, by curating and processing a dataset of over 4,000 high-quality images for neural network training.
  4. **Exchange Student (ITB)**:
     - Improved industrial poultry environment monitoring accuracy by 15% as measured by sensor data consistency, by engineering an ESP32-based automated climate control system during the ITB exchange program.
* **Sections Trimmed/Optimized:** Trimmed the declaration section and streamlined organizational/project descriptions.
* **Target Word Count:** ~550 words (excluding bibtex metadata/preamble).

---

## 5. EXECUTION CHECKLIST (according to AGENTS.md)
- [x] Contact information: Email, Phone, LinkedIn included.
- [x] >= 5 bullet points with measurable XYZ metrics.
- [x] Hard/soft skills from JD naturally integrated into experience.
- [x] Free of first-person pronouns, clichés, or buzzwords (anti-fluff).
- [x] Word count fits target (475 - 600 words for industry).
- [x] CV language matches target (English).
- [x] Git branch name: `cv/mitech-ioteng-2026`.
- [ ] Compilation: Managed via GitHub Actions.
- [ ] Commit/push: Only if requested.


