# 🎮 Last Semester

> Kumpulan resource, script, dan aset untuk pengembangan server **FiveM** — dibuat untuk mempercepat proses development dan mempermudah kolaborasi tim.

![Status](https://img.shields.io/badge/status-active-success)
![FiveM](https://img.shields.io/badge/platform-FiveM-orange)
![License](https://img.shields.io/badge/license-MIT-blue)
![Language](https://img.shields.io/badge/lang-Lua%20%7C%20JS%20%7C%20HTML-lightgrey)

---

## 📖 Daftar Isi

- [Tentang Project](#-tentang-project)
- [Fitur](#-fitur)
- [Struktur Folder](#-struktur-folder)
- [Persyaratan](#-persyaratan)
- [Instalasi](#-instalasi)
- [Cara Penggunaan](#-cara-penggunaan)
- [Daftar Resource](#-daftar-resource)
- [Kontribusi](#-kontribusi)
- [License](#-license)
- [Credits](#-credits)
- [Penutup](#-penutup)

---

## 🧩 Tentang Project

**Last Semester** adalah repository yang berisi kumpulan resource untuk server **FiveM**, mencakup script gameplay, antarmuka pengguna (NUI/UI panel), sistem manajemen server, dan berbagai aset pendukung lainnya. Project ini dibuat untuk mempermudah proses pengembangan server roleplay, baik untuk kebutuhan pribadi maupun kolaborasi tim.

Repository ini dirancang agar mudah dipahami, dikembangkan, dan disesuaikan sesuai kebutuhan server masing-masing.

---

## ✨ Fitur

- 🗂️ Kumpulan resource FiveM yang terorganisir dengan rapi
- 🎨 Antarmuka (UI/NUI) modern dengan desain dark theme
- ⚙️ Struktur kode yang mudah dibaca dan dikembangkan
- 🌐 Mendukung konten berbahasa Indonesia
- 🔧 Mudah dikonfigurasi dan diintegrasikan ke server FiveM
- 📦 Update dan penambahan resource secara berkala

---

## 📁 Struktur Folder

Berikut contoh struktur folder pada repository ini:

```
last-semester/
├── resources/
│   ├── ls-ui/              # Resource antarmuka (NUI)
│   ├── ls-core/             # Script inti server
│   └── ls-jobs/             # Sistem pekerjaan/job
├── docs/
│   └── DESIGN.md            # Dokumentasi sistem desain
├── config/
│   └── config.lua           # File konfigurasi utama
├── README.md
└── LICENSE
```

> 💡 Struktur di atas bersifat contoh dan dapat berbeda tergantung resource yang tersedia di dalam repository.

---

## 📋 Persyaratan

Sebelum menggunakan resource pada repository ini, pastikan sudah menyiapkan:

| Kebutuhan | Keterangan |
|---|---|
| **FXServer** | Versi terbaru (recommended build) |
| **Framework** | ESX / QBCore / Standalone (tergantung resource) |
| **Database** | MySQL / MariaDB (jika resource membutuhkan) |
| **Dependencies** | Sesuai kebutuhan masing-masing resource |

---

## 🚀 Instalasi

1. **Clone repository** ini ke folder `resources` server FiveM Anda:
   ```bash
   git clone https://github.com/username/last-semester.git
   ```

2. **Pindahkan** folder resource yang dibutuhkan ke dalam direktori `resources` server.

3. **Tambahkan resource** ke dalam file `server.cfg`:
   ```cfg
   ensure ls-ui
   ensure ls-core
   ensure ls-jobs
   ```

4. **Restart server** atau jalankan resource secara manual melalui konsol:
   ```bash
   restart nama-resource
   ```

---

## 🛠️ Cara Penggunaan

- Sesuaikan konfigurasi pada file `config.lua` sesuai kebutuhan server.
- Jalankan server FiveM seperti biasa menggunakan `txAdmin` atau `run.cmd` / `run.sh`.
- Pastikan seluruh dependency resource sudah aktif sebelum menjalankan resource utama.
- Cek dokumentasi tambahan (jika tersedia) di dalam folder `docs/` untuk panduan lebih detail.

<details>
<summary>💬 Tips Tambahan (klik untuk melihat)</summary>

- Selalu backup database sebelum melakukan instalasi resource baru.
- Gunakan environment testing/development sebelum menerapkan ke server production.
- Periksa log konsol server untuk memastikan tidak ada error saat startup.

</details>

---

## 📦 Daftar Resource

| Resource | Deskripsi | Status |
|---|---|---|
| `ls-ui` | Kumpulan antarmuka NUI/dashboard server | ✅ Aktif |
| `ls-core` | Script inti dan fungsi dasar server | ✅ Aktif |
| `ls-jobs` | Sistem pekerjaan dan ekonomi server | 🚧 Pengembangan |

> 📌 Daftar resource akan terus diperbarui seiring perkembangan project.

---

## 🤝 Kontribusi

Kontribusi sangat terbuka untuk siapa saja yang ingin membantu mengembangkan project ini!

1. **Fork** repository ini
2. Buat **branch baru** untuk fitur/perbaikan:
   ```bash
   git checkout -b fitur-baru
   ```
3. **Commit** perubahan Anda:
   ```bash
   git commit -m "Menambahkan fitur baru"
   ```
4. **Push** ke branch Anda:
   ```bash
   git push origin fitur-baru
   ```
5. Buka **Pull Request** untuk direview

> 💡 Pastikan mengikuti gaya penulisan kode yang sudah ada agar konsistensi tetap terjaga.

---

## 📜 License

Project ini dilisensikan di bawah **MIT License**. Silakan lihat file [`LICENSE`](./LICENSE) untuk informasi lebih lanjut mengenai hak penggunaan.

---

## 👏 Credits

Terima kasih kepada seluruh pihak yang telah berkontribusi dalam pengembangan **Last Semester**, baik melalui kode, ide, maupun dukungan lainnya.

- 💻 Developer & Maintainer: *Aku Jamal*
- 🌐 Komunitas FiveM Indonesia

---

## 🎓 Penutup

Terima kasih telah menggunakan atau berkontribusi pada **Last Semester**! Semoga repository ini bermanfaat untuk mendukung pengembangan server FiveM Anda. Jangan ragu untuk membuka *issue* atau *pull request* jika menemukan bug atau memiliki ide pengembangan baru. 🚀

---

<p align="center">Made with ❤️ for FiveM Indonesian Community</p>
