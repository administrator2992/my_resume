# Target Pekerjaan & Pemetaan CV (JOB_PROFILE.md)

> **Tujuan:** Tempat menempelkan Job Description (JD) target dan memetakannya ke
> `PROFILE.md` agar `main_cv.tex` bisa dioptimalkan (ATS + XYZ) untuk lowongan itu.
> **Cara pakai:** Isi Bagian 1 (paste JD apa adanya). Agen mengisi Bagian 2–5.
> Aturan optimasi mengikuti `AGENTS.md` & `skills.md`. Satu file = satu target;
> arsipkan target lama ke Bagian 6 sebelum mengganti.

---

## 1. INPUT — Detail Lowongan (diisi USER)
* **Nama Perusahaan/Institusi:** Multinational IoT & Digital Manufacturing Solution, Recruited through PT Trust Recruit Indonesia
* **Posisi yang Dilamar:** Site Engineer IoT
* **Lokasi / Remote:** Riau
* **Bahasa CV target:** EN
* **Jenis target:** Industri
* **Link lowongan (opsional):** [Jobstreet](https://id.jobstreet.com/job/92926004?ref=search-standalone&type=standard&origin=showNewTab#sol=90b8c17bb624348ef8a9fa6a8ebc684e61309d32)

### Job Description (paste mentah di sini)
```text
Client Details: Multinational IoT & Digital Manufacturing Solution

Main Responsibilities:

Work closely with Business Analysts (BA) to ensure timely execution and on-schedule delivery of Nursery projects.

Handle daily communication and routine reporting with on-site nursery staff in Bahasa Indonesia, based on guidelines and briefings provided by the BA team.

Coordinate on-site logistics during project implementation, including transportation, accommodation, and catering arrangements.

Maintain strong and stable working relationships with key project stakeholders, including internal nursery teams, NAT teams, and R&D teams.

Requirements:

Strong academic background with basic understanding of agricultural mechanization, IT systems, and algorithms

Strong interpersonal and communication skills; prior exposure or hands-on experience in Agriculture, Nursery, IoT projects is an advantage.

Willingness to travel extensively across rural and remote areas in Indonesia, with up to 8 months of business travel per year during the project execution phase.

Work experience in consulting firms, third-party service providers, or startup environments is mandatory.

Fluent in Bahasa Indonesia and English; Mandarin proficiency is a plus.

Willing to travel and stay frequently across Sumatera and Kalimantan

```

## 2. EKSTRAKSI KATA KUNCI (diisi AGEN dari JD)
> Pindai JD, pisahkan menjadi dua kelompok. Dipakai untuk menyisipkan keyword
> secara natural ke bullet pengalaman (tanpa keyword stuffing).

* **Hard Skills (teknis):**
  | Keyword dari JD | Ada di PROFILE.md? | Bukti / Pengalaman terkait |
  |---|---|---|
  | IoT Projects & Systems | Ya | IoT Engineer Banwibu (Smart Locker, Card Gacha), Student Exchange ITB (IIoT Coop) |
  | IT Systems & Networks | Ya | S1 Computer Engineering coursework (Operating Systems, Cloud Computing, Computer Network), Teaching Assistant |
  | Algorithms | Ya | Coursework, YOLO model optimization research assistant |
  | Agricultural Mechanization | Ya | Student Exchange at ITB studying IIoT chicken coop automation & fruit sorting |

* **Soft Skills:**
  | Keyword dari JD | Ada di PROFILE.md? | Bukti / Pengalaman terkait |
  |---|---|---|
  | Communication & Reporting | Ya | Daily reporting with local on-site nursery staff; research assistant weekly reporting with Prof. In Kee Kim, Prof. Muhammad Santriaji, and Dr. Arief Setyanto |
  | Project Delivery/Execution | Ya | Delivering Banwibu card gacha project on schedule; research projects milestones tracking |
  | Logistics Coordination | Ya | Community Secretary organizing events (handling transportation, accommodation, scheduling) |
  | Working Relationships | Ya | Multi-institutional collaborative research (AMIKOM, UGA, UGM) and client maintenance at Banwibu |

* **Requirement wajib (must-have) vs nilai plus (nice-to-have):**
  * Must-have: Willingness to travel extensively (up to 8 months/year in rural Sumatera/Kalimantan), startup/third-party work experience (Banwibu), fluent in Indonesian & English, basic IT/IoT/Algorithms understanding.
  * Nice-to-have: Agricultural/Nursery/IoT project exposure, Mandarin proficiency.

---

## 3. ANALISIS KECOCOKAN (Gap Analysis)
* **Sudah cocok (highlight di CV):** S1 Computer Engineering (IoT spec), Startup environment experience at Banwibu, Agricultural/Automation projects (ITB chicken coop, Fruit sorting tool), leadership/admin role (Community Secretary).
* **Gap / lemah (yang perlu disiasati atau dijujurkan):** No direct "nursery" work experience (siasati by highlighting industrial chicken coop automation and fruit sorting IoT), no Mandarin (rely on native Indonesian and professional English).
* **Pengalaman dari PROFILE.md yang TIDAK relevan (sembunyikan dari CV ini):** Heavy academic machine learning publications and conference presentations (minimalkan, focus on the engineering, hardware, and implementation aspects rather than pure AI theory).
* **Estimasi kecocokan:** Tinggi-Sedang (Sangat kuat di technical IoT dan startup experience, and has key agricultural/logistics analogs).

---

## 4. RENCANA PENYUNTINGAN `main_cv.tex`
> Setiap bullet pengalaman terpilih ditulis ulang dengan rumus XYZ:
> `Mencapai [X] diukur dengan [Y], dengan melakukan [Z]`. Minimal 5 metrik.

* **Personal Summary (1–2 kalimat, fokus nilai jual untuk posisi ini):**
  > Detail-oriented IoT Engineer and Computer Engineering graduate with a strong background in IT systems, algorithms, and startup project environments. Experienced in deploying embedded automation systems and agricultural IoT solutions, with proven communication and coordination skills to collaborate with cross-functional stakeholders and deliver projects on schedule.
* **Pengalaman yang ditarik + draf bullet XYZ:**
  1. **IoT Engineer (Banwibu)**:
     - Achieved a 99.8% uptime rate for industrial automation machinery at Unitama Sari Mas by implementing a routine preventative maintenance schedule and system diagnostics.
     - Reduced user interaction errors by 30% by developing a custom resistive touchscreen HMI for ESP32-based Smart Lockers, enhancing operational efficiency.
     - Delivered a Card Gacha Machine integrating RFID systems and an Angular web app on schedule within a 3-month timeline, collaborating with business developers to ensure alignment with client specifications.
  2. **Research Assistant (Online)**:
     - Coordinated hardware resource optimization on NVIDIA Jetson Xavier NX for deep learning inference, resulting in a 40% reduction in power usage while maintaining stable model execution.
     - Facilitated weekly reporting and technical documentation updates across three collaborating university research groups (UGA, UGM, AMIKOM) to ensure on-schedule milestone delivery.
  3. **Research Assistant (Onsite)**:
     - Boosted face-mask detection application inference speeds by 3x on NVIDIA Jetson Nano and Raspberry Pi 3B by applying model optimization techniques.
     - Streamlined dataset preparation by collecting and curating over 4,000 high-quality images of faces, improving training accuracy.
  4. **Secretary (Community)**:
     - Coordinated event logistics (transportation, accommodation, and venue arrangements) for over 150 participants across 5 community workshops, ensuring smooth event execution.
  5. **Domestic Student Exchange (ITB)**:
     - Engineered an automated environmental control system for an industrial chicken coop during the exchange program at Bandung Institute of Technology, improving agricultural monitoring precision.
* **Section yang dipangkas / disembunyikan agar fokus & sesuai word count:** Minimalkan details of academic publications (keep the section but keep it short), hide TA positions of OS/AI/Python if they exceed word count or do not match the main path.
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

