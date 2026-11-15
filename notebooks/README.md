# Analisis Dataset Steam — Milestone 1

Notebook ini berisi analisis data eksploratif (EDA) untuk dataset platform game Steam. Dokumentasi di bawah ini menjelaskan tentang dataset, sumber, cara menjalankan program, serta ringkasan temuan utama.

---

## 1. Deskripsi Dataset & Sumber
* **Nama Dataset**: Steam Games Dataset
* **Sumber Data**: [GitHub - Rayhan193 Steam Dataset](https://raw.githubusercontent.com/Rayhan193/statistika-probabilitas-uniska/refs/heads/main/steam.csv)
* **Deskripsi**: Dataset ini mencakup daftar game yang rilis di platform Steam beserta berbagai atribut penting, seperti nama game, tanggal rilis, pengembang (developer), penerbit (publisher), sistem operasi yang didukung (platforms), batasan umur, jumlah prestasi (achievements), jumlah penilaian positif & negatif, rata-rata waktu bermain, dan harga game (price).

---

## 2. Cara Menjalankan Notebook
Untuk menjalankan analisis ini di Google Colab, ikuti langkah-langkah berikut:
1. **Hubungkan Runtime**: Klik tombol **Connect** di pojok kanan atas untuk menghubungkan runtime Google Colab.
2. **Jalankan Secara Berurutan**: Jalankan setiap sel kode mulai dari atas ke bawah secara berurutan dengan menekan tombol **Play** atau pintasan `Shift + Enter`.
3. **Langkah Kerja Utama**:
   * **STEP 1**: Memuat pustaka visualisasi (`pandas`, `seaborn`, `matplotlib`) dan mengimpor dataset secara langsung melalui URL raw GitHub.
   * **STEP 2**: Memeriksa keberadaan nilai kosong (*missing values*) serta data ganda (*duplicates*).
   * **STEP 3 & 4**: Menghitung ukuran pemusatan data (Mean, Median) dan penyebaran data (Standar Deviasi, IQR, CV).
   * **STEP 5 & 6**: Menampilkan visualisasi data secara grafis (Univariate & Bivariate).

---

## 3. Ringkasan Insight Utama
* **Pasar Didominasi Game Murah**: Setengah dari total game di Steam dijual dengan harga di bawah **$3.99 USD** (nilai median), menunjukkan bahwa pasar Steam sangat ramah untuk game indie atau game dengan harga terjangkau.
* **Harga Tidak Menjamin Popularitas**: Tidak ditemukan korelasi antara harga game dengan jumlah rating positif atau durasi bermain. Banyak game gratis (*free-to-play*) justru memiliki keterlibatan pemain (*user engagement*) yang jauh lebih tinggi daripada game berbayar mahal.
* **Fenomena Keterlibatan Ekstrem**: Sebagian besar game di Steam hampir tidak pernah dimainkan secara signifikan oleh pembelinya (median waktu bermain adalah 0 jam), namun ada sebagian kecil game populer yang dimainkan secara masif hingga ratusan ribu jam oleh komunitasnya.
