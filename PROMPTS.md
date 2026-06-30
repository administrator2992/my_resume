# Kumpulan Instruksi Templat (PROMPTS.md)

Dokumen ini berisi *template prompt* baku yang akan digunakan oleh pengguna untuk memerintah Agen AI. Dengan menggunakan *template* ini, Agen akan otomatis menerapkan seluruh aturan dari `AGENTS.md` dan `skills.md`.

---

## 1. Templat: Aplikasi Lowongan Industri (Corporate Job)
**Gunakan *prompt* ini ketika melamar ke perusahaan (Software Engineer, AI Engineer, IoT Developer, dll).**

```text
[Lang: ID/EN] (Pilih salah satu)
Tolong buatkan draf CV untuk lowongan berikut.

Target Perusahaan: [Nama Perusahaan]
Posisi: [Nama Posisi]
Job Description (JD):
[Paste JD di sini]

Instruksi Wajib Eksekusi untuk Agen:
1. Pindai JD di atas dan cocokkan dengan data di `PROFILE.md`. Tarik hanya pengalaman yang paling relevan.
2. Sertakan tautan ke profil LinkedIn saya di bagian kontak.
3. Setiap bullet point pengalaman kerja HARUS menggunakan format XYZ: "Mencapai [X] yang diukur dengan [Y], dengan melakukan [Z]".
4. Ekstrak Hard Skills dan Soft Skills dari JD, dan pastikan setiap bullet point pengalaman mengandung minimal satu dari kata kunci tersebut secara natural (tanpa keyword stuffing).
5. Hapus SEMUA kata ganti orang pertama (Saya/Kami), cliches, dan buzzwords.
6. Jaga total panjang dokumen di rentang 475 hingga 600 kata.
7. Eksekusi alur Git (branch baru: cv/[target]-[tahun]) dan kompilasi ke PDF menggunakan LaTeX.
```

---

## 2. Templat: Aplikasi Akademik (Master's/PhD/Research Lab)
**Gunakan *prompt* ini ketika menghubungi Profesor atau mendaftar program pascasarjana.**

```text
[Lang: EN]
Tolong buatkan draf CV Akademik untuk keperluan aplikasi riset.

Target Institusi: [Nama Universitas, misal: KAUST / NTUST]
Nama Profesor/Lab: [Nama Profesor / Lab]
Fokus Riset Lab:
[Paste deskripsi lab atau abstrak paper terbaru dari Profesor target di sini]

Instruksi Wajib Eksekusi untuk Agen:
1. Prioritaskan data dari bagian "Pengalaman Riset" dan "Pendidikan" di `PROFILE.md`.
2. Sertakan skor tes kemampuan bahasa (TOEFL) dan tautan profil publikasi/LinkedIn.
3. Gunakan metrik XYZ untuk mendeskripsikan efisiensi algoritma atau hasil eksperimen (misal: "Meningkatkan efisiensi komputasi sebesar X% yang diukur dari...").
4. Abaikan batasan maksimal 600 kata; jabarkan teknis publikasi dan proyek secara mendetail.
5. Eksekusi alur Git (branch baru: cv/academic-[target]-[tahun]) dan kompilasi ke PDF menggunakan LaTeX.
```
