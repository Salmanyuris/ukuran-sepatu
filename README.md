# 👟 ShoeFit — Kalkulator Ukuran Sepatu

> Aplikasi web modern untuk memperkirakan ukuran sepatu berdasarkan tinggi badan. Dibangun dengan HTML, CSS, dan JavaScript murni — tanpa framework tambahan.

![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=flat-square)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![License](https://img.shields.io/badge/License-MIT-purple?style=flat-square)

---

## 📌 Tentang Project

**ShoeFit** adalah aplikasi web kalkulator ukuran sepatu yang didesain dengan tampilan modern dan premium. Pengguna cukup memasukkan tinggi badan, tekan tombol, dan langsung mendapatkan perkiraan ukuran sepatu EU mereka.

Project ini menggabungkan estetika **dark glassmorphism**, **animasi sepatu SVG inline**, dan **micro-interactions** untuk pengalaman pengguna yang menarik — sekaligus menjadi latihan fundamental web development.

---

## ✨ Fitur Unggulan

| Fitur | Keterangan |
|---|---|
| 📏 Input Tinggi Badan | Input angka dengan validasi real-time |
| 🧮 Kalkulasi Instan | Rumus proporsional tubuh, hasil langsung tampil |
| 👟 Animasi Sepatu SVG | Sepatu melayang dengan animasi float & gradient |
| 🌌 Dark Glassmorphism | Tema gelap modern dengan `backdrop-filter: blur()` |
| ✨ Floating Particles | Emoji sepatu melayang animatif di background |
| 📊 Progress Bar Dinamis | Visualisasi ukuran dengan bar animasi |
| 💫 Micro-Animations | Pop animation pada angka hasil kalkulasi |
| ⌨️ Keyboard Support | Tekan `Enter` untuk langsung menghitung |
| 📱 Responsive Design | Tampilan optimal di semua ukuran layar |
| ⚡ Zero Dependencies | Tidak butuh library atau framework apapun |

---

## 🛠️ Teknologi yang Digunakan

| Teknologi | Versi / Detail | Kegunaan |
|---|---|---|
| HTML5 Semantic | Latest | Struktur & markup halaman |
| CSS3 Custom Properties | Latest | Design tokens & sistem tema |
| CSS Animations & Keyframes | Latest | Animasi sepatu, particles, transisi UI |
| CSS Glassmorphism | `backdrop-filter: blur()` | Efek kaca transparan modern |
| SVG Inline | Handcrafted | Ilustrasi sepatu animatif |
| Vanilla JavaScript | ES6+ | Logika kalkulasi & manipulasi DOM |
| Google Fonts — Outfit | wght 300–900 | Tipografi modern & bersih |

---

## 📁 Struktur Project

```text
ukuran-sepatu/
├── index.html    ← Struktur halaman, SVG sepatu & script validasi
├── style.css     ← Dark glassmorphism theme, animasi & responsive
├── script.js     ← Fungsi kalkulasi ukuran sepatu (core logic)
└── README.md     ← Dokumentasi project
```

---

## 🧮 Rumus Perhitungan

```
Ukuran Sepatu (EU) = (Tinggi Badan × 0.24) + 0.42
```

Hasil dibulatkan menggunakan `Math.round()`.

> **⚠️ Catatan:** Hasil merupakan **perkiraan** berdasarkan proporsi tubuh rata-rata manusia, bukan standar resmi dari produsen sepatu.

---

## 🚀 Cara Menjalankan

### Cara Cepat (tanpa instalasi)
1. **Clone** repository ini:
   ```bash
   git clone https://github.com/Salmanyuris/ukuran-sepatu.git
   ```
2. **Masuk** ke folder project:
   ```bash
   cd ukuran-sepatu
   ```
3. **Buka** `index.html` langsung di browser *(double-click)*, atau gunakan **Live Server** di VS Code untuk pengalaman terbaik.

### Menggunakan Live Server (VS Code)
1. Install ekstensi **Live Server** di VS Code
2. Klik kanan `index.html` → **"Open with Live Server"**
3. Browser akan otomatis terbuka di `http://127.0.0.1:5500`

---

## 📖 Contoh Hasil Perhitungan

| Tinggi Badan | Ukuran Sepatu (EU) | Keterangan |
|:---:|:---:|:---|
| 150 cm | 36 | Ukuran kecil |
| 155 cm | 38 | Rata-rata perempuan |
| 165 cm | 40 | Transisi perempuan/laki-laki |
| 170 cm | 41 | Rata-rata laki-laki Indonesia |
| 175 cm | 42 | Di atas rata-rata |
| 180 cm | 43 | Laki-laki tinggi |
| 190 cm | 46 | Ukuran besar |

---

## 🎯 Tujuan Pembelajaran

Project ini dibuat sebagai latihan untuk memahami:

- ✅ **Manipulasi DOM** dengan JavaScript murni
- ✅ **CSS Modern** — Custom Properties, Glassmorphism, Keyframe Animations
- ✅ **Validasi Input** — pengecekan nilai sebelum kalkulasi
- ✅ **SVG Inline** — membuat ilustrasi vektor langsung di HTML
- ✅ **Micro-interactions** — UX yang hidup & responsif
- ✅ **Responsive Design** — tampilan lintas perangkat
- ✅ **Git Workflow** — version control & push ke GitHub

---

## 🤝 Kontribusi

Kontribusi sangat terbuka! Jika ingin berkontribusi:

1. **Fork** repository ini
2. Buat **branch** baru: `git checkout -b fitur/nama-fitur`
3. **Commit** perubahan: `git commit -m "feat: tambah fitur X"`
4. **Push** ke branch: `git push origin fitur/nama-fitur`
5. Buat **Pull Request**

---

## 📄 Lisensi

Project ini dilisensikan di bawah **MIT License** — bebas digunakan, dimodifikasi, dan didistribusikan.

---

## 👤 Author

**Salman Yuris**
- GitHub: [@Salmanyuris](https://github.com/Salmanyuris)

---

<div align="center">

⭐ **Jika project ini bermanfaat, berikan Star pada repository ini!** ⭐

*Dibuat dengan ❤️ menggunakan HTML, CSS & JavaScript murni*

</div>
