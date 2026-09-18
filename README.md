# 📱 Grid Generator - Bukti Pengerjaan Misi (PWA Studio Grid)

Aplikasi web modern berbasis **PWA (Progressive Web App)** yang dirancang khusus untuk memudahkan penggabungan banyak foto bukti pengerjaan misi ke dalam satu bingkai foto (grid 2 kolom) secara instan, rapi, dan profesional langsung dari perangkat seluler (HP).

---

## ✨ Fitur Utama

- **📱 Tampilan Khusus Mobile (High-Density UI):** Desain antarmuka modern dengan warna netral *slate-gray*, font *Inter* & *Space Grotesk*, serta navigasi yang responsif dan sangat mudah digunakan di layar HP.
- **🖼️ Ukuran Foto Asli (No Cropping):** Rasio dan proporsi asli foto tetap dipertahankan secara utuh tanpa terpotong (*no object-fit cover*).
- **📝 Sistem Preset Judul Cepat (Quick Title Manager):** 
  - Kelola daftar judul sekaligus (dipisahkan baris baru/enter).
  - Judul tersimpan otomatis di *LocalStorage* browser HP.
  - Pengisian judul pada foto cukup memilih dari *dropdown list* tanpa perlu mengetik ulang manual.
- **📐 Grid 2 Kolom Sejajar:** Foto dan judul otomatis tersusun 2 kolom secara padat, hemat tempat, dan terstruktur.
- **🏷️ Judul di Atas Foto & Header Otomatis:** Setiap foto menampilkan judul di bagian atas gambar, dilengkapi header utama bertuliskan **"BUKTI PENGERJAAN MISI"**.
- **⚡ Urutan Konsisten (Async Order Fix):** Menggunakan `Promise` pembacaan file untuk menjamin urutan foto dan judul 100% tepat dan tidak pernah tertukar.
- **🗑️ Manajemen Foto Fleksibel:** Dilengkapi tombol **Hapus Per Foto** dan **Hapus Semua (Reset)**.
- **📲 PWA Standalone Murni (Installable APK-like):** 
  - Dapat diinstal langsung ke layar utama HP sebagai aplikasi mandiri (*Standalone App*).
  - Ikon aplikasi bersih tanpa badge/logo browser Chrome (menggunakan *maskable vector icon*).
- **📥 Unduh Gambar Kualitas Tinggi:** Mengunduh hasil bingkai kolase dalam format `.png` tajam menggunakan library `html2canvas`.

---

## 📂 Struktur File Proyek

```text
grid-generator/
├── index.html        # File utama (UI, Animasi CSS Smooth, & Logic JS)
├── manifest.json     # Konfigurasi PWA (Icon, Standalone Mode, Theme Color)
├── sw.js             # Service Worker (Fitur Offline & Cache PWA)
└── README.md         # Dokumentasi proyek
```

---

## 🚀 Cara Penggunaan & Instalasi

### 1. Menjalankan Aplikasi Web
1. Unduh atau *clone* seluruh file dalam repositori ini.
2. Unggah file `index.html`, `manifest.json`, dan `sw.js` ke hosting berprotokol **HTTPS** (seperti [Vercel](https://vercel.com/), [Netlify](https://www.netlify.com/), atau [GitHub Pages](https://pages.github.com/)).
3. Buka URL web menggunakan browser HP (Google Chrome / Microsoft Edge).

### 2. Menginstal sebagai Aplikasi PWA di HP
1. Buka web di browser HP.
2. Klik banner **"Instal Aplikasi PWA"** yang muncul di bagian atas aplikasi, atau tekan tombol **Menu (titik tiga)** di browser lalu pilih **"Instal Aplikasi"** / **"Tambahkan ke Layar Utama"**.
3. Aplikasi akan terinstal di daftar *App Drawer* HP kamu sebagai aplikasi murni tanpa logo Chrome.

---

## 🛠️ Teknologi yang Digunakan

- **HTML5 & CSS3** (Custom Properties, CSS Grid, Flexbox, Keyframe Animations)
- **JavaScript (ES6+)** (Service Worker API, Web Storage API, Promises)
- **[html2canvas](https://html2canvas.hertzen.com/)** (Render DOM Element ke Gambar PNG)
- **Google Fonts** (Inter & Space Grotesk)

---

## 📄 Lisensi

Proyek ini dibuat untuk penggunaan pribadi maupun tim operasional. Bebas dikembangkan dan disesuaikan kembali sesuai kebutuhan.
