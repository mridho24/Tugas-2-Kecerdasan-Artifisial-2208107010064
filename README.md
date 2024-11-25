# Tugas-2-Kecerdasan-Artifisial-2208107010064

## Jenis Kasus
Klasifikasi Gambar

## Dataset yang Digunakan
Dataset yang digunakan adalah **CIFAR-10**, yang berisi gambar-gambar berukuran 32x32 piksel dari 10 kelas yang berbeda. Anda bisa mengunduhnya di [CIFAR-10 Dataset](https://www.cs.toronto.edu/~kriz/cifar.html).

## Jumlah Fitur
Setiap gambar pada dataset CIFAR-10 memiliki dimensi **32x32 piksel** dengan **3 saluran warna (RGB)**, sehingga jumlah fitur (input) untuk setiap gambar adalah: 3,072 fitur


## Jumlah Label
Dataset CIFAR-10 memiliki **10 kelas** yang berbeda, yaitu:
- Pesawat
- Mobil
- Burung
- Kucing
- Rusa
- Anjing
- Kodok
- Kuda
- Kapal
- Truk

## Jenis Jaringan Saraf Tiruan yang Digunakan
Model ini menggunakan **Convolutional Neural Network (CNN)**, yang sangat efektif untuk tugas klasifikasi gambar.

## Jenis Optimisasi
Model ini menggunakan **Adam optimizer**, sebuah algoritma optimisasi yang sering digunakan dalam pelatihan jaringan saraf tiruan, karena memiliki kemampuan adaptif yang baik.

## Jenis Fungsi Aktivasi yang Digunakan
- **Lapisan Konvolusi & Dense Pertama:** Menggunakan fungsi aktivasi **ReLU (Rectified Linear Unit)**.
- **Lapisan Output:** Menggunakan fungsi aktivasi **Softmax**, yang mengubah output menjadi probabilitas untuk klasifikasi multi-kelas.

## Jumlah Hidden Layer
- **Lapisan Konvolusi Pertama:** 32 filter
- **Lapisan Konvolusi Kedua:** 64 filter
- **Lapisan Konvolusi Ketiga:** 128 filter
- **Lapisan Dense Pertama:** 128 node

## Jumlah Total Hidden Node per Layer
Total jumlah node (termasuk output) pada model ini adalah: 352 node

## Jumlah Total Bobot (Weight)
Jumlah total bobot (weights) yang digunakan dalam model ini adalah **110,050**.

-----------------------------

## Deskripsi Model
Model CNN ini terdiri dari tiga lapisan konvolusi yang dilanjutkan dengan lapisan Dense untuk klasifikasi 10 kelas gambar. Setiap lapisan konvolusi diikuti dengan lapisan pooling untuk mengurangi dimensi data, dan lapisan Dense digunakan untuk menghubungkan hasil ekstraksi fitur ke kelas output. Fungsi aktivasi ReLU digunakan untuk lapisan tersembunyi, sementara Softmax digunakan di lapisan output untuk klasifikasi multi-kelas.



