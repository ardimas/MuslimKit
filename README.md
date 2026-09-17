# MuslimKit

**All-in-One Islamic Companion App — 100% On-Device, 100% Offline**

MuslimKit adalah aplikasi Android pendamping ibadah Islami yang menggabungkan kecerdasan buatan (AI) dengan panduan syar'i, semuanya berjalan sepenuhnya lokal di perangkat tanpa memerlukan koneksi internet (kecuali untuk fitur opsional seperti terjemahan ayat & unduhan paket bahasa).

---

## ✨ Fitur Utama

### 🕌 Jadwal Shalat & Shalat Sunnah
- Perhitungan waktu shalat astronomis offline (mendukung berbagai metode kalkulasi: MABIMS, Umm al-Qura, Mesir, Karachi, Turki, ISNA, MWL, dan Auto-Detect berdasarkan lokasi)
- Notifikasi per waktu shalat dengan 4 pilihan (Adzan, Suara Standar, Senyap, Nonaktif)
- **Rawatib & Witir**: tampilan terkelompok shalat sunnah Rawatib Mu'akkad (Qabliyah/Ba'diyah) di sekitar shalat Fardhu, dengan 3 pilihan pelaksanaan Witir
- **Shalat Sunnah Custom**: tambahkan Dhuha, Tahajud, Taubat, Hajat, Istikharah (atau shalat/pengingat custom lainnya) lengkap dengan niat, panduan rakaat, dan **validasi waktu sesuai kaidah fiqih** (mis. Dhuha dikunci ke rentang terbit matahari s.d. menjelang Dzuhur; Tahajud ke rentang Isya s.d. Subuh; waktu-waktu terlarang shalat sunnah otomatis diblokir)
- Modal niat interaktif dengan pilihan peran (Sendiri/Makmum/Imam) untuk shalat Fardhu

### 🎯 Rakaat Counter (AI)
- Deteksi otomatis jumlah raka'at menggunakan Google ML Kit Pose Detection — cukup letakkan HP, AI yang menghitung
- Berjalan 100% on-device, tidak ada data yang dikirim ke server manapun

### 🧭 Kompas Kiblat
- Penunjuk arah kiblat presisi berbasis sensor magnetometer perangkat

### 📿 Tasbih Digital
- Preset dzikir (Tasbih, Tahmid, Takbir, Istighfar, Dzikir Setelah Shalat, dll.) dengan target hitungan
- Progres tiap preset independen — pindah preset tidak menghapus progres yang sedang berjalan
- Reset otomatis harian, dengan indikator visual preset yang sudah mencapai target

### 📖 Al-Qur'an Digital
- Teks Arab lengkap 114 surah dengan murottal audio per ayat
- Terjemahan multi-bahasa (real-time via API untuk bahasa selain Indonesia)
- Bookmark, pencarian surah/ayat, navigasi per Juz, mode highlight tajwid
- Pengaturan pengulangan ayat (repeat per-ayat/rentang, kecepatan playback)

### 📅 Kalender Dual (Masehi & Hijriah)
- Grid kalender dengan Masehi atau Hijriah sebagai tampilan utama (bisa ditukar), lengkap tanggal padanan di bawahnya
- Koreksi offset Hijriah manual (-2 s.d. +2 hari) untuk menyesuaikan pengumuman resmi wilayah setempat
- **Info Puasa Sunnah & Terlarang** otomatis: Ayyamul Bidh, Tasu'a, Asyura, 6 Hari Syawal, Arafah (dianjurkan) serta Idul Fitri, Idul Adha, Hari Tasyrik (terlarang)
- **Hari Besar Islam**: Tahun Baru Islam, Maulid Nabi, Isra Mi'raj, Nisfu Sya'ban, Awal Ramadhan, Idul Fitri, Idul Adha
- **Reminder Puasa Sunnah** otomatis (H-1 & Sahur) dengan waktu yang bisa dikustomisasi, plus deep-link notifikasi langsung ke tanggal terkait
- **Agenda Personal**: catatan & acara (dengan jam + reminder otomatis 15/10/5 menit sebelum mulai), bisa dilihat per hari, minggu, atau bulan

### 🌍 Dukungan 15 Bahasa
Indonesia, English, العربية, Français, Deutsch, Русский, Bahasa Melayu, Nederlands, اردو, Türkçe, Español, বাংলা, 中文, 日本語, 한국어 — dengan paket bahasa yang bisa diunduh terpisah agar ukuran APK tetap kecil.

---

## 📲 Instalasi

Unduh APK langsung dari halaman **[Releases](https://github.com/ardimas/MuslimKit/releases)** repo ini — pilih rilis terbaru, unduh file `.apk` di bagian Assets, lalu instal di perangkat Android (aktifkan "Install from unknown sources" jika diminta).

---

## 🔢 Skema Versi

Versi mengikuti [Semantic Versioning](https://semver.org/) (`MAJOR.MINOR.PATCH`), mencerminkan rilis publik yang sudah diuji & stabil.

| Versi  | Tanggal | Highlight                                                                                                                                                  |
| ------ | ------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| v1.0.0 | 2026-09 | Rilis publik pertama — Rakaat Counter AI, Jadwal Shalat + Rawatib/Witir/Shalat Sunnah Custom, Kiblat, Tasbih, Al-Qur'an, Kalender Dual + Agenda, 15 bahasa |

Lihat [CHANGELOG.md](CHANGELOG.md) untuk rincian lengkap setiap rilis.

---

## 🌐 Paket Bahasa

File paket bahasa (JSON) untuk 12 bahasa yang bisa diunduh terpisah ada di folder [`lang_packs/`](lang_packs/) repo ini. Aplikasi mengunduh paket ini otomatis saat pengguna memilih bahasa yang belum dibundel (Indonesia, English, dan Arabic sudah dibundel langsung di APK).

---

## 📄 Lisensi

*(Isi sesuai lisensi yang kamu pilih — mis. MIT, GPL-3.0, atau proprietary/all-rights-reserved kalau belum open source penuh.)*

---

## 🐞 Lapor Bug / Saran Fitur

Semua laporan bug dan saran fitur silakan dibuka lewat **[Issues](../../issues/new/choose)** repo ini — pilih template yang sesuai (Bug Report / Feature Request) di [`.github/ISSUE_TEMPLATE`](.github/ISSUE_TEMPLATE).
