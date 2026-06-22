# 🩺 Anamnexy

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE) [![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-deploy-green.svg)](https://github.com/RanggaCX31/anamnex)

**Anamnexy** adalah aplikasi web dokumentasi klinis untuk tenaga medis — berisi generator SOAP, kalkulator dosis obat, guideline kegawatdaruratan IGD, dan ensiklopedia diagnosis/penyakit A-Z. Dibuat sebagai aplikasi statis agar mudah di-host di GitHub Pages atau dijalankan lokal.

🔗 Demo (GitHub Pages): https://RanggaCX31.github.io/anamnex/

---

## ✨ Fitur

- **🔐 Login Member & Admin** — autentikasi sederhana tersimpan di `localStorage` browser.
- **🛠️ Kelola Member (Admin)** — admin dapat menambah, melihat, dan menghapus akun member.
- **📋 SOAP Generator** — buat dokumentasi SOAP cepat per jenis pasien (dewasa, anak, kebidanan, dll) lengkap dengan template pemeriksaan fisik.
- **💊 Kalkulator Dosis Obat** — 100+ obat & merek dagang tersusun A–Z, dosis dihitung otomatis berdasarkan berat badan pasien.
- **📘 Guideline 2026** — ringkasan pendekatan kegawatdaruratan IGD (ABCDE, triase, RJP/ACLS, syok, SKA, stroke, sepsis, dll) dengan ilustrasi SVG, plus daftar sumber rujukan resmi.
- **📖 Ensiklopedia Diagnosis A–Z** — ringkasan penyakit per kategori: definisi, gejala, pendekatan diagnosis, tata laksana, dan sumber referensi tiap entri.

---

## ⚠️ Disclaimer

Aplikasi ini adalah **alat bantu dokumentasi & edukasi klinis**, bukan pengganti penilaian klinis langsung, pedoman resmi terbaru, atau konsultasi dengan sejawat/spesialis. Selalu verifikasi dosis, pedoman, dan keputusan klinis dengan referensi resmi dan sumber terpercaya.

Data login & member disimpan secara **lokal di browser** (`localStorage`) — tidak ada server/database. Jika cache browser dihapus atau aplikasi dibuka di device/browser lain, data tersebut tidak akan tersinkron; export/import data disarankan untuk backup.

---

## 🚀 Cara Menjalankan

Karena ini murni file statis (HTML/CSS/JS dalam satu file `index.html`), tidak perlu instalasi atau server khusus.

### Opsi 1 — Buka langsung
Cukup buka file `index.html` di browser (Chrome/Edge/Firefox).

### Opsi 2 — Local server (disarankan agar semua fitur browser berjalan normal)
```bash
# Python
python3 -m http.server 8000
# lalu buka http://localhost:8000

# atau Node.js
npx serve .
```

### Akun default
- **Admin:** `admin` / `admin123` (disarankan segera diganti lewat menu *Kelola Member* setelah login)
- **Member:** belum ada — tambahkan melalui akun admin

---

## 🌐 Deploy ke GitHub Pages

1. Push repo ini ke GitHub.
2. Buka **Settings → Pages**.
3. Pilih **Branch: main**, folder **/ (root)**.
4. Simpan — situs akan tersedia di `https://<username>.github.io/<nama-repo>/` dalam beberapa menit.

Contoh: https://RanggaCX31.github.io/anamnex/

---

## 📁 Struktur Project

```
anamnexy/
├── index.html      # Seluruh aplikasi (HTML + CSS + JS dalam satu file)
├── README.md
├── LICENSE
└── .gitignore
```

> Catatan: project ini sengaja dibuat sebagai single-file app agar mudah di-host di mana saja (GitHub Pages, Netlify, atau dibuka langsung secara offline) tanpa proses build.

---

## 🤝 Kontribusi

Pull request untuk menambah/memperbarui materi medis, dosis obat, atau perbaikan UI sangat diterima. Pastikan setiap entri medis baru menyertakan sumber rujukan yang jelas (tautan ke pedoman resmi, jurnal, atau sumber otoritatif).

Lihat `CONTRIBUTING.md` untuk panduan kontribusi dan checklist review.

## 📄 Lisensi

MIT License — lihat file [LICENSE](LICENSE).
