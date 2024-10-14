---
title: boolean

---
# boolean
## aljabar boolean
Aljabar Boolean adalah sistem matematika untuk manipulasi variabel yang dapat memiliki salah satu dari dua nilai.  
Dalam logika formal, nilai-nilai ini adalah "benar" dan "salah."  
Dalam sistem digital, nilai-nilai ini adalah "nyala" dan "mati," 1 dan 0, atau "tinggi" dan "rendah."  
Ekspresi Boolean dibuat dengan melakukan operasi pada variabel Boolean.  
Operator Boolean yang umum termasuk AND (AND), (OR), dan (NOT).

Berikut adalah pengisian tabel berdasarkan kombinasi variabel Boolean \( x \) dan \( y \):

|  x  |  y  | AND FORM       | OR FORM        | NOT FORM       |
| --- | --- | --------------- | --------------- | --------------- |
|  0  |  0  | \( 0 \land 0 = 0 \) | \( 0 \lor 0 = 0 \) | \( \neg 0 = 1 \) |
|  0  |  1  | \( 0 \land 1 = 0 \) | \( 0 \lor 1 = 1 \) | \( \neg 0 = 1 \) |
|  1  |  0  | \( 1 \land 0 = 0 \) | \( 1 \lor 0 = 1 \) | \( \neg 1 = 0 \) |
|  1  |  1  | \( 1 \land 1 = 1 \) | \( 1 \lor 1 = 1 \) | \( \neg 1 = 0 \) |


### fungsi boolean
Sebuah fungsi Boolean memiliki: 
Setidaknya satu variabel Boolean, 
Setidaknya satu operator Boolean, dan 
Setidaknya satu input dari himpunan {0,1}. 
Fungsi ini menghasilkan output yang juga merupakan anggota dari himpunan {0,1}.


| Identity Name    | AND FORM           | OR FORM             |
| ---------------- | ------------------ | ------------------- |
| Identity LAW     | $1x=x$             | $0+x=x$             |
| Null Law         | $0x=0$             | $1+x=1$             |
| Idempotent Law   | $xx=x$             | $x+x=x$             |
| Invers Law       | $x\overline {x}=0$ | $x+\overline {x}=1$ |
| Comunicative Law | $xy=yx$            | $x+y=y+x$           |
| Associative Law  | $(xy)z=x(yz)$      | $(x+y)+z=x+(y+z)$   |
| Distributive Law | $x+yz=x(x+y)(x+z)$ | $x(y+z)=xy+xz$      |
|Absorption Law De Morgan' Law|$x(x+y)=x$ atau $\overline {(xy)}=\overline {x}+\overline {y}$ |$x+xy=x$ atau $\overline {(x+y)}=\overline {x}\overline {y}$                   |
|Double Complemen Law|$\overline {(\overline{x})}=x$|$\overline {(\overline{x})}=x$                     |

## Logic gates
Fungsi Boolean diimplementasikan dalam sirkuit komputer digital yang disebut gerbang (gates).  

Gerbang adalah perangkat elektronik yang menghasilkan hasil berdasarkan dua atau lebih nilai input.  

Dalam kenyataannya, gerbang terdiri dari satu hingga enam transistor, tetapi desainer digital menganggapnya sebagai satu kesatuan.  

Sirkuit terintegrasi mengandung kumpulan gerbang yang sesuai untuk tujuan tertentu..

Tiga gerbang AND, OR, XOR, dan  NOT.



### Tabel Gerbang Logika

| Nama Gerbang | Simbol IEC | Simbol Amerika | Fungsi / Karakteristik | Tabel Kebenaran |
|--------------|------------|----------------|------------------------|-----------------|
| AND Gate     |![image](https://hackmd.io/_uploads/r1eaF_KJkl.png)|![image](https://hackmd.io/_uploads/BJMM9dFJye.png)| Gerbang AND terdiri dari dua input atau lebih. Jika salah satu input = 0 maka output = 0.<br> Y = A · B | <table><tr><th>A</th><th>B</th><th>AB</th></tr><tr><td>0</td><td>0</td><td>0</td></tr><tr><td>0</td><td>1</td><td>0</td></tr><tr><td>1</td><td>0</td><td>0</td></tr><tr><td>1</td><td>1</td><td>1</td></tr></table> |
| OR Gate      |![image](https://hackmd.io/_uploads/By5ZhuKJyl.png)|![image](https://hackmd.io/_uploads/H1Qm3OK1Jl.png)| Gerbang OR terdiri dari dua input atau lebih. Jika salah satu input = 1 maka output = 1.<br> Y = A + B | <table><tr><th>A</th><th>B</th><th>A+B</th></tr><tr><td>0</td><td>0</td><td>0</td></tr><tr><td>0</td><td>1</td><td>1</td></tr><tr><td>1</td><td>0</td><td>1</td></tr><tr><td>1</td><td>1</td><td>1</td></tr></table> |
| NOT Gate     |![image](https://hackmd.io/_uploads/r1xTnOYkJg.png)|![image](https://hackmd.io/_uploads/S1jA2_Y1Jx.png)    | Gerbang NOT hanya memiliki satu input. Output merupakan kebalikan dari input.<br> Y = Ā | <table><tr><th>A</th><th>Ā</th></tr><tr><td>0</td><td>1</td></tr><tr><td>1</td><td>0</td></tr></table> |
| NAND Gate    |![image](https://hackmd.io/_uploads/S1WQTdFykl.png)|![image](https://hackmd.io/_uploads/SJQE6dFJkg.png)          | Gerbang NAND terdiri dari dua input. Jika salah satu input = 0 maka output = 1.<br> Y = A̅B̅ | <table><tr><th>A</th><th>B</th><th>A̅B̅</th></tr><tr><td>0</td><td>0</td><td>1</td></tr><tr><td>0</td><td>1</td><td>1</td></tr><tr><td>1</td><td>0</td><td>1</td></tr><tr><td>1</td><td>1</td><td>0</td></tr></table> |
| NOR Gate     |![image](https://hackmd.io/_uploads/HJ7B6dKyye.png)|![image](https://hackmd.io/_uploads/HJX86_Kkyl.png)       | Gerbang NOR terdiri dari dua input atau lebih. Jika salah satu input = 1 maka output = 0.<br> Y = A̅ + B̅ | <table><tr><th>A</th><th>B</th><th>A̅+B̅</th></tr><tr><td>0</td><td>0</td><td>1</td></tr><tr><td>0</td><td>1</td><td>0</td></tr><tr><td>1</td><td>0</td><td>0</td></tr><tr><td>1</td><td>1</td><td>0</td></tr></table> |
| X-OR Gate    |![image](https://hackmd.io/_uploads/HJ4_6OYkJl.png)|![image](https://hackmd.io/_uploads/SkztTdt1Jg.png)      | Gerbang X-OR hanya terdiri dari dua input. Jika kedua input sama maka output = 0.<br> Y = A ⊕ B | <table><tr><th>A</th><th>B</th><th>A⊕B</th></tr><tr><td>0</td><td>0</td><td>0</td></tr><tr><td>0</td><td>1</td><td>1</td></tr><tr><td>1</td><td>0</td><td>1</td></tr><tr><td>1</td><td>1</td><td>0</td></tr></table> |
| X-NOR Gate   |![image](https://hackmd.io/_uploads/r1J5p_tykg.png)| ![image](https://hackmd.io/_uploads/S1n9TdYyye.png)      | Gerbang X-NOR hanya terdiri dari dua input. Jika kedua input sama maka output = 1.<br> $Y = A ⊙ B$ atau $Y = \overline{A ⊕ B}$ | <table><tr><th>A</th><th>B</th><th>A⊙B</th></tr><tr><td>0</td><td>0</td><td>1</td></tr><tr><td>0</td><td>1</td><td>0</td></tr><tr><td>1</td><td>0</td><td>0</td></tr><tr><td>1</td><td>1</td><td>1</td></tr></table> |

Gerbang dapat memiliki beberapa input dan lebih dari 1 output
![image](https://hackmd.io/_uploads/BJoS7FY1kg.png)

komponen digital
kombinasi gebang menerapkan fungsi boolean.
contoh :
![image](https://hackmd.io/_uploads/rk9LNFYJJg.png)

Sirkuit Kombinasi

Pendahuluan

Sirkuit kombinasi adalah jenis sirkuit logika di mana outputnya hanya bergantung pada kombinasi input saat ini. Tidak ada memori yang terlibat dalam sirkuit ini, sehingga output selalu merupakan fungsi dari input.

 Definisi

- **Input:** Sinyal yang diberikan ke sirkuit.
- **Output:** Sinyal yang dihasilkan oleh sirkuit.
- **Gerbang Logika:** Komponen dasar sirkuit kombinasi seperti AND, OR, dan NOT.

Half adder adalah sirkuit logika yang digunakan untuk menjumlahkan dua bit biner. Half adder menghasilkan dua keluaran: sum (S) dan carry (C).

Tabel Kebenaran
| A | B | Sum (S) | Carry (C) |
|---|---|---------|-----------|
| 0 | 0 |    0    |     0     |
| 0 | 1 |    1    |     0     |
| 1 | 0 |    1    |     0     |
| 1 | 1 |    0    |     1     |

Rumus
Keluaran dari half adder dapat dinyatakan dengan rumus berikut:
- $Sum (S): ( S = A \oplus B )$
- $Carry (C): ( C = A \cdot B )$

## Referensi


1. David Harris dan Sarah Harris, **Digital Design and Computer Architecture**, 2nd Edition. Morgan Kaufmann, 2015.
2. K. J. Ray Liu, **Introduction to Digital Circuits**, Wiley, 2008.
3. **Gerbang Logika Dasar**. Tersedia di: [https://katahugo.wordpress.com/2015/04/15/gerbang-logika-dasar/](https://katahugo.wordpress.com/2015/04/15/gerbang-logika-dasar/) (diakses pada 13 Oktober 2024).

