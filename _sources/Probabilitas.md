---
title: Probabilitas

---

# Probabilitas
## Probabilitas Diskrit Probabilitas Bayesian
## Teorema Bayes

Teorema Bayes memberi tahu kita cara menghitung probabilitas kondisional dari suatu peristiwa berdasarkan pengetahuan sebelumnya tentang peristiwa tersebut. Dengan kata lain, ini memungkinkan kita menghitung probabilitas posterior berdasarkan probabilitas sebelumnya:

$P(E | C) = \frac{P(C | E) \cdot P(E)}{P(C)}$

Dalam persamaan ini, kita memiliki empat istilah:
- **Probabilitas posterior \( P(E | C) \)**: probabilitas peristiwa E terjadi, dengan syarat bahwa kondisi C benar;
- **Probabilitas sebelumnya \( P(E) \)**: probabilitas tunggal peristiwa E terjadi, yang merupakan pengetahuan sebelumnya tentang peristiwa itu sendiri;
- **Likelihooh \( P(C | E) \)**: probabilitas kondisi C benar, dengan syarat bahwa peristiwa E terjadi;
- **Probabilitas marginal \( P(C) \)**: probabilitas tunggal kondisi C benar.

Jika kita mengganti beberapa hal, kita dapat menggunakan Teorema Bayes dalam masalah kita. Karena peristiwa kita didasarkan pada variabel target Beach (B), mari kita ganti Peristiwa E dengan Beach B. Selain itu, kondisi kita (ada dua) diberikan oleh dua fitur yang bernama Temperature (\(X_1\)) dan Wind (\(X_2\)), jadi mari kita ganti Kondisi C dengan fitur \(X_1, X_2\). Ingatlah bahwa karena kita memiliki dua fitur dalam masalah ini, kita akan menggunakan semacam probabilitas gabungan. Semua modifikasi ini menghasilkan persamaan berikut:

$P(B | X_1, X_2) = \frac{P(X_1, X_2 | B) \cdot P(B)}{P(X_1, X_2)}$

Jika perlu, Anda dapat menambahkan langkah ekstra di sini dan secara mental menyebutkan \(X = X_1, X_2\), sehingga persamaan menjadi lebih mudah dipahami:

$P(B | X) = \frac{P(X | B) \cdot P(B)}{P(X)}$

dan Anda selalu dapat mengganti \(X\) dengan \(X_1, X_2\).

## Variabel Independen

Langkah terbesar yang akan kita ambil sekarang adalah mengasumsikan bahwa fitur \(X_1\) dan \(X_2\) independen — sehingga nama "Naive" menjadi bagian dari model pengklasifikasi kita (Naive Bayes). Mungkin naif untuk mengasumsikan bahwa variabel-variabel ini memang independen, tetapi itu akan sangat menyederhanakan model (dan perhitungan) kita.

Jika kita menggunakan aturan produk untuk probabilitas gabungan, kita dapat menulis ulang probabilitas marginal sebagai:

$P(X) = P(X_1) \cdot P(X_2)$

Demikian juga, kita dapat menulis ulang likelihood sebagai:

$P(X_1, X_2 | B) = P(X_1 | B) \cdot P(X_2 | B)$

Kemudian, persamaan utama kita menjadi:

$P(B | X_1, X_2) = \frac{P(X_1 | B) \cdot P(X_2 | B) \cdot P(B)}{P(X_1) \cdot P(X_2)}$

Sebelum kita menyelami persamaan ini dan mulai memasukkan semua angka, mari kita lihat plot di bawah ini yang merangkum distribusi semua lima sampel yang kita miliki dari tabel di atas.

## Perhitungan Probabilitas

Sekarang kita kembali ke masalah kita: mengingat sampel baru dari fitur (\(X_1, X_2\)), kita ingin memprediksi target \(B\). Jika kita tetap pada contoh di mana Temperature = medium (\(X_1 = M\)) dan Wind = weak (\(X_2 = W\)), kita harus menghitung:

$P(B = T | X_1 = M, X_2 = W)$

dan

$P(B = F | X_1 = M, X_2 = W)$

untuk mengetahui mana yang lebih besar. Baiklah, mari kita hitung satu per satu.

### 1) Probabilitas Sebelumnya

Setiap probabilitas sebelumnya harus dihitung secara individual, tetapi perhitungannya mudah: dari semua (5) sampel, berapa banyak yang benar dan berapa banyak yang salah? Jawabannya adalah 3 dan 5, masing-masing. Jadi,

$P(B = T) = \frac{3}{5} = 0.6$

dan

$P(B = F) = \frac{2}{5} = 0.4$

Sekali lagi, ini disebut probabilitas sebelumnya karena ini adalah pengetahuan sebelum peristiwa itu sendiri, sehingga mereka dapat dihitung hanya berdasarkan sampel yang kita miliki.

### 2) Likelihoods

Sama seperti probabilitas sebelumnya, setiap persamaan probabilitas posterior akan mengarah pada likelihood-nya sendiri.

Untuk \(B = T\), kita memiliki:

$P(X_1 = M, X_2 = W | B = T) = P(X_1 = M | B = T) \cdot P(X_2 = W | B = T)$

di mana

$P(X_1 = M | B = T) = \frac{1}{3} \approx 0.33$

dan

$P(X_2 = W | B = T) = \frac{1}{3} \approx 0.33$

Ini mewakili berapa banyak fitur suhu yang sedang dari semua target beach true

Ini menunjukkan berapa banyak fitur suhu yang sedang dari semua target pantai yang benar, dan berapa banyak fitur angin yang lemah dari semua target pantai yang benar, masing-masing.

Sehingga, $P(X_1 = M, X_2 = W | B = T) = \frac{1}{3} \cdot \frac{1}{3} = \frac{1}{9} \approx 0.11$.

Dengan cara yang sama, untuk $B = F$, kita memiliki:

$P(X_1 = M, X_2 = W | B = F) = P(X_1 = M | B = F) \cdot P(X_2 = W | B = F)$, dimana $P(X_1 = M | B = F) = \frac{1}{2} = 0.5$ dan $P(X_2 = W | B = F) = \frac{1}{2} = 0.5$.

Sehingga, $P(X_1 = M, X_2 = W | B = F) = \frac{1}{2} \cdot \frac{1}{2} = \frac{1}{4} = 0.25$.

### 3) Probabilitas Marginal

Probabilitas marginal adalah sama dalam kedua persamaan yang ingin kita hitung (untuk $B = T$ dan $B = F$):

$P(X_1 = M, X_2 = W) = P(X_1 = M) \cdot P(X_2 = W)$, dimana $P(X_1 = M) = \frac{2}{5} = 0.4$ (dua suhu sedang dari semua lima sampel) dan $P(X_2 = W) = \frac{2}{5} = 0.4$ (dua angin lemah dari semua lima sampel).

Jadi, $P(X_1 = M, X_2 = W) = \frac{2}{5} \cdot \frac{2}{5} = \frac{4}{25} = 0.16$.

### 4) Probabilitas Posterior

Sekarang kita akhirnya bisa memasukkan semua nilai ke dalam dua persamaan utama kita untuk menghitung setiap probabilitas posterior:

$P(B = T | X_1 = M, X_2 = W)$ dan $P(B = F | X_1 = M, X_2 = W)$.

Karena $0.63 > 0.42$, kita bisa memprediksi bahwa $B = F$, atau mengatakan bahwa kita tidak harus pergi ke pantai, mengingat kondisi tersebut.

Probabilitas Prediksi
Langkah lain yang diambil oleh model Naive Bayes adalah menghitung probabilitas relatif untuk kedua keputusan benar dan salah. Ini dilakukan karena probabilitas posterior tidak menambahkan hingga satu ($0.63 > 0.42 = 1.05 \neq 1$ atau, jika Anda ingin lebih tepat, $\frac{5}{12} + \frac{5}{8} = \frac{25}{24} \neq 1$).

Kita dapat mendefinisikan $P_T$ sebagai probabilitas memprediksi benar dan $P_F$ sebagai probabilitas memprediksi salah sebagai berikut:

$P_T = \frac{P(B = T | X)}{P(B = T | X) + P(B = F | X)}$ dan $P_F = \frac{P(B = F | X)}{P(B = T | X) + P(B = F | X)}$.

Catatan bahwa kita mengabaikan nilai aktual untuk $X_1$ dan $X_2$ demi kesederhanaan. Juga, sekarang kita dapat memastikan bahwa $P_T + P_F = 1$.

Keuntungan utama menggunakan probabilitas (yang menambahkan hingga satu) adalah jika kita menemukan yang pertama lebih besar dari 0.5, kita dapat membuat keputusan tanpa menghitung yang kedua. Atau, jika kita berurusan dengan lebih dari dua kelas untuk variabel target kita, segera setelah kita menemukan satu probabilitas yang lebih besar dari 0.5, itu sudah menjadi jawaban kita.

Menghubungkan probabilitas posterior yang telah kita hitung memberi kita:

$P_T = \frac{0.63}{1.05} \approx 0.6$ dan $P_F = \frac{0.42}{1.05} \approx 0.4$, dan, sekali lagi, kita akan memilih $B = F$. Tetapi segera setelah kita menghitung probabilitas prediksi pertama, $P_T = 0.4$, karena $P_T < 0.5$, kita akan otomatis memprediksi kelas yang lain (selain T); yaitu, F — yang, sekali lagi, berarti kita tidak harus pergi ke pantai.

### Skor Prediksi
Kita telah menyadari bahwa kemungkinan marginal adalah sama dalam kedua kasus, sehingga bisa diabaikan jika kita hanya untuk membandingkan probabilitas posterior.

Kita dapat mendefinisikan satu konsep lagi di sini, yaitu skor yang dapat digunakan untuk membuat prediksi. Dan skor ini adalah pembilang dari persamaan probabilitas posterior kita; yaitu, produk antara kemungkinan dan probabilitas awal (tidak perlu membaginya dengan probabilitas marginal). Ini menghasilkan:

$S_T = P(X | B = T) \cdot P(B = T)$ dan $S_F = P(X | B = F) \cdot P(B = F)$.

Sebaliknya, keputusan kita dapat didasarkan pada perbandingan sederhana antara ($S_T$ dan $S_F$ tidak menambahkan hingga 1 juga).

Dalam contoh kita:

$S_T = \frac{1}{15} \approx 0.067$ dan $S_F = \frac{1}{10} = 0.1$.

Karena $0.1 > 0.067$ (SF > ST), kita akan memutuskan untuk $B = F$, seperti yang diprediksi sebelumnya: kita tidak harus pergi ke pantai.

Pada akhirnya, ketika menghitung probabilitas prediksi, probabilitas marginal juga dibatalkan secara alami. Kita bahkan dapat menulis ulang mereka sebagai fungsi dari skor prediksi:

$P_T = \frac{S_T}{S_T + S_F}$ dan $P_F = \frac{S_F}{S_T + S_F}$, dimana
## Probabilitas Hipertensi pada Usia Paruh Baya dengan Tekanan Darah Sangat Tinggi

Bagaimana kemungkinan/probabilitas usia paruh baya dengan tekanan darah sangat tinggi mengalami penyakit Hipertensi (H) atau Tidak (T)?

## Data

| No | Usia       | Tekanan Darah   | Penyakit (H/T) |
|----|------------|-----------------|----------------|
| 1  | Muda       | Normal          | T              |
| 2  | Muda       | Tinggi          | T              |
| 3  | Paruh baya | Normal          | T              |
| 4  | Paruh baya | Tinggi          | H              |
| 5  | Tua        | Normal          | H              |
| 6  | Tua        | Sangat Tinggi   | H              |
| 7  | Muda       | Normal          | T              |
| 8  | Tua        | Tinggi          | H              |

## Perhitungan

### Probabilitas Dasar

- Total data: 8
- Hipertensi (H): 4
- Tidak Hipertensi (T): 4

### Probabilitas Dasar

- $( P(H) = \frac{4}{8} = 0.5 )$
- $( P(T) = \frac{4}{8} = 0.5 )$

### Probabilitas Kondisional

#### Hipertensi (H)
- $( P(U=Paruh Baya | H) = \frac{1}{4} )$ (dari 4 orang dengan Hipertensi, 1 adalah paruh baya)
- $( P(T=Sangat Tinggi | H) = \frac{1}{4} )$ (dari 4 orang dengan Hipertensi, 1 memiliki tekanan darah sangat tinggi)

#### Tidak Hipertensi (T)
- $( P(U=Paruh Baya | T) = \frac{1}{4} )$ (dari 4 orang tanpa Hipertensi, 1 adalah paruh baya)
- $( P(T=Sangat Tinggi | T) = \frac{0}{4} = 0 )$ (dari 4 orang tanpa Hipertensi, tidak ada yang memiliki tekanan darah sangat tinggi)

### Menghitung Probabilitas

#### Hipertensi (H)



$[ 
P(H | U=Paruh Baya, T=Sangat Tinggi) = \frac{P(U=Paruh Baya | H) \cdot P(T=Sangat Tinggi | H) \cdot P(H)}{P(U=Paruh Baya, T=Sangat Tinggi)} 
]$




