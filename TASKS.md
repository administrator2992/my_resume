# TASKS.md — Agent Memory & Recovery Notes

> **Tujuan file ini:** Catatan persisten jika konteks Agen hilang/terkompaksi.
> Baca file ini DULU saat memulai sesi, lalu baca `AGENTS.md`, `skills.md`,
> `PROMPTS.md`, dan `PROFILE.md` (single source of truth).
> Terakhir diperbarui: 2026-06-25.

---

## 0. PERAN SAYA (ringkas)
Agen AI Spesialis Optimasi CV (ATS-friendly) dengan alur kerja LaTeX + Git.
Tugas: menyesuaikan CV master (`main_cv.tex`) berdasarkan Job Description (JD)
industri ATAU profil riset Profesor (akademik). Data ditarik dari `PROFILE.md`.

## 1. ATURAN WAJIB (dari AGENTS.md & skills.md)
- **Single source of truth:** `PROFILE.md`. Jika data CV ≠ PROFILE.md, perbaiki
  PROFILE.md dulu (kecuali user minta sebaliknya).
- **Rumus XYZ:** `Mencapai [X] yang diukur dengan [Y], dengan melakukan [Z]`.
  Minimal **5 metrik terukur** tersebar di seluruh dokumen.
- **Keyword balance:** ekstrak hard + soft skill dari JD; sisipkan ≥1 per bullet
  pengalaman. JANGAN keyword stuffing.
- **Word count:** industri **475–600 kata** (pangkas jika >600, kembangkan jika
  <475). Akademik (Master/PhD, mis. KAUST/NTUST): abaikan batas maksimal.
- **Anti-fluff:** hapus kata ganti orang pertama (Saya/Kami), klise, buzzwords,
  hiperbola. Kalimat lugas.
- **Kontak wajib:** Email, Telepon, LinkedIn (+ publikasi untuk akademik).
- **Bahasa:** Internasional = EN, Domestik = ID. Sesuaikan section header &
  action verbs.

## 2. ALUR KERJA GIT + LATEX
1. Branch baru: `cv/[target]-[posisi/topik]-[tahun]`
   (akademik: `cv/academic-[target]-[tahun]`).
2. Edit konten LaTeX langsung di `main_cv.tex` (terapkan XYZ + word count).
3. Commit: `docs: optimize CV for [Target], applied XYZ metrics ...`
4. Kompilasi PDF: `pdflatex main_cv.tex` → output `CV_[Nama]_[Target].pdf`.
   (Catatan: ada bibliografi `biblio.bib` via biblatex → mungkin perlu
   `pdflatex → biber → pdflatex → pdflatex`.)
- **Penting:** commit/push HANYA jika user minta. Jangan kerja di branch `main`
  tanpa membuat branch dulu.

## 3. TEMPLATE PROMPT (dari PROMPTS.md)
- **Industri:** scan JD → tarik pengalaman relevan → XYZ tiap bullet →
  keyword balance → hapus fluff → 475–600 kata → Git + PDF.
- **Akademik:** prioritaskan "Pengalaman Riset" + "Pendidikan" → sertakan TOEFL
  & link publikasi → XYZ untuk hasil eksperimen → abaikan batas 600 kata →
  Git + PDF.

## 4. FAKTA KUNCI KANDIDAT (verifikasi dari PROFILE.md sebelum dipakai)
- Nama: Ahmad Naufal Labiib Nabhaan | Email: nabhaan.ahmad.ln@gmail.com
- Telp: +62 853-1498-8120 | GitHub: administrator2992 | LinkedIn: ahmadnabhaan
- Web: administrator2992.github.io | Lokasi: Indonesia
- S1 Teknik Komputer (IoT), AMIKOM Yogyakarta, GPA 3.88, Sep 2019–Jan 2025.
- TOEFL iBT 58, ITP 500.
- Target: beasiswa penuh Master/PhD Ilmu Komputer angkatan 2027 (KAUST, NTUST)
  + peran Fullstack/AI/IoT Engineer.
- Pembimbing/kolaborator: Prof. Arief Setyanto (AMIKOM), Prof. In Kee Kim
  (Univ. of Georgia), Prof. Muhammad Santriaji (UGM).

## 5. STATUS PEKERJAAN
- [x] Sinkronisasi `PROFILE.md` dengan `main_cv.tex` (selesai 2026-06-25).
  Keputusan user: Banwibu = "IoT Engineer, Mei 2025–Juni 2026"; entri bookstore
  (Lead Auditor) DIHAPUS; TOEFL iBT 58 & ITP 500 keduanya valid.
- [ ] CATATAN TERBUKA: CV (`main_cv.tex` baris ~368) hanya cantumkan TOEFL iBT 58.
  Tanyakan/tambahkan ITP 500 ke CV jika user mau.
- [ ] CATATAN TERBUKA: target KAUST/NTUST 2027 ada di PROFILE.md tapi tidak di CV
  (wajar — itu konteks profil, bukan isi CV).

## 6. FILE PENTING
- `main_cv.tex` — CV LaTeX utama (satu-satunya .tex).
- `biblio.bib` — referensi publikasi (keys: matrikraka, matrikahmad, edge24,
  nabhaan2026coral).
- `PROFILE.md` — master data kandidat (single source of truth).
- `AGENTS.md` / `skills.md` / `PROMPTS.md` — aturan & template operasional.
