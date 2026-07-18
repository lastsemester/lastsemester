<div align="center">

<img src="https://avatars.githubusercontent.com/u/306572549?s=400&u=8d8b00a8a4df26b2267da611b13be660e495dd5b" width="140" alt="Last Semester Logo" />

# 🎓 Last Semester

**FiveM Roleplay Server — Kehidupan Kampus, Perjuangan Akademik, dan Cerita yang Tak Pernah Usai**

[![Repository](https://img.shields.io/badge/Repository-last--semester--fivem-1f2937?style=for-the-badge&logo=github)](https://github.com/lastsemester/last-semester-fivem)
[![FiveM](https://img.shields.io/badge/Platform-FiveM-f97316?style=for-the-badge&logo=data:image/png;base64,&logoColor=white)](https://fivem.net)
[![Lua](https://img.shields.io/badge/Lua-5.4-2c2d72?style=for-the-badge&logo=lua&logoColor=white)](https://www.lua.org)
[![Roleplay](https://img.shields.io/badge/Genre-Roleplay-9333ea?style=for-the-badge)]()
[![Status](https://img.shields.io/badge/Status-In%20Development-22c55e?style=for-the-badge)]()
[![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)](#-lisensi)

</div>

---

## 📖 Deskripsi Singkat

**Last Semester** adalah repository resmi yang menjadi pusat pengembangan seluruh resource FiveM untuk server roleplay **Last Semester**. Di sini tersimpan script, asset, konfigurasi, antarmuka pengguna (UI), serta berbagai berkas pendukung lain yang dibutuhkan untuk membangun, memelihara, dan menjalankan server secara efisien dan terstruktur.

---

## 🏫 Tentang Last Semester

> *"Setiap mahasiswa baru membawa cerita. Setiap semester menulis babnya sendiri."*

**Last Semester** adalah server **FiveM Roleplay** yang mengangkat tema kehidupan pendidikan dan universitas — sebuah dunia di mana pemain tidak hanya bermain peran, tetapi benar-benar *menjalani* kehidupan kampus dari sudut pandang yang autentik. Pengembangan server ini dimulai pada **13 Juni 2026**, dengan visi menghadirkan simulasi roleplay yang jarang dieksplorasi di ekosistem FiveM: dunia akademik yang hidup dan penuh dinamika.

Di Last Semester, setiap karakter memulai perjalanannya sebagai mahasiswa baru — canggung, penuh harap, dan siap beradaptasi dengan ritme kehidupan kampus. Dari ruang kelas yang menuntut fokus, tugas dan ujian yang menguji ketekunan, hingga organisasi mahasiswa yang membentuk jaringan sosial dan kepemimpinan, setiap keputusan membawa konsekuensi nyata terhadap arah cerita masing-masing pemain.

Namun kehidupan kampus bukan hanya tentang akademik. Di luar kelas, dunia sosial berjalan penuh warna: pertemanan yang terjalin di kantin, rivalitas antar organisasi, kisah cinta yang tumbuh di sudut taman kampus, hingga dinamika UKM dan komunitas yang membentuk identitas setiap mahasiswa. Semuanya dirancang untuk menciptakan pengalaman roleplay yang imersif, membumi, dan relevan dengan kehidupan nyata.

Perjalanan setiap karakter berakhir pada satu tujuan besar: **kelulusan** — puncak dari seluruh perjuangan, relasi, dan keputusan yang telah diambil sepanjang masa perkuliahan. Last Semester bukan sekadar server roleplay, melainkan sebuah narasi panjang tentang tumbuh, berjuang, dan menemukan jati diri di tengah riuhnya kehidupan kampus.

---

## ✨ Fitur & Tujuan Repository

Repository ini dirancang sebagai pusat pengembangan yang rapi, modular, dan mudah dikelola untuk seluruh kebutuhan server Last Semester.

| Aspek | Deskripsi |
|---|---|
| 🧩 **Modular Resources** | Setiap sistem (akademik, sosial, ekonomi, dll.) dikembangkan sebagai resource terpisah agar mudah dipelihara |
| 🎨 **Custom NUI/UI** | Antarmuka pengguna khas bertema kampus, dirancang modern dan intuitif |
| 🗂️ **Konfigurasi Terpusat** | Pengaturan server, job, dan sistem tersimpan rapi dan terdokumentasi |
| 🔄 **Version Control Rapi** | Struktur commit dan branching yang mendukung kolaborasi tim developer |
| 🧑‍🎓 **Tema Edukasi Otentik** | Sistem roleplay yang secara khusus mensimulasikan kehidupan universitas |
| 🚀 **Deployment Efisien** | Disusun agar proses instalasi dan maintenance server menjadi lebih cepat |

---

## 🗂️ Struktur Folder

Berikut contoh struktur direktori pada repository ini:

```
last-semester-fivem/
├── [academic]/              # Sistem perkuliahan, kelas, dan nilai
│   ├── ls-classroom/
│   └── ls-lecturer/
├── [core]/                  # Resource inti server (framework, database, dll.)
│   ├── ls-core/
│   └── ls-multichar/
├── [interface]/             # NUI, HUD, dan dashboard antarmuka
│   ├── ls-nui-dashboard/
│   └── ls-hud/
├── [social]/                 # Organisasi kampus, komunitas, dan sistem sosial
│   ├── ls-organization/
│   └── ls-social/
├── [maps]/                  # Custom map kampus dan fasilitas pendukung
│   └── ls-campus-map/
├── config/                  # Berkas konfigurasi umum server
├── docs/                    # Dokumentasi teknis dan panduan developer
└── README.md
```

> 📌 Struktur di atas bersifat contoh dan dapat berkembang mengikuti kebutuhan pengembangan server.

---

## ⚙️ Cara Penggunaan

### Prasyarat
- Server **FiveM** (build terbaru direkomendasikan)
- Framework dasar yang kompatibel (ESX/QBCore atau custom framework Last Semester)
- Database MySQL (disarankan menggunakan `oxmysql`)

### Instalasi

1. **Clone repository ini** ke dalam folder `resources` server FiveM Anda:
   ```bash
   git clone https://github.com/lastsemester/last-semester-fivem.git
   ```

2. **Pindahkan atau salin** setiap resource ke direktori `resources` sesuai kategori masing-masing.

3. **Tambahkan resource** ke dalam `server.cfg`:
   ```cfg
   ensure ls-core
   ensure ls-classroom
   ensure ls-nui-dashboard
   ```

4. **Import database** (jika resource menyertakan file `.sql`) melalui phpMyAdmin, HeidiSQL, atau tools sejenis.

5. **Restart server** dan pastikan seluruh resource berjalan tanpa error pada konsol.

---

## 🤝 Kontribusi

Kontribusi dari rekan developer sangat terbuka untuk membantu pengembangan Last Semester menjadi lebih baik. Sebelum berkontribusi, mohon perhatikan alur berikut:

1. **Fork** repository ini.
2. Buat branch baru untuk fitur atau perbaikan Anda:
   ```bash
   git checkout -b fitur/nama-fitur-anda
   ```
3. Lakukan commit dengan pesan yang jelas dan deskriptif.
4. Ajukan **Pull Request** ke branch utama beserta penjelasan perubahan yang dilakukan.
5. Tunggu proses review dari tim maintainer sebelum perubahan digabungkan.

> Setiap kontribusi, sekecil apa pun, adalah langkah nyata dalam membangun dunia kampus Last Semester yang lebih hidup.

---

## 📜 Lisensi

Proyek ini dilisensikan di bawah **MIT License**. Silakan gunakan, modifikasi, dan kembangkan dengan tetap mencantumkan atribusi yang sesuai.

---

<div align="center">

---

> *"Kita tidak hanya kuliah untuk lulus — kita kuliah untuk menemukan siapa diri kita sebenarnya."*
> **— Last Semester**

<sub>© 2026 Last Semester. Dibangun dengan dedikasi untuk komunitas roleplay Indonesia.</sub>

</div>
