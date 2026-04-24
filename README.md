# Pedef — PDF Toolkit

> Aplikasi pengolah PDF berbasis browser. Semua pemrosesan dilakukan **100% lokal** — tidak ada file yang diunggah ke server.

![Pedef](https://img.shields.io/badge/Pedef-PDF%20Toolkit-7c6aff?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)
![Made by](https://img.shields.io/badge/dibuat%20oleh-Samuel%20Lana-orange?style=flat-square)

---

## ✨ Fitur

### Mode Single
Gunakan satu tool untuk satu file PDF.

| Tool | Deskripsi |
|------|-----------|
| 🔗 **Gabung** | Gabungkan beberapa file PDF menjadi satu dokumen |
| ✂️ **Pisah** | Pisahkan PDF berdasarkan range halaman (misal: 1-3, 4-6) |
| 🗜️ **Kompres** | Kurangi ukuran file PDF dengan mengatur kualitas gambar |
| 🔄 **Putar** | Putar halaman individual atau semua halaman sekaligus |
| 🗑️ **Hapus Halaman** | Pilih dan hapus halaman tertentu dari PDF |
| ↕️ **Atur Urutan** | Seret thumbnail untuk mengubah urutan halaman |
| 💧 **Watermark** | Tambahkan teks watermark dengan pengaturan warna, opacity, dan sudut |
| ✍️ **Tanda Tangan** | Upload gambar TTD, background putih otomatis dihapus, posisikan bebas drag & drop |

### Mode Pipeline 🚀
Jalankan **beberapa tool sekaligus secara berurutan** tanpa perlu download di setiap langkah. Cukup **1x download** di akhir.

**Contoh pipeline:** Gabung → Hapus Halaman → Atur Urutan → Tanda Tangan → Download

Urutan eksekusi otomatis diatur secara logis:
1. Gabung
2. Kompres
3. Hapus Halaman
4. Atur Urutan
5. Putar
6. Pisah
7. Watermark
8. Tanda Tangan

---

## 🔒 Privasi & Keamanan

- **Tidak ada upload ke server** — file PDF hanya dibaca oleh browser kamu
- **Tidak ada database** — tidak ada data yang disimpan di server manapun
- **Bisa dipakai offline** — setelah halaman dimuat, tidak perlu koneksi internet
- Preferensi pengguna (bahasa, tema, font) disimpan di **localStorage** browser

---

## 🛠️ Teknologi

| Library | Fungsi |
|---------|--------|
| [PDF.js](https://mozilla.github.io/pdf.js/) | Render preview halaman PDF di browser |
| [pdf-lib](https://pdf-lib.js.org/) | Manipulasi PDF (gabung, pisah, watermark, dll) |
| Google Fonts | Plus Jakarta Sans, Outfit, Fraunces, DM Sans, Unbounded |

---

## 🚀 Cara Pakai

### Opsi A — File Lokal (paling simpel)
1. Download file `index.html`
2. Buka langsung di browser (double-click atau drag ke Chrome/Firefox)
3. Selesai — tidak perlu install apapun

### Opsi B — Deploy ke Vercel
1. Fork atau clone repo ini
2. Connect ke [Vercel](https://vercel.com)
3. Deploy otomatis — Vercel cukup serve file HTML-nya

> **Catatan:** Meskipun di-deploy ke Vercel, semua pemrosesan PDF tetap terjadi di browser pengguna. Vercel hanya mengirimkan file HTML ke browser, bukan memproses PDF.

### Opsi C — Self-host
Cukup taruh `index.html` di web server manapun (Apache, Nginx, GitHub Pages, Netlify, dll). Tidak perlu backend atau database.

---

## 🎨 Kustomisasi UI

Tersedia langsung dari antarmuka aplikasi:

- **5 pilihan font** — Plus Jakarta Sans, Outfit, Fraunces, DM Sans, Unbounded
- **Dark / Light mode** — toggle di header
- **Bilingual** — Bahasa Indonesia & English

---

## 📱 Mobile

Tampilan mobile-friendly dengan sidebar drawer:
- Tap ☰ untuk membuka sidebar
- Tap di luar sidebar atau ✕ untuk menutup
- Mode Pipeline: sidebar tetap terbuka saat memilih tools, menutup otomatis setelah klik "Mulai Pipeline"

---

## 📂 Struktur File

```
pedef/
└── index.html    # Seluruh aplikasi dalam satu file
```

Tidak ada dependensi tambahan, tidak ada build step, tidak ada `node_modules`.

---

## 📄 Lisensi

MIT License — bebas digunakan, dimodifikasi, dan didistribusikan.

---

© 2026 · Dibuat oleh **Samuel Lana**
