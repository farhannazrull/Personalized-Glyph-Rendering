# Case Study: Personalized Glyph Rendering

Proyek ini merupakan implementasi Grafis Komputer untuk memvisualisasikan inisial nama dan digit terakhir NRP menjadi objek 3D interaktif berbasis WebGL.

## 👤 Identitas Mahasiswa

| Atribut | Detail |
| :--- | :--- |
| **Nama** | Farhan |
| **NRP** | 5025231053 |
| **Kode Glyph** | `Fa3` |

---

## 📝 Laporan Studi Kasus

Berikut adalah penjabaran teknis sesuai poin-poin studi kasus:

### 1. Identifikasi Karakter
Berdasarkan aturan pengambilan karakter:
- **Dua huruf pertama nama:** Ambil **"Fa"** dari **Fa**rhan.
- **Satu angka terakhir NRP:** Ambil **"3"** dari 502523105**3**.

### 2. Desain Karakter
Setiap karakter dirancang menggunakan bentuk primitif geometri (*Primitives*) dengan sentuhan warna dan transformasi:

| Karakter | Geometri Dasar (Primitives) | Warna Hex | Transformasi & Konsep |
| :---: | :--- | :--- | :--- |
| **F** | `BoxGeometry` (Balok) | `#00AAFF` (Cyan) | Disusun dari balok vertikal dan horizontal untuk kesan kokoh/tegas. |
| **a** | `TorusGeometry` + `CylinderGeometry` | `#FF0055` (Magenta) | Kombinasi lingkaran (donat) dan batang silinder, gaya sans-serif geometris. |
| **3** | `TubeGeometry` (Spline/Kurva) | `#FFAA00` (Emas) | Menggunakan jalur kurva (*CatmullRomCurve3*) agar lengkungan mulus tanpa patahan. **Skala diperbesar 1.1x**. |

### 3. Implementasi
- **Bahasa & Library:** Menggunakan **JavaScript (ES6)** dan **Three.js** sebagai engine WebGL.
- **Scene Setup:**
  - **Pencahayaan:** *Three-Point Lighting* (Directional, Ambient, dan Rim Light) untuk menonjolkan volume 3D.
  - **Material:** `MeshStandardMaterial` agar objek bereaksi realistis terhadap cahaya.
  - **Layout:** Posisi huruf diatur sejajar pada sumbu X dengan jarak proporsional.

### 4. Output
Hasil render ditampilkan dalam halaman web tunggal (`HTML`) dengan fitur:
- **Interaktif:** Pengguna dapat memutar (*Rotate*), menggeser (*Pan*), dan memperbesar (*Zoom*) objek.
- **Animasi:** Objek memiliki animasi *floating* (naik-turun) dan rotasi global perlahan.
- **UI:** Terdapat overlay informasi nama dan panduan kontrol.

---

## 🚀 Cara Menjalankan (How to Run)

1. Pastikan Anda memiliki koneksi internet (untuk memuat library Three.js).
2. Buka file `fa3_glyph_clean.html` menggunakan browser modern:
   - Google Chrome
   - Mozilla Firefox
   - Microsoft Edge
3. Gunakan Mouse untuk berinteraksi dengan objek 3D.

---

*Dibuat untuk memenuhi tugas Grafis Komputer.*# Case Study: Personalized Glyph Rendering

Proyek ini merupakan implementasi Grafis Komputer untuk memvisualisasikan inisial nama dan digit terakhir NRP menjadi objek 3D interaktif berbasis WebGL.

## 👤 Identitas Mahasiswa

| Atribut | Detail |
| :--- | :--- |
| **Nama** | Farhan |
| **NRP** | 5025231053 |
| **Kode Glyph** | `Fa3` |

---

## 📝 Laporan Studi Kasus

Berikut adalah penjabaran teknis sesuai poin-poin studi kasus:

### 1. Identifikasi Karakter
Berdasarkan aturan pengambilan karakter:
- **Dua huruf pertama nama:** Ambil **"Fa"** dari **Fa**rhan.
- **Satu angka terakhir NRP:** Ambil **"3"** dari 502523105**3**.

### 2. Desain Karakter
Setiap karakter dirancang menggunakan bentuk primitif geometri (*Primitives*) dengan sentuhan warna dan transformasi:

| Karakter | Geometri Dasar (Primitives) | Warna Hex | Transformasi & Konsep |
| :---: | :--- | :--- | :--- |
| **F** | `BoxGeometry` (Balok) | `#00AAFF` (Cyan) | Disusun dari balok vertikal dan horizontal untuk kesan kokoh/tegas. |
| **a** | `TorusGeometry` + `CylinderGeometry` | `#FF0055` (Magenta) | Kombinasi lingkaran (donat) dan batang silinder, gaya sans-serif geometris. |
| **3** | `TubeGeometry` (Spline/Kurva) | `#FFAA00` (Emas) | Menggunakan jalur kurva (*CatmullRomCurve3*) agar lengkungan mulus tanpa patahan. **Skala diperbesar 1.1x**. |

### 3. Implementasi
- **Bahasa & Library:** Menggunakan **JavaScript (ES6)** dan **Three.js** sebagai engine WebGL.
- **Scene Setup:**
  - **Pencahayaan:** *Three-Point Lighting* (Directional, Ambient, dan Rim Light) untuk menonjolkan volume 3D.
  - **Material:** `MeshStandardMaterial` agar objek bereaksi realistis terhadap cahaya.
  - **Layout:** Posisi huruf diatur sejajar pada sumbu X dengan jarak proporsional.

### 4. Output
Hasil render ditampilkan dalam halaman web tunggal (`HTML`) dengan fitur:
- **Interaktif:** Pengguna dapat memutar (*Rotate*), menggeser (*Pan*), dan memperbesar (*Zoom*) objek.
- **Animasi:** Objek memiliki animasi *floating* (naik-turun) dan rotasi global perlahan.
- **UI:** Terdapat overlay informasi nama dan panduan kontrol.

---

## 🚀 Cara Menjalankan (How to Run)

1. Pastikan Anda memiliki koneksi internet (untuk memuat library Three.js).
2. Buka file `fa3_glyph_clean.html` menggunakan browser modern:
   - Google Chrome
   - Mozilla Firefox
   - Microsoft Edge
3. Gunakan Mouse untuk berinteraksi dengan objek 3D.

---

*Dibuat untuk memenuhi tugas Grafis Komputer.*
