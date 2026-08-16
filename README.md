# 📘 Kelas XI - Dart Programming

[![Dart](https://img.shields.io/badge/Dart-Language-0175C2.svg)](https://dart.dev/)

Repositori ini berisi modul pembelajaran interaktif berbasis web untuk siswa Kelas XI SMK bidang Rekayasa Perangkat Lunak (RPL). *Course* ini dirancang khusus untuk membangun pondasi logika pemrograman menggunakan bahasa **Dart**, sebelum siswa benar-benar terjun ke dalam pengembangan antarmuka aplikasi *mobile* menggunakan *framework* **Flutter**.

## ✨ Fitur Utama Modul

- **Pendekatan Analogi:** Setiap konsep teknis yang berat (seperti OOP, Asynchronous, dan Memory) selalu dijelaskan menggunakan perumpamaan kehidupan sehari-hari.
- **Micro-Learning:** Materi dipecah menjadi halaman-halaman yang singkat, padat, dan langsung ke intinya.
- **Kuis Interaktif Vanilla:** Dilengkapi dengan kuis mandiri di akhir setiap bab untuk menguji pemahaman siswa secara langsung.
- **Adaptif Dark Mode:** Menggunakan tema *MkDocs Material* yang indah dengan pergantian mode terang/gelap otomatis.
- **Tugas Terpandu:** Dilengkapi dengan *Starter Kit* Github untuk menguji kemampuan OOP siswa di akhir bab.

## 🗂️ Struktur Kurikulum

Materi disusun secara sistematis (*step-by-step*):
1. **Dart Dasar:** Variabel, Tipe Data, Functions, Null Safety, dll.
2. **Control Flow:** Percabangan dan Perulangan.
3. **OOP Dasar:** Class, Object, Constructor, Inheritance.
4. **Futures (Asynchronous):** Sinkron vs Asinkron, `async/await`, `try-catch`.
5. **OOP Lanjutan:** Abstract Class, Interface, Mixins, Extension Method.
6. **Materi Opsional:** Functional Programming, Generics.

## 🚀 Cara Menjalankan Secara Lokal (*Local Development*)

Untuk menjalankan *website course* ini di komputermu sendiri:

1. Pastikan kamu sudah menginstal [Python](https://www.python.org/downloads/) dan `pip`.
2. Instal MkDocs dan Tema Material melalui terminal:
   ```bash
   pip install mkdocs mkdocs-material
   ```
3. *Clone* repositori ini:
   ```bash
   git clone <url-repo-github>
   cd kelas_xi_dart_dasar
   ```
4. Jalankan server lokal:
   ```bash
   mkdocs serve
   ```
5. Buka browser dan akses `http://127.0.0.1:8000`.
