Tugas Kelompok: Linear Regression & Logistic Regression

Mata Kuliah: Fundamen Sains Data

Repositori ini berisi pengerjaan dua tugas pemodelan machine learning menggunakan Python di Google Colab.

Anggota Kelompok

1. Muhammad Dimas Satrio Domargo (25523262)
2. Abi Manyu Maheswara Ghoevara (25523084)
3. Pradhipta Widya Satria(23523129)

Deskripsi Dataset

Kami menggunakan dua dataset bawaan dari library seaborn agar kodenya bisa langsung dijalankan tanpa perlu mengunduh file CSV secara terpisah.

Bagian A (Linear Regression) - Dataset tips

Sumber: seaborn.load_dataset('tips')

Tujuan: Memprediksi jumlah tip yang diberikan pelanggan (target kontinu) berdasarkan total tagihan dan beberapa faktor pendukung lainnya.

Bagian B (Logistic Regression) - Dataset titanic

Sumber: seaborn.load_dataset('titanic')

Tujuan: Memprediksi probabilitas keselamatan penumpang kapal Titanic (target biner: selamat/tidak selamat) berdasarkan umur, jenis kelamin, kelas tiket, dll.

Ringkasan Hasil

1. Model Linear Regression (tips)

Fitur total_bill menjadi variabel yang paling berpengaruh terhadap tingginya jumlah tip.

Berdasarkan evaluasi residual plot, model masih menunjukkan gejala heteroskedastisitas (residual membesar di nilai tagihan tinggi). Kesimpulannya, model ini kurang akurat saat memprediksi tip untuk tagihan yang nominalnya sangat besar.

2. Model Logistic Regression (titanic)

Model klasifikasi berhasil mendeteksi penumpang selamat dengan metrik Recall yang tinggi karena kami menerapkan penyesuaian class_weight='balanced'.

Fitur yang paling dominan menentukan probabilitas keselamatan penumpang adalah jenis kelamin (perempuan memiliki peluang lebih tinggi) dan kelas tiket penumpang (pclass).

Pembagian Kontribusi

Agar pengerjaan tugas merata, berikut adalah rincian tugas masing-masing anggota:

[Nama Anggota 1]: Bertanggung jawab pada tahap preprocessing (menangani missing values, encoding) dan eksplorasi data (EDA).

[Nama Anggota 2]: Membangun model (Linear & Logistic) serta menyusun visualisasi untuk evaluasi model menggunakan Matplotlib/Seaborn.

[Nama Anggota 3]: Menyusun draf analisis/kesimpulan akhir, merapikan format teks (Markdown) di notebook, dan mengatur repositori GitHub.
