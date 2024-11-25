# Tugas-2-Kecerdasan-Artifisial-2208107010064

Proyek ini menunjukkan cara membuat dan melatih model komputer (disebut CNN) yang bisa mengenali gambar dari dataset CIFAR-10. Dataset ini berisi gambar-gambar seperti pesawat, mobil, burung, kucing, dan lainnya.

## Dataset

CIFAR-10 adalah kumpulan data yang berisi 60.000 gambar berwarna dengan ukuran 32x32 piksel. Gambar-gambar ini dibagi ke dalam 10 kategori berikut:

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

Dataset ini dibagi menjadi 50.000 gambar untuk melatih model dan 10.000 gambar untuk menguji hasilnya.

## Langkah-langkah

1. **Memuat Data CIFAR-10**  
   Dataset ini dimuat dan dibagi menjadi dua bagian: data pelatihan dan data pengujian (testing).

2. **Menyiapkan Data**  
   - Gambar-gambar dinormalisasi, artinya kita mengubah nilai warna piksel ke dalam rentang antara 0 dan 1 supaya lebih mudah diproses oleh komputer.
   - Label atau kategori gambar diubah ke dalam format yang lebih mudah dipahami oleh model.

3. **Membangun Model**  
   Kita membuat model yang disebut CNN (Convolutional Neural Network). Model ini dilatih untuk mengenali pola dalam gambar menggunakan beberapa lapisan, seperti:
   - Lapisan untuk mengenali fitur-fitur gambar (seperti garis, bentuk, warna).
   - Lapisan yang mengurangi ukuran gambar (pooling).
   - Lapisan yang membuat keputusan akhir untuk menentukan kategori gambar.

4. **Melatih Model**  
   Model ini dilatih menggunakan gambar pelatihan selama 10 putaran (epoch) untuk belajar mengenali berbagai objek dengan lebih baik.

5. **Mengukur Hasil**  
   Setelah pelatihan, kita melihat bagaimana akurasi model (seberapa sering model bisa menebak dengan benar) dan seberapa baik model kita bekerja saat diuji dengan data baru.

6. **Menyimpan Model**  
   Setelah model berhasil dilatih, kita menyimpannya ke dalam file supaya bisa digunakan lagi di masa depan tanpa harus melatihnya ulang.

## Persyaratan

Agar bisa menjalankan proyek ini, Anda membutuhkan:

- Python 3.x
- TensorFlow (digunakan untuk membangun dan melatih model)
- Matplotlib (digunakan untuk menampilkan grafik)

