# SEWALAYAN MOBILE // FLUTTER CLIENT

> **Peer-to-Peer Sustainable Rental Platform — Conscious Shopping & Sustainable Living**

**Sewalayan Mobile** adalah aplikasi klien mobile multiplatform berbasis **Flutter** untuk ekosistem sewa-menyewa barang antar-pengguna **Sewalayan**. Platform ini mendorong pola konsumsi yang lebih bijak dengan memungkinkan pengguna menyewakan barang yang jarang terpakai sekaligus menyewa barang milik pengguna lain—mengurangi pemborosan akibat pembelian barang sesekali sekaligus membuka peluang penghasilan tambahan bagi pemilik barang.

---

## 📱 Mobile Scope & Architecture Overview

Aplikasi ini dirancang sebagai klien mobile untuk alur utama **Sewalayan** dengan pemisahan fitur per modul agar pengembangan paralel antaranggota tim tetap terukur dan minim konflik:

* **Modular Feature Structure:** Setiap modul dipisahkan ke dalam struktur fitur masing-masing di bawah direktori `lib/` agar mudah dirawat dan dikembangkan bertahap.
* **Core Navigation & Shared UI:** Navigasi antar-halaman dan komponen antarmuka bersama dikelola secara terpusat untuk menjaga konsistensi alur pengguna di perangkat mobile.
* **Backend & API Integration:** Terhubung dengan layanan backend / REST API **Sewalayan** untuk sinkronisasi data autentikasi, katalog barang, proses penyewaan, serta ulasan dan pelaporan.

---

## 👥 Engineering Roster (PBP-E-10)

| Nama | NPM | Tanggung Jawab Modul |
| :--- | :--- | :--- |
| **Asmiranda Ghina Winandari** | `25006564882` | **User & Profile** |
| **Jordan Manaksak Hutahaean** | `2506532580` | **Item** |
| **Faeiz Faiza Fasha** | `2506602196` | **Rental** |
| **Lavida Yuthiana Faizah** | `2506605941` | **Review and Report** |

---

## 🧩 Core Modules

### 01 // User & Profile
**Owner:** Asmiranda Ghina Winandari (`25006564882`)

Mengelola autentikasi dan profil pengguna pada aplikasi mobile, mencakup registrasi, login, dan logout, serta pembuatan dan pembaruan data profil seperti nama, foto, bio, lokasi, dan kontak dengan pembatasan akses sesuai hak pengguna.

### 02 // Item
**Owner:** Jordan Manaksak Hutahaean (`2506532580`)

Mengelola seluruh data barang yang disewakan melalui antarmuka mobile—mulai dari menambah, melihat, mengubah, hingga menghapus barang. Mendukung pencarian serta penyaringan berdasarkan kategori, harga, kondisi, dan lokasi, serta integrasi layanan lokasi untuk informasi barang.

### 03 // Rental
**Owner:** Faeiz Faiza Fasha (`2506602196`)

Mengelola alur penyewaan barang di aplikasi mobile dari tahap pengajuan hingga selesai, meliputi pemilihan tanggal sewa, kalkulasi total biaya, pemantauan riwayat penyewaan, serta pengelolaan status rental (`Pending`, `Accepted`, `Active`, `Completed`, dan `Cancelled`).

### 04 // Review and Report
**Owner:** Lavida Yuthiana Faizah (`2506605941`)

Mengelola sistem ulasan dan pelaporan pengguna. Penyewa dapat memberikan rating (`1–5`) serta menambah, mengubah, atau menghapus ulasan pada pesanan yang telah selesai; ulasan dan rata-rata rating ditampilkan pada detail barang. Pengguna juga dapat melaporkan barang atau pengguna bermasalah dari detail pesanan—barang terkait akan dinonaktifkan sementara hingga ditinjau admin untuk ditandai, diblokir pengguna terlapornya, atau diaktifkan kembali.

---

## 🔐 Access Roles

* **User:** Dapat menyewakan barang, mencari dan menyewa barang milik pengguna lain, mengelola profil, menjalankan alur penyewaan, memberikan ulasan, serta mengajukan laporan atas barang atau pengguna yang bermasalah.
* **Admin:** Bertugas mengelola data platform, memantau dan memproses laporan pengguna, serta melakukan moderasi konten atau akun yang melanggar aturan demi menjaga keamanan dan kenyamanan ekosistem **Sewalayan**.

---
