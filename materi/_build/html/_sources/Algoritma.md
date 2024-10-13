---
title: Algoritma

---

# Algoritma
## Definisi Algoritma
Algoritma matematika  dan  ilmu  komputer  adalah  kumpulan  perintah terkait  untuk  memecahkan  masalah(  Suhendar,  Ali,  &  Suratman,  2021). Perintah-perintah  ini  dapat  dikonversi  langkah  demi  langkah  dari  awal sampai akhir. Persiapan memerlukan urutan serta logika supaya algoritma yang  dihasilkan  cocok  dengan  yang  diharapkan.

Algoritma  memiliki  lima  karakteristik  kunci  yang  terkait  dengannya( Kusumaningtyas & Wahyuddin, 2022). 
1. Input merupakan  permasalahan  di  mana  Kamu  berpengalaman  serta mau  mencari  pemecahan.  Algoritma  mempunyai  nol  ataupun  lebih nilai input.
1. Proses,   yakni   langkah-langkah   yang   harus   dicoba   buat   mencapai tujuan akhir.
1. Output yakni  pemecahan  ataupun  penanda  akhir  yang  diperoleh  dari algoritma. Algoritma mempunyai paling tidak satu output.
1. Instruksi-instruksi  yang  jelas dan  tidak  ambigu,  yakni  instruksi  yang jelas   dalam   algoritma   sehingga   tidak   terjalin   kesalahan   dalam menghasilkan output.
1. Tujuan  akhir  yang  dicapai  merupakan  akhir  program,  serta  program berakhir kala tujuan akhir tercapai.

### Algoritma squential Search
**Pengertian Sequential Search**
Sequential search adalah teknik pencarian data yang dilakukan dengan cara membandingkan setiap elemen data satu per satu, mulai dari elemen pertama hingga elemen yang dicari ditemukan. Proses ini terus berlanjut hingga data ditemukan atau seluruh elemen telah diperiksa.

Algoritma ini termasuk salah satu algoritma pencarian yang paling sederhana dan sering digunakan dalam situasi di mana data tidak memiliki struktur tertentu.

Fungsi Sequential Search
Digunakan untuk mencari data dengan melakukan proses membandingkan setiap elemen larik secara beruntun satu persatu, mulai dari elemen pertama, sampai elemen yang dicari ditemukan, atau seluruh elemen sudah diperiksa .
Dapat digunakan untuk pengelolaan data, seperti fungsi pencarian data barang pada master data barang .
Dalam konteks pengujian kecepatan pencarian, Algoritma Sequential Search dapat digunakan dengan fungsi microtime untuk mengevaluasi kecepatan pencarian data
Cara Kerja Sequential Search
Algoritma Sequential Search bekerja dengan melakukan perbandingan satu persatu secara beruntun dalam kumpulan data dengan data yang dicari sampai data tersebut ditemukan atau tidak ditemukan.

Proses pencarian ini hanya melakukan pengulangan data dari 1 sampai dengan jumlah data (N). Setiap pengulangan, dilakukan perbandingan data ke-i dengan data yang sedang dicari. Jika data sama dengan yang dicari, berarti data telah berhasil ditemukan. Sebaliknya, jika sampai akhir pengulangan tidak ada data yang sama dengan yang dicari, berarti data tidak ditemukan.

Langkah-langkah urutan Algoritma Sequential Search:
1. Algoritma Sequential Search dimulai dari elemen pertama dalam daftar.
1. Setiap elemen dalam daftar diperiksa satu per satu secara berurutan.
1. Pemeriksaan berhenti ketika elemen yang dicari ditemukan atau ketika seluruh daftar telah diperiksa tanpa menemukan elemen yang dicari.
1. Jika elemen yang dicari ditemukan, indeks elemen tersebut dikembalikan. Jika tidak ditemukan, umumnya -1 atau nilai lain yang menunjukkan bahwa elemen tidak ditemukan dikembalikan.
### Algoritma Binary Search
Pencarian   Biner   (binary   Search)   adalah   metode pencarian  data  pada  array  yang  telah terurut,  metode  ini lebih  effisien  dari  pada  metode  pencarian  linier  dimana semua  elemen  di  dalam  array  diuji  satu  persatu  sampai ditemukan elemen yang diinginkan .
Algoritma  ini  bekerja  dengan  cara  memilih  record dengan  indeks  tengah  dari  tabel  dan  membandingkannya dengan  record  yang  hendak  dicari.  Jika  record  tersebut lebih  rendah  atau  lebih  tinggi,  maka  tabel  tersebut  dibagi dua  dan  bagian  tabel  yang  bersesuaian  akan  diproses kembali secara rekursif .

Kondisi untuk menerapkan Algoritma Pencarian Biner dalam Struktur Data Untuk menerapkan algoritma Pencarian Biner: 

* Struktur data harus diurutkan. 
* Akses ke elemen mana pun dari struktur data harus memerlukan waktu yang konstan. 

Algoritma Pencarian Biner Di bawah ini adalah algoritma langkah-demi-langkah untuk Pencarian Biner: 

1. Bagilah ruang pencarian menjadi dua bagian dengan menemukan indeks tengah "tengah".
1. Bandingkan elemen tengah ruang pencarian dengan kunci.
1. Jika kunci ditemukan di elemen tengah, proses dihentikan. 
1. Jika kunci tidak ditemukan di elemen tengah, pilih bagian mana yang akan digunakan sebagai ruang pencarian berikutnya. 
1. Jika kunci lebih kecil dari elemen tengah, maka sisi kiri yang digunakan untuk pencarian berikutnya. 
1. Jika kunci lebih besar dari elemen tengah, maka sisi kanan yang digunakan untuk pencarian berikutnya. 
1. Proses ini terus berlanjut hingga kunci ditemukan atau total ruang pencarian habis.
## Pseudocode adalah
**Pengertian Pseudocode**

Pseudocode berasal dari kata pseudo dan code yang artinya kode semu atau mirip atau menyerupai kode program yang sebenarnya dengan menggunakan suatu bahasa pemrograman tertentu. Pseudocode menggunakan simbol-simbol yang mirip atau menyerupai kode program dengan bahasa pemrograman tertentu. Flowchart dalam menjelaskan alur logika dari suatu masalah dengan menggunakan simbol-simbol khusus dengan gambar, pseudocode menggunakan kata-kata, namun keduanya mempunyai tujuan yang sama, yaitu membantu menjelaskan alur logika suatu masalah, sehingga mudah membuat program.
 
## BIG O ALGORTMA
Big O adalah notasi matematis yang digunakan untuk menggambarkan kompleksitas waktu dan ruang dari algoritma. Ini membantu kita memahami seberapa efisien suatu algoritma dalam hal penggunaan waktu dan memori seiring dengan meningkatnya ukuran input.

**Pengertian Big O**

1. **Kompleksitas Waktu**: Menunjukkan seberapa lama algoritma akan berjalan tergantung pada ukuran input. Ini memberikan gambaran tentang pertumbuhan waktu eksekusi saat ukuran data meningkat.

2. **Kompleksitas Ruang**: Menggambarkan berapa banyak memori yang digunakan oleh algoritma dalam prosesnya.

**Notasi Umum Big O**

- **O(1)**: Waktu konstan. Algoritma selesai dalam waktu yang sama terlepas dari ukuran input. Contoh: Mengakses elemen dalam array.
  
- **O(log n)**: Waktu logaritmik. Algoritma beroperasi dalam waktu yang tumbuh secara logaritmik. Contoh: Pencarian biner dalam array terurut.

- **O(n)**: Waktu linier. Waktu yang dibutuhkan tumbuh secara langsung sebanding dengan ukuran input. Contoh: Menjumlahkan elemen dalam array.

- **O(n log n)**: Waktu linier-logaritmik. Contoh: Algoritma pengurutan yang efisien seperti mergesort.

- **O(n²)**: Waktu kuadratik. Waktu yang dibutuhkan tumbuh sebanding dengan kuadrat ukuran input. Contoh: Algoritma pengurutan sederhana seperti bubble sort.

- **O(2^n)**: Waktu eksponensial. Waktu yang dibutuhkan meningkat secara eksponensial dengan penambahan elemen input. Contoh: Beberapa algoritma rekursif, seperti menghitung angka Fibonacci.

- **O(n!)**: Waktu faktorial. Waktu yang dibutuhkan tumbuh sebanding dengan faktorial dari ukuran input. Contoh: Solusi brute force untuk masalah traveling salesman.

**Pentingnya Big O**

- **Memprediksi Kinerja**: Membantu memprediksi bagaimana algoritma akan berperforma dengan input yang lebih besar.
  
- **Perbandingan Algoritma**: Memungkinkan perbandingan antara berbagai algoritma untuk memilih yang paling efisien.

- **Skalabilitas**: Memahami bagaimana algoritma akan beroperasi saat ukuran data meningkat, yang penting dalam pengembangan perangkat lunak.

Jika Anda memiliki pertanyaan lebih lanjut atau membutuhkan contoh tertentu, silakan tanyakan!

## Hitung Big O dalam Algortima Sequential Search
* **Waktu Kompleksitas**

kompleksitas waktu adalah kompleksitas komputasi yang mengggambarkan sejumlah waktu komputer yang dibutuhkan untuk menjalankan suatu algoritme. Kompleksitas waktu biasanya diperkirakan dengan menghitung jumlah operasi dasar yang dilakukan oleh algoritme, dengan assumsi bahwa setiap operasi dasar membutuhkan sejumlah waktu yang sama untuk dijalankan. Dengan demikian, jumlah waktu yang dibutuhkan dan jumlah operasi dasar yang dilakukan oleh algoritme diangggap terkait dengan faktor konstan.
### Langkah-langkah Menghitung Waktu Kompleksitas

1. **Identifikasi Algoritma**:
   - Tentukan algoritma yang ingin dianalisis. Misalnya, pengurutan, pencarian, atau operasi pada struktur data tertentu.

2. **Tentukan Input**:
   - Tentukan ukuran input, biasanya dinyatakan dengan \( n \). Ini bisa berupa jumlah elemen dalam array, panjang string, atau ukuran data lainnya.

3. **Analisis Langkah Eksekusi**:
   - Hitung jumlah operasi yang dilakukan algoritma berdasarkan ukuran input. Pertimbangkan operasi dasar seperti perbandingan, penugasan, dan pengulangan.

4. **Identifikasi Struktur Kontrol**:
   - Perhatikan loop, kondisi, dan struktur lainnya yang dapat mempengaruhi jumlah operasi. Misalnya:
     - **Loop Tunggal**: Jika ada loop yang berjalan \( n \) kali, waktu kompleksitasnya adalah \( O(n) \).
     - **Loop Bersarang**: Jika ada loop di dalam loop, waktu kompleksitasnya bisa \( O(n^2) \).

5. **Gabungkan Operasi**:
   - Jika algoritma memiliki beberapa bagian dengan waktu kompleksitas berbeda, gunakan aturan berikut:
     - **Penjumlahan**: Ambil waktu maksimum dari bagian yang berbeda.
     - **Penggandaan**: Kalikan waktu kompleksitas.

6. **Simplifikasi**:
   - Buang konstanta dan koefisien terendah. Misalnya, \( O(2n) \) disederhanakan menjadi \( O(n) \).

* **Ruang Kompleksitas**

Kompleksitas ruang adalah ukuran jumlah memori yang digunakan oleh sebuah algoritma seiring dengan pertambahan ukuran input. Ini mencakup semua jenis memori yang diperlukan untuk menjalankan algoritma, termasuk:

Ruang untuk Data Input: Memori yang digunakan untuk menyimpan data yang dimasukkan ke dalam algoritma.
Ruang untuk Variabel: Memori yang digunakan untuk menyimpan variabel lokal, variabel global, dan struktur data tambahan yang digunakan selama proses.
Ruang untuk Rekursi: Jika algoritma menggunakan rekursi, setiap panggilan rekursif mungkin memerlukan ruang tambahan di stack.
### Langkah-langkah Menghitung Kompleksitas Ruang

1. **Identifikasi Algoritma**:
   - Tentukan algoritma yang ingin dianalisis.

2. **Tentukan Input**:
   - Tentukan ukuran input, biasanya dinyatakan dengan \( n \). Ini bisa berupa jumlah elemen dalam array, panjang string, atau ukuran data lainnya.

3. **Hitung Penggunaan Memori**:
   - Identifikasi variabel yang digunakan (baik yang statis maupun dinamis).
   - Hitung ruang yang digunakan oleh variabel tersebut:
     - **Ruang Konstan**: Variabel yang tidak bergantung pada input (misalnya, beberapa integer).
     - **Ruang Dinamis**: Struktur data seperti array, list, dan lain-lain yang bergantung pada ukuran input.

4. **Gabungkan Ruang**:
   - Jumlahkan semua penggunaan ruang untuk mendapatkan total.

5. **Simplifikasi**:
   - Seperti kompleksitas waktu, buang konstanta dan fokus pada pertumbuhan yang signifikan.


## Referensi
- Putri, Meidyan P., et al. ALGORITMA DAN STRUKTUR DATA. Edited by Putri, Meidyan P. CV WIDINA MEDIA UTAMA, 2022.
- Toyib, R., Darnita, Y., & Deva, A. R. (2021). PENERAPAN ALGORITMA BINARY SEARCH PADA APLIKASI E-ORDER. JURNAL MEDIA INFOTAMA, 17(1).
- Sitorus, Lomhut, 2015, ALGORITMA dan PEMROGRAMAN, Medan: Penerbit andi.
