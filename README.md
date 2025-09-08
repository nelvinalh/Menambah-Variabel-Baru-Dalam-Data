# Menambah Variabel Baru Dalam Data

Proyek ini adalah latihan eksplorasi data sederhana dengan dataset **Titanic**.  
Tujuannya adalah **menambah wawasan** dari data dengan cara membuat beberapa variabel baru yang bisa membantu kita melihat pola keselamatan penumpang.

---

## ✨ Apa yang Dilakukan?

Pada data Titanic, awalnya hanya ada informasi dasar seperti usia, jenis kelamin, kelas tiket, pelabuhan keberangkatan, dll.  
Di proyek ini saya **menambahkan variabel baru** supaya analisis lebih mudah dimengerti, terutama untuk orang awam.

---

## 🆕 Variabel Baru yang Ditambahkan

### 1. `social_status` (Status Sosial)  
- Dibuat berdasarkan **kelas tiket (pclass)**.  
- Penumpang kelas 1 dianggap **High Class**, kelas 2 → **Middle Class**, dan kelas 3 → **Lower Class**.  
- Tujuannya: melihat apakah status sosial berhubungan dengan peluang selamat.

---

### 2. `origin_city` (Asal Kota)  
- Dibuat dari kolom **embarked** (kode pelabuhan keberangkatan).  
- Kode diubah menjadi nama kota:
  - `C` → Cherbourg  
  - `Q` → Queenstown  
  - `S` → Southampton  
- Tujuannya: mengetahui apakah ada perbedaan peluang selamat berdasarkan kota keberangkatan.

---

### 3. `profession` (Profesi / Peran Sosial — versi simulasi)  
- Karena dataset Titanic bawaan tidak punya nama lengkap, kita buat **simulasi sederhana**:  
  - Anak-anak (< 12 tahun) → `Child`  
  - Perempuan dewasa → `Woman`  
  - Laki-laki dewasa → `Man`  
- Tujuannya: membedakan kelompok penumpang berdasarkan usia & gender untuk melihat pola keselamatan.

---

## 🔎 Kenapa Ditambah Variabel Baru?

Menambahkan variabel seperti ini disebut **data enrichment**.  
Alasannya:  
- Membantu **membaca cerita** di balik data (misalnya: siapa yang lebih banyak selamat?).  
- Memudahkan **visualisasi** (misalnya grafik perbandingan selamat/tidak selamat berdasarkan status sosial).  
- Bisa jadi langkah awal sebelum melakukan analisis yang lebih lanjut atau modeling.

---

## 📊 Hasil Singkat

- Penumpang dari **kelas atas (High Class)** cenderung lebih banyak selamat.  
- **Perempuan dan anak-anak** memiliki peluang keselamatan lebih tinggi.  
- Ada sedikit perbedaan tingkat keselamatan berdasarkan **asal kota** penumpang.  

---

## 🚀 Rencana Pengembangan

Jika menggunakan dataset Titanic yang lebih lengkap (seperti dari Kaggle), masih bisa ditambahkan variabel baru lainnya, misalnya:  
- **Title/Gelar** dari nama (Mr, Mrs, Dr) → lebih akurat untuk profesi/status sosial.  
- **Lokasi kabin (deck)** dari kolom Cabin → untuk melihat apakah letak kabin berpengaruh pada keselamatan.  

---
