---
title: Deretan (Sequence)

---

# Deretan (Sequence)

Deretan adalah suatu urutan atau susunan elemen atau objek yang disusun secara teratur berdasarkan suatu aturan tertentu. Elemen dalam deretan biasanya berupa angka, huruf, simbol, atau objek lainnya, dan urutannya dapat didasarkan pada pola, nilai, atau hubungan tertentu.

**Definisi**: Sebuah deretan adalah fungsi dari subset suatu himpunan bilangan bulat (biasanya N atau P) ke sebuah himpunan S.

Contoh:
- N = {1, 2, 3, 4, ...}
- S misalnya {2, 4, 6, 8, ...}, {1/3, 1/5, 1/7, ...,}, dsb

**Notasi deretan**: {a_n}

# Deretan Umumnya Dinyatakan dalam Suatu Formula, Misalnya:

- $a_n = 2n$
- $a_n = \frac{1}{n}$
- $a_n = 7 - 3n$

Dalam konteks matematika, **deretan** sering merujuk pada barisan bilangan, yaitu kumpulan bilangan yang disusun dalam suatu pola tertentu.

Misalnya:
1. Deretan bilangan ganjil: 1, 3, 5, 7, ...
2. Deretan bilangan genap: 2, 4, 6, 8, ...
3. Deretan bilangan yang membentuk deret aritmetika: 3, 6, 9, 12, ...

---

# Contoh-Contoh Deretan dan Formulanya:

## Deret Aritmetika

Deret dengan pola kenaikan atau penurunan tetap.
- Contoh: 2, 5, 8, 11, 14, ...

### Rumus Suku ke-n:
$a_n = a + (n - 1) \cdot b$

Dimana:
- $a$: suku pertama
- $b$: beda (selisih antar suku)
- $n$: nomor suku yang dicari

---

## Deret Geometri

Deret dengan pola kelipatan tetap.
- Contoh: 3, 6, 12, 24, 48, ...

### Rumus Suku ke-n:
$a_n = a \cdot r^{(n-1)}$

Dimana:
- $a$: suku pertama
- $r$: rasio (perbandingan antar suku)
- $n$: nomor suku yang dicari

---

## Deret Bilangan Kuadrat

Deret dengan pola nilai berupa kuadrat bilangan bulat.
- Contoh: 1, 4, 9, 16, 25, ...

### Rumus Suku ke-n:
$a_n = n^2$

---

## Deret Bilangan Kubik

Deret dengan pola nilai berupa kubik bilangan bulat.
- Contoh: 1, 8, 27, 64, 125, ...

### Rumus Suku ke-n:
$a_n = n^3$

---

## Deret Fibonacci

Deret dengan pola di mana setiap suku merupakan jumlah dua suku sebelumnya.
- Contoh: 0, 1, 1, 2, 3, 5, 8, ...

### Rumus Suku ke-n (Rekursif):
$F_n = F_{n-1} + F_{n-2}, \quad F_0 = 0, \quad F_1 = 1$

---

## Deret String

Deret berupa rangkaian karakter.
- **String** adalah deretan berhingga karakter berbentuk $a_1a_2a_3 \ldots a_n$
- Panjang string S adalah jumlah karakter di dalam string tersebut
- Contoh: "informatika" adalah string dengan panjang 11 karakter, "10100101" adalah string biner dengan panjang 8 bit
- String kosong dilambangkan dengan $\lambda$, panjangnya = 0

---

# Penjumlahan Deretan

Penjumlahan deretan adalah proses menjumlahkan elemen-elemen dalam suatu deretan. Misalkan kita memiliki deretan $a_m, a_{m+1}, a_{m+2}, \ldots, a_n$, maka penjumlahannya adalah:

$a_m + a_{m+1} + a_{m+2} + \ldots + a_n$

Notasi sigma digunakan untuk menyatakan penjumlahan deretan tersebut:

$\sum_{k=m}^{n} a_k$

Dimana:
- $k$ adalah indeks summasi (indeks penjumlahan).
- $m$ adalah batas bawah indeks.
- $n$ adalah batas atas indeks.

---

## Contoh Penjumlahan Deretan

**Contoh 1: Hitunglah nilai $\sum_{k=1}^{5} k^2$**

Jawaban:

$\sum_{k=1}^{5} k^2 = 1^2 + 2^2 + 3^2 + 4^2 + 5^2 = 1 + 4 + 9 + 16 + 25 = 55$

**Contoh 2: Sumasi dapat dipecah dengan membagi dua indeksnya**

$\sum_{k=1}^{100} k^2 = \sum_{k=1}^{49} k^2 + \sum_{k=50}^{100} k^2$

**Contoh 3: Batas bawah sumasi kadangkala perlu digeser agar dapat dijumlahkan dengan sumasi lain yang memiliki batas bawah berbeda**

$\sum_{k=1}^{5} k^2 = \sum_{k=0}^{4} (k + 1)^2$

---


## Tabel Formula Penjumlahan Berguna

### TUGAS PEMBUKTIAN
Dari 3 rumus di bawah ini, buktikan:
| Sum | Closed Form | 
| --- | ----------- | 
| $\sum_{k=0}^{n} ar^k$ | $\frac{ar^{n+1} - a}{r - 1}, \ r \neq 1$ |
| $\sum_{k=1}^{n} k$ | $\frac{n(n+1)}{2}$ |
| $\sum_{k=1}^{n} k^2$ | $\frac{n(n+1)(2n+1)}{6}$ |
| $\sum_{k=1}^{n} k^3$ | $\frac{n^2(n+1)^2}{4}$ | 
| $\sum_{k=0}^{\infty} x^k,\|x\| < 1$ | $\frac{1}{1-x}$ | 
| $\sum_{k=1}^{\infty} kx^{k-1},\|x\| < 1$ | $\frac{1}{(1-x)^2}$ |

### Contoh Penjumlahan Deretan

**Contoh 5: Hitung nilai $\sum_{k=50}^{100} k^2$**

Jawaban:



$\sum_{k=50}^{100} k^2 = \sum_{k=1}^{100} k^2 - \sum_{k=1}^{49} k^2$



Gunakan rumus:



$\sum_{k=1}^{n} k^2 = \frac{n(n+1)(2n+1)}{6}$





$\sum_{k=50}^{100} k^2 = \frac{(100)(101)(201)}{6} - \frac{(49)(50)(99)}{6} = 338350 - 40425 = 297925$
# Sumasi Ganda

Di dalam algoritma, kita perlu menghitung berapa kali suatu operasi tertentu dilakukan di dalam sebuah kalang bersarang (nested loop). Penjumlahan semua operasi di dalam kalang bersarang dinyatakan dalam bentuk sumasi ganda.
Contoh: $\sum_{i=1}^{4} \sum_{j=1}^{3} ij$
Untuk menghitung sumasi ganda, mula-mula ekspansi sumasi terdalam, lalu dilanjutkan dengan sumasi terluar:
$\sum_{i=1}^{4} \sum_{j=1}^{3} ij = \sum_{i=1}^{4} (i \cdot 1 + i \cdot 2 + i \cdot 3) = \sum_{i=1}^{4} 6i = 6 \cdot 1 + 6 \cdot 2 + 6 \cdot 3 + 6 \cdot 4 = 6 + 12 + 18 + 24 = 60$

## Contoh Penggunaan Sumasi Ganda

Berapa kali operasi + dilakukan di dalam algoritma di bawah ini?

x = 0 for j = 1 to 10 do for k = 1 to j do x = x + 2 end for end for

**Penyelesaian:**

Operasi + terdapat di dalam pernyataan `x = x + 2`. Operasi ini dilakukan satu kali pada setiap pengulangan. Jumlah seluruh operasi + adalah:



$t = \sum_{j=1}^{10} \sum_{k=1}^{j} 1$





$= \sum_{j=1}^{10} (1 + 1 + ... + 1 \text{ sebanyak } j \text{ kali})$





$= \sum_{j=1}^{10} j$





$= \frac{10(10+1)}{2} = 55$

### 1. Tentukan nilai $\sum_{k=1}^{8} 2^k + \sum_{k=2}^{8} (-3)^k$
Jawaban:


$\sum_{k=1}^{8} 2^k = 2^1 + 2^2 + 2^3 + 2^4 + 2^5 + 2^6 + 2^7 + 2^8 = 2 + 4 + 8 + 16 + 32 + 64 + 128 + 256 = 510$




$\sum_{k=2}^{8} (-3)^k = (-3)^2 + (-3)^3 + (-3)^4 + (-3)^5 + (-3)^6 + (-3)^7 + (-3)^8$




$= 9 - 27 + 81 - 243 + 729 - 2187 + 6561 = 4923$




$\sum_{k=1}^{8} 2^k + \sum_{k=2}^{8} (-3)^k = 510 + 4923 = 5433$



### 2. Tentukan nilai $\sum_{i=0}^{2} \sum_{j=0}^{3} (2i + 3j)$
Jawaban:


$\sum_{i=0}^{2} \sum_{j=0}^{3} (2i + 3j) = \sum_{i=0}^{2} [(2i + 3 \cdot 0) + (2i + 3 \cdot 1) + (2i + 3 \cdot 2) + (2i + 3 \cdot 3)]$




$= \sum_{i=0}^{2} [2i + 2i + 3 + 2i + 6 + 2i + 9]$




$
= \sum_{i=0}^{2} [8i + 18]
$




$= 8 \cdot 0 + 18 + 8 \cdot 1 + 18 + 8 \cdot 2 + 18$




$= 18 + 26 + 34 = 78$



### 3. Tentukan nilai $\sum_{i=0}^{3} \sum_{j=0}^{2} i$
Jawaban:


$\sum_{i=0}^{3} \sum_{j=0}^{2} i = \sum_{i=0}^{3} [i \cdot 3] = 3 \sum_{i=0}^{3} i$




$= 3 (0 + 1 + 2 + 3) = 3 \cdot 6 = 18$

# Rekursi

- Sebuah objek dikatakan rekursif (recursive) jika ia didefinisikan dalam terminologi dirinya sendiri.
- Proses mendefinisikan objek dalam terminologi dirinya sendiri disebut rekursi (recursion).
- Perhatikan tiga buah gambar pada tiga slide berikut ini.
# Fungsi Rekursif

### Basis
- Bagian yang berisi nilai fungsi yang terdefinisi secara eksplisit.
- Bagian ini juga sekaligus menghentikan rekursif (dan memberikan sebuah nilai yang terdefinisi pada fungsi rekursif).

### Rekurens
- Bagian ini mendefinisikan fungsi dalam terminologi dirinya sendiri.
- Berisi kaidah untuk menemukan nilai fungsi pada suatu input dari nilai-nilai lainnya pada input yang lebih kecil.

### Contoh 6

Diberikan fungsi rekursif $f(n)$ sebagai berikut:

$f(n) = \begin{cases} 3, & n = 0 \\ 2f(n-1) + 4, & n > 0 \end{cases}$

Tentukan nilai $f(4)$.
s
olusi:

$f(4) = 2f(3) + 4$

$= 2(2f(2) + 4) + 4$

$= 2(2(2f(1) + 4) + 4) + 4$

$= 2(2(2(2f(0) + 4) + 4) + 4) + 4$

$= 2(2(2(2 \cdot 3 + 4) + 4) + 4) + 4$

$= 2(2(2(6 + 4) + 4) + 4) + 4$

$= 2(2(2 \cdot 10 + 4) + 4) + 4$

$= 2(2(20 + 4) + 4) + 4$

$= 2(2 \cdot 24 + 4) + 4$

$= 2(48 + 4) + 4$

$= 2 \cdot 52 + 4$

$= 108$

### Contoh 7

Nyatakan $n!$ dalam definisi rekursif

Solusi: $n! = 1 \times 2 \times 3 \times ... \times (n - 1) \times n = (n - 1)! \times n$

Misalkan $f(n) = n!$, maka

$n! = \begin{cases} 1, & n = 0 \\ n \times (n - 1)!, & n > 0 \end{cases}$

Menghitung $5!$ secara rekursif adalah:
$5! = 5 \times 4!$
$= 5 \times 4 \times 3!$
$= 5 \times 4 \times 3 \times 2!$
$= 5 \times 4 \times 3 \times 2 \times 1!$
$= 5 \times 4 \times 3 \times 2 \times 1 \times 0!$
$= 5 \times 4 \times 3 \times 2 \times 1 \times 1$
$= 120$

### Algoritma Menghitung Faktorial

function Faktorial (input n : integer) -> integer
{ 
  mengembalikan nilai n!;
  basis : jika n = 0, maka 0! = 1
  rekurens: jika n > 0, maka n! = n × (n-1)!
}

DEKLARASI


ALGORITMA:
if n = 0 then
    return 1          { basis }
else
    return n * Faktorial(n - 1)  { rekurens }
end

### Contoh 8: Barisan Fibonacci

Barisan Fibonacci didefinisikan secara rekursif sebagai berikut:

$f_n = \begin{cases} 
0, & n = 0 \\
1, & n = 1 \\
f_{n-1} + f_{n-2}, & n > 1 
\end{cases}$

### Contoh 9: Fungsi (Polinom) Chebyshev

Fungsi polinom Chebyshev didefinisikan sebagai:

$T(n, x) = \begin{cases} 
1, & n = 0 \\
x, & n = 1 \\
2x \cdot T(n-1, x) - T(n-2, x), & n > 1 
\end{cases}$
# Contoh 10

Sumasi $\sum_{k=0}^{n} a_k$ didefinisikan secara rekursif sebagai berikut:

$\sum_{k=0}^{n} a_k = a_0 + a_1 + a_2 + ... + a_{n-1} + a_n$

$= (a_0 + a_1 + a_2 + ... + a_{n-1}) + a_n$

$= \left( \sum_{k=0}^{n-1} a_k \right) + a_n$

sehingga

$\sum_{k=0}^{n} a_k = \begin{cases} a_0, & n = 0 \\ \left( \sum_{k=0}^{n-1} a_k \right) + a_n, & n > 0 \end{cases}$


# Struktur Rekursif

Struktur data yang penting dalam komputer adalah pohon biner (binary tree).

- Pohon biner adalah struktur data rekursif yang terdiri dari simpul (node) yang dihubungkan oleh cabang (branch). Setiap simpul memiliki paling banyak dua anak (child), yang disebut anak kiri (left child) dan anak kanan (right child).

## Definisi

1. Sebuah pohon kosong adalah sebuah pohon biner.
2. Sebuah pohon biner adalah simpul akar (root) yang memiliki dua pohon biner anak, yaitu anak kiri dan anak kanan.

### Contoh Pohon Biner:

Simpul | Anak Kiri | Anak Kanan
------ | --------- | ----------
A      | B         | C
B      | D         | E
C      | F         | G

Pada tabel di atas, simpul A adalah akar yang memiliki anak kiri B dan anak kanan C. Simpul B memiliki anak kiri D dan anak kanan E, dan simpul C memiliki anak kiri F dan anak kanan G.

## Traversal Pohon Biner

Traversal adalah proses mengunjungi setiap simpul dalam pohon biner.

### Tiga jenis traversal pohon biner:
1. **Inorder Traversal (Traversal dalam urutan):**
   - Kunjungi anak kiri
   - Kunjungi simpul akar
   - Kunjungi anak kanan

2. **Preorder Traversal (Traversal awal urutan):**
   - Kunjungi simpul akar
   - Kunjungi anak kiri
   - Kunjungi anak kanan

3. **Postorder Traversal (Traversal akhir urutan):**
   - Kunjungi anak kiri
   - Kunjungi anak kanan
   - Kunjungi simpul akar

### Pohon Biner

Simpul (node) pada pohon biner mempunyai paling banyak dua buah anak.

- Jumlah anak pada setiap simpul bisa 1, 2, atau 0.
- Simpul yang mempunyai anak disebut simpul cabang (branch node) atau simpul dalam (internal node).
- Simpul yang tidak mempunyai anak disebut simpul daun (leave).

# Pohon Biner Rekursif

Oleh karena itu, pohon dapat didefinisikan secara rekursif sebagai berikut:

(i) **Basis**: kosong adalah pohon biner

(ii) **Rekurens**: Jika $T_1$ dan $T_2$ adalah pohon biner, maka $•$ adalah pohon biner

Diagram:

$ T1 \quad T2 $

$ \quad \quad / \quad \ \ $ $ \quad \ \ \bullet $





# TUGAS PEMBUKTIAN
Dari 3 rumus di bawah ini, buktikan:
| Sum | Closed Form | 
| --- | ----------- | 
| $\sum_{k=0}^{n} ar^k$ | $\frac{ar^{n+1} - a}{r - 1}, \ r \neq 1$ |
| $\sum_{k=1}^{n} k$ | $\frac{n(n+1)}{2}$ |
| $\sum_{k=1}^{n} k^2$ | $\frac{n(n+1)(2n+1)}{6}$ |
| $\sum_{k=1}^{n} k^3$ | $\frac{n^2(n+1)^2}{4}$ | 
| $\sum_{k=0}^{\infty} x^k,\|x\| < 1$ | $\frac{1}{1-x}$ | 
| $\sum_{k=1}^{\infty} kx^{k-1},\|x\| < 1$ | $\frac{1}{(1-x)^2}$ |

### 1. Bukti $\sum_{k=0}^{n} ar^k = \frac{ar^{n+1} - a}{r - 1}, \ r \neq 1$

Bukti ini adalah untuk deret geometri.

Misalkan $S = \sum_{k=0}^{n} ar^k$.

$S = a + ar + ar^2 + \cdots + ar^n$

Kalikan kedua sisi dengan $r$:

$rS = ar + ar^2 + ar^3 + \cdots + ar^{n+1}$

Kurangkan persamaan pertama dari yang kedua:

$S - rS = a - ar^{n+1}$

Faktorkan $S$ pada ruas kiri dan $a$ pada ruas kanan:

$S(1 - r) = a(1 - r^{n+1})$

Bagi kedua sisi dengan $(1 - r)$:

$S = \frac{a(1 - r^{n+1})}{1 - r}$

Maka didapatkan:

$\sum_{k=0}^{n} ar^k = \frac{a(1 - r^{n+1})}{1 - r}$

---

### 2. Bukti $\sum_{k=1}^{n} k = \frac{n(n+1)}{2}$

Bukti ini adalah untuk jumlah bilangan bulat dari 1 sampai n.

Misalkan $S = \sum_{k=1}^{n} k$.

$S = 1 + 2 + 3 + \cdots + n$

Tuliskan lagi $S$ secara terbalik:

$S = n + (n-1) + (n-2) + \cdots + 1$

Jumlahkan kedua persamaan:

$2S = (1 + n) + (2 + (n-1)) + (3 + (n-2)) + \cdots + (n + 1)$

Tiap pasang jumlahnya sama dengan $(n + 1)$ dan ada $n$ pasang:

$2S = n(n + 1)$

Bagi kedua sisi dengan 2:

$S = \frac{n(n + 1)}{2}$

Maka didapatkan:

$\sum_{k=1}^{n} k = \frac{n(n+1)}{2}$

---

### 3. Bukti $\sum_{k=1}^{n} k^2 = \frac{n(n+1)(2n+1)}{6}$

Bukti ini adalah untuk jumlah bilangan kuadrat dari 1 sampai n.

Kita gunakan metode induksi matematika.

**Basis**: Untuk $n = 1$,

$\sum_{k=1}^{1} k^2 = 1^2 = 1$

dan

$\frac{1(1+1)(2 \cdot 1 + 1)}{6} = \frac{1 \cdot 2 \cdot 3}{6} = 1$

Basis terpenuhi.

**Hipotesis Induksi**: Misalkan rumus benar untuk $n = m$,

$\sum_{k=1}^{m} k^2 = \frac{m(m+1)(2m+1)}{6}$

**Langkah Induksi**: Tunjukkan bahwa rumus benar untuk $n = m+1$,

$\sum_{k=1}^{m+1} k^2 = \sum_{k=1}^{m} k^2 + (m+1)^2$

Menggunakan hipotesis induksi:

$= \frac{m(m+1)(2m+1)}{6} + (m+1)^2$

Faktorkan $(m+1)$:

$= \frac{(m+1)[m(2m+1) + 6(m+1)]}{6}$

Sederhanakan dalam kurung:

$= \frac{(m+1)[2m^2 + m + 6m + 6]}{6}
= \frac{(m+1)(2m^2 + 7m + 6)}{6}$

Faktorkan polinomial:

$= \frac{(m+1)(m+2)(2m+3)}{6}$

Maka,

$\sum_{k=1}^{m+1} k^2 = \frac{(m+1)(m+2)(2(m+1)+1)}{6}$

Yang merupakan bentuk yang sama seperti yang kita inginkan, maka bukti selesai.

Dengan bukti ini, kita telah membuktikan kebenaran ketiga rumus tersebut secara umum.


