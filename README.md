# 📸 Timemark Photo Generator (Pro Creator)

**Timemark Photo Generator** adalah aplikasi web berbasis *client-side* sederhana, cepat, dan responsif untuk menambahkan stempel watermark berupa **waktu, lokasi geotag (koordinat & alamat lengkap), serta catatan kegiatan** pada satu atau banyak foto (*batch processing*) sekaligus.

Aplikasi ini dirancang khusus untuk kemudahan pelaporan kegiatan lapangan (seperti kunjungan dinas, pendataan, inspeksi, dan dokumentasi program) tanpa perlu mengunggah foto ke server luar—semua pemrosesan dilakukan secara lokal di browser Anda untuk menjaga privasi data.

---

## ✨ Fitur Utama

- **📦 Multi-Photo Batch Processing**: Tambahkan puluhan foto sekaligus, edit metadata tiap foto atau terapkan data ke seluruh foto secara masal.
- **📍 Geotagging & Pencarian Lokasi**:
  - **Pencarian Alamat**: Cari otomatis nama jalan, desa, kecamatan, atau kota berbasis *Nominatim OpenStreetMap*.
  - **GPS Otomatis**: Ambil posisi titik koordinat presisi langsung dari sensor GPS perangkat.
  - **Input Manual**: Ubah latitude, longitude, dan nama daerah secara bebas.
- **🕒 Waktu & Catatan Fleksibel**:
  - Konversi otomatis tanggal ke hari dan format *DD/MM/YYYY*.
  - Tambahkan deskripsi atau catatan kegiatan pada foto.
- **🎨 Custom Watermark Verified**:
  - Opsi menampilkan/menyembunyikan watermark logo khas *Timemark* di pojok kanan atas.
  - Kustomisasi kode verifikasi unik (*Verification Code*).
- **📋 Tangkap Gambar dari Clipboard**: Tempel gambar langsung menggunakan pintasan `Ctrl + V` atau tombol paste.
- **⚡ Ekspor Cepat**:
  - Unduh foto individual yang sedang diaktifkan.
  - Unduh semua foto sekaligus dalam format **.ZIP** serentak.
- **🔒 Safe & Private**: Tanpa backend / server. Foto Anda **100% diproses di browser sendiri** (Client-side HTML5 Canvas).

---

## 🛠️ Teknologi yang Digunakan

Aplikasi ini dibangun menggunakan pustaka standar web yang ringan dan modern:

- **HTML5 & JavaScript (ES6+)**
- **[Tailwind CSS](https://tailwindcss.com/)** (Via CDN) - Penataan antarmuka & responsivitas web.
- **[Font Awesome 6](https://fontawesome.com/)** - Ikon antarmuka.
- **[JSZip](https://stuk.github.g/jszip/)** - Ekspor file kompresi `.zip` untuk pengunduhan masal.
- **[Nominatim OpenStreetMap API](https://nominatim.org/)** - Layanan *Geocoding* & *Reverse Geocoding* gratis.

---

## 🚀 Cara Penggunaan

### 1. Membuka Aplikasi
Cukup buka file `timemark-generator.html` di peramban web (*browser*) favorit Anda (Google Chrome, Mozilla Firefox, Edge, atau Safari). Tidak memerlukan instalasi server atau `node_modules`.

### 2. Mengunggah Foto
- Klik area **"Tambah Foto"** untuk memilih berkas foto dari perangkat Anda.
- Atau **Seret & Lepas (Drag and Drop)** beberapa foto sekaligus ke area pengunggahan.
- Atau tekan `Ctrl + V` untuk menempelkan (*paste*) gambar dari papan klip (*clipboard*).

### 3. Mengatur Lokasi & Geotag
- **Gunakan GPS Saya**: Klik tombol **"GPS Saya"** untuk mengambil posisi latitude & longitude riil perangkat Anda saat ini.
- **Cari Alamat**: Masukkan nama tempat/jalan di kolom pencarian lalu klik **"Cari"**.
- Edit teks nama desa, kecamatan/kabupaten, dan koordinat secara manual bila diperlukan.

### 4. Mengatur Waktu & Catatan
- Atur jam, tanggal, hari, dan teks catatan kegiatan pada form yang tersedia.
- Gunakan tombol:
  - **"Terapkan lokasi ke semua foto"**: Meng-copy data lokasi saja ke seluruh daftar foto.
  - **"Terapkan semua tag ke semua foto"**: Meng-copy seluruh info (lokasi, waktu, & catatan) ke semua foto.

### 5. Mengunduh Hasil
- Klik **"Unduh Foto Ini"** untuk menyimpan foto yang sedang dipratinjau dalam format `.jpg`.
- Klik **"Unduh Semua (ZIP)"** untuk memproses seluruh foto dan mengunduhnya sekaligus dalam satu file compressed `.zip`.

---

## 📂 Struktur Berkas

```text
├── timemark-generator.html  # Berkas tunggal utama (HTML, CSS Tailwind, & Logic JavaScript)
└── README.md                # Dokumentasi proyek
```

---

## 📄 Lisensi

Proyek ini bersifat bebas dan terbuka (*Open Source*). Anda dapat memodifikasi dan mengembangkannya sesuai kebutuhan pelaporan Anda.