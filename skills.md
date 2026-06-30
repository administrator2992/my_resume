# Agent Skills & Operational Procedures (skills.md)

Dokumen ini mendefinisikan daftar keahlian (skills) teknis dan prosedur operasional yang harus dijalankan oleh Agen AI Pembuat CV.

---

## 1. Skill: ATS Metrics & XYZ Formatter
**Deskripsi:** Mengubah pengalaman kerja menjadi *impact statement* yang terukur menggunakan standar XYZ.
**Prosedur Pelaksanaan:**
* Selalu format kalimat menggunakan: `Mencapai [X] yang diukur dengan [Y], dengan melakukan [Z]`.
* Pastikan agen mendistribusikan setidaknya lima metrik yang jelas di seluruh dokumen.
* *Contoh EN:* "Accomplished a 50ms reduction in hardware response latency as measured by system stability tests, by engineering an IoT actuator controller using ESP32."

## 2. Skill: Keyword & Soft-Skill Balancer
**Deskripsi:** Memastikan *hard skills* (teknis) dan *soft skills* dari *Job Description* terpenuhi secara seimbang tanpa *keyword stuffing*.
**Prosedur Pelaksanaan:**
* Ekstrak kedua tipe keahlian dari teks target.
* Masukkan minimal satu *hard skill* atau *soft skill* ke dalam setiap *bullet point* pengalaman. 
* Hapus jargon berlebihan (*fluff*).

## 3. Skill: Word Count Validator
**Deskripsi:** Menjaga agar panjang dokumen berada di rentang optimal yang disukai rekruter.
**Prosedur Pelaksanaan:**
* Setelah *drafting* pada `main_cv.tex`, hitung estimasi kata keluaran.
* Jika target adalah industri, pangkas teks jika melebihi **600 kata** dan kembangkan metrik jika di bawah **475 kata**.
* Jika target adalah akademik (Master's/PhD), abaikan batas maksimal ini.

## 4. Skill: Bilingual Context & Language Manager
**Deskripsi:** Mengatur terjemahan CV (ID/EN) secara dinamis.
**Prosedur Pelaksanaan:**
* Deteksi target (Internasional = EN, Domestik = ID).
* Sesuaikan *Section Headers*, *Action Verbs*, dan makro bahasa LaTeX (`babel`).

## 5. Skill: Git Controller & LaTeX Builder
**Deskripsi:** Otomatisasi versi dan kompilasi PDF.
**Prosedur Pelaksanaan:**
* Branch default repo ini adalah `main` (bukan `master`).
* Eksekusi urutan: `git status` -> `git checkout main` -> `git checkout -b cv/<target>-<tahun>` -> edit -> `git add .` -> `git commit`.
* **Commit/push hanya jika diminta user.** Jangan bekerja langsung di `main` tanpa membuat branch.
* File LaTeX utama adalah `main_cv.tex` (bukan `resume.tex`).
* Dokumen memakai **biblatex + biber** (`\addbibresource{biblio.bib}`), jadi kompilasi butuh pass biber, bukan `pdflatex` saja:
  ```bash
  pdflatex main_cv.tex
  biber main_cv
  pdflatex main_cv.tex
  pdflatex main_cv.tex
  ```
* Ganti nama output sesuai target: `CV_Nabhaan_<Target>.pdf`.
