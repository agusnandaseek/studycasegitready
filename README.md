# 👥 Profile Card Interactive — Study Case Git & GitHub

Proyek web interaktif **Profile Card** yang dikembangkan secara kolaboratif sebagai studi kasus simulasi alur kerja tim profesional menggunakan Git & GitHub (Branching, Pull Request, dan Code Review).

---

## 📌 Daftar Isi
1. [Tentang Proyek](#-tentang-proyek)
2. [Fitur Utama](#-fitur-utama)
3. [Susunan Anggota & Pembagian Tugas](#-susunan-anggota--pembagian-tugas)
4. [Tech Stack](#-tech-stack)
5. [Alur Kolaborasi Git (Workflow)](#-alur-kolaborasi-git-workflow)
6. [Cara Menjalankan Secara Lokal](#-cara-menjalankan-secara-lokal)

---

## 📖 Tentang Proyek

Website ini menampilkan kartu profil interaktif dari setiap anggota kelompok. Setiap pengunjung dapat melihat profil spesifik, ringkasan keahlian, memberikan tombol *Like*, dan berganti antara mode gelap (*Dark Mode*) dan mode terang (*Light Mode*).

Proyek ini dibuat untuk mempraktikkan kolaborasi multiorang tanpa konflik merge, di mana masing-masing anggota mengerjakan branch fitur terpisah:
- **Struktur Halaman (HTML)**
- **Desain & Responsivitas (CSS)**
- **Interaktivitas & Logika Dinamis (JavaScript)**

---

## ✨ Fitur Utama

- 🔄 **Dynamic Profile Switching**: Menampilkan informasi dan skill anggota secara bergantian dengan navigasi tab tanpa me-reload halaman.
- 🌙 **Dark / Light Mode**: Pengalihan tema gelap dan terang secara fleksibel menggunakan CSS variables dan DOM event listener.
- 👍 **Interactive Like Counter**: Penghitung jumlah apresiasi (like) independen untuk masing-masing profil anggota.
- 📱 **Responsive Design**: Tampilan yang menyesuaikan dengan baik di perangkat desktop, tablet, maupun layar smartphone.

---

## 👥 Susunan Anggota & Pembagian Tugas

| No | Nama Anggota | GitHub Profile | Peran / Kontribusi | Branch Terkait |
|:---:|:---|:---|:---|:---|
| **1** | **Putu Agus Nanda Pratama** *(Lead)* | [@agusnandaseek](https://github.com/agusnandaseek) | Setup repository, pembuatan kerangka dasar HTML (`index.html`), integrasi navbar, dan me-review/merge Pull Request. | `master` |
| **2** | **Celvin Aprilian** | [@CelvinAprilian-cloud](https://github.com/CelvinAprilian-cloud) | Perancangan UI/UX, styling CSS (`style.css`), efek visual card/avatar, tema dark mode, dan responsivitas mobile. | `add/style.css` (PR #1) |
| **3** | **Marwento** | [@marwento07](https://github.com/marwento07) | Pengembangan logika JavaScript (`script.js`), manipulasi DOM untuk rendering data anggota, event switcher tab, like counter, dan tema. | `add/script.js` (PR #2) |

---

## 🛠️ Tech Stack

- **HTML5**: Kerangka semantik web.
- **CSS3**: Layouting fleksibel (Flexbox & Grid), Glassmorphism, CSS Variables, dan animasi transisi.
- **JavaScript (Vanilla ES6+)**: Logika interaktif DOM manipulation & event handlers.
- **Git & GitHub**: Version Control System, Feature Branching, dan Pull Request collaboration.

---

## 🌿 Alur Kolaborasi Git (Workflow)

Proyek ini menerapkan kaidah *Feature-Branch Workflow*:

```mermaid
gitGraph
   commit id: "Setup index.html"
   branch add/style.css
   checkout add/style.css
   commit id: "feat: add style.css"
   checkout master
   branch add/script.js
   checkout add/script.js
   commit id: "feat: add script.js"
   checkout master
   merge add/style.css id: "PR #1 Merged (Styling)"
   merge add/script.js id: "PR #2 Merged (Scripting)"
   commit id: "Docs: README Kelompok"
```

1. **Inisiasi (`master`)**: Membuat kerangka `index.html`.
2. **Branch `add/style.css`**: Dikerjakan oleh Anggota 2 untuk styling visual, lalu diajukan melalui Pull Request #1 dan di-merge.
3. **Branch `add/script.js`**: Dikerjakan oleh Anggota 3 untuk fungsionalitas logika, diajukan melalui Pull Request #2 dan di-merge.
4. **Finalisasi**: Dokumentasi dan integrasi akhir pada branch utama.

---

## 🚀 Cara Menjalankan Secara Lokal

1. **Clone repository ini ke komputer lokal:**
   ```bash
   git clone https://github.com/agusnandaseek/studycasegitready.git
   ```

2. **Masuk ke direktori proyek:**
   ```bash
   cd studycasegitready
   ```

3. **Jalankan aplikasi:**
   - Cukup klik ganda (double-click) file `index.html` untuk membukanya di browser favorit kamu (Chrome, Edge, Firefox, dll), **atau**
   - Gunakan ekstensi **Live Server** di VS Code (`Right Click -> Open with Live Server`).

---

<p align="center">
  Dibuat dengan dedikasi untuk <b>Workshop Git & GitHub Collaboration</b> 🚀<br>
  © 2026 Tim Profile Card
</p>
