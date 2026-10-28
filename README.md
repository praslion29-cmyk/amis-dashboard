<div align="center">

# ✈️ AMIS — Aircraft Maintenance Intelligence System

**Smarter Maintenance. Better Decisions.**

Prototipe akademik untuk memantau pekerjaan maintenance pesawat dan melatih alur berpikir troubleshooting.

![HTML5](https://img.shields.io/badge/HTML5-single%20file-8b2338)
![JavaScript](https://img.shields.io/badge/JavaScript-vanilla-b88a45)
![Status](https://img.shields.io/badge/status-training%20prototype-35101d)
![Data](https://img.shields.io/badge/data-demo%20only-188568)

</div>

---

## 📌 Tentang AMIS

**AMIS (Aircraft Maintenance Intelligence System)** adalah dashboard berbasis web untuk mendukung proses belajar dan visualisasi pekerjaan maintenance pesawat, dengan fokus awal **Boeing 737NG** dan **ATA Chapter 24 (Electrical Power)**.

Seluruh aplikasi berjalan di satu file HTML, tanpa server dan tanpa instalasi. Data disimpan di `localStorage` browser.

> ⚠️ **Disclaimer:** AMIS adalah prototipe akademik dengan data simulasi. Bukan sistem maintenance operasional dan bukan pengganti manual resmi (AMM, FIM, dan dokumen approved lainnya). Semua isi troubleshooting bersifat pembelajaran dan harus diverifikasi pada dokumen yang berlaku.

## ✨ Fitur Utama

| Modul | Fungsi |
|---|---|
| 🏠 **Overview** | Ringkasan work order, peta sistem pesawat interaktif (hotspot ATA), kartu navigasi modul, dan log aktivitas |
| 🔧 **Maintenance Tracking** | Catat, cari, filter, dan perbarui work order beserta ATA Chapter dan progres |
| ➕ **Defect Intake** | Form laporan defect (aircraft type, registrasi, ATA, rute, uraian) yang menjadi dasar kasus simulasi |
| 🧪 **Troubleshooting Lab** | Simulasi investigasi bertahap: *Observe → Assess → Decide → Review*, lengkap dengan diagram interaktif ATA 24 |
| 🤖 **FIM AI Assistant** | Menyusun pertanyaan terstruktur dari defect, membukanya di NotebookLM, dan mencatat temuan yang sudah diverifikasi |
| 📊 **Reports & Data** | Statistik ringkas, ekspor CSV, dan health check prototipe |
| 📖 **Panduan AMIS** | Alur penggunaan dan penjelasan setiap tab |

## 🖼️ Tampilan

Letakkan screenshot pada folder `docs/` lalu ganti tautan di bawah.

| Cover | Overview |
|---|---|
| ![Cover](docs/cover.png) | ![Overview](docs/overview.png) |

## 🚀 Cara Menjalankan

**Opsi 1 — Langsung dibuka**
1. Unduh atau clone repository ini.
2. Buka file `AMIS_dashboard_v21_Final.html` di browser modern (Chrome, Edge, Firefox).
3. Klik **ENTER DASHBOARD** pada halaman cover.

```bash
git clone https://github.com/<username>/<nama-repo>.git
cd <nama-repo>
# buka file HTML dengan browser
```

**Opsi 2 — GitHub Pages**
1. Ubah nama file HTML menjadi `index.html`.
2. Buka **Settings → Pages**, pilih branch `main` dan folder `/ (root)`.
3. Dashboard akan tersedia di `https://<username>.github.io/<nama-repo>/`.

## 🗂️ Struktur Repository

```
.
├── AMIS_dashboard_v21_Final.html   # Aplikasi (single file)
├── README.md
└── docs/                                     # Screenshot untuk README
```

## 🔄 Alur Penggunaan

1. Isi laporan di **Defect Intake**, lalu simpan untuk membuat *simulation case*.
2. Buka **Troubleshooting Lab** dan kerjakan kasus secara berurutan.
3. Gunakan **FIM AI Assistant** untuk menyiapkan pertanyaan ke NotebookLM, lalu verifikasi task, revisi, dan effectivity pada manual approved.
4. Tinjau hasil di **Reports & Data** dan ekspor bila perlu.

## 🧱 Teknologi

- HTML5, CSS3 (grid, flexbox, animasi CSS), dan JavaScript vanilla
- Ilustrasi inline SVG, tanpa library atau framework eksternal
- Penyimpanan lokal dengan `localStorage`
- Desain responsif untuk desktop, tablet, dan mobile

## 🛣️ Roadmap

- [ ] Integrasi Google Sheets (Apps Script endpoint) untuk data bersama
- [ ] Validasi input dan penanganan error koneksi
- [ ] Penambahan kasus training untuk ATA Chapter lain
- [ ] Autentikasi pengguna dan peran (admin, teknisi, instruktur)
- [ ] Review konten oleh personel berwenang

## ⚠️ Catatan Data dan Keamanan

- Data tersimpan **lokal di browser** dan tidak dikirim ke server mana pun.
- Jangan memasukkan data sensitif, rahasia, atau terbatas milik organisasi.
- Angka pada dashboard adalah data demo dan tidak mewakili kondisi armada nyata.

## 📄 Lisensi

Tentukan lisensi sesuai kebutuhan (misalnya MIT untuk kode) dan tambahkan file `LICENSE`. Pastikan Anda memiliki hak atas seluruh aset gambar, termasuk foto pada cover.

## 👤 Kontributor

Dikembangkan oleh **AeroTech Solutions** — AMIS Project.
