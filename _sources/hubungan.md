---
title: 'G = nx.Graph([(0, 1), (0, 2), (0, 3), (1, 2), (1, 3)])'

---
# hubungan


![image](https://hackmd.io/_uploads/SJLbqI_z1x.png)




## Social Network Analysis

Social Network Analysis (SNA) adalah bidang kajian yang mengeksplorasi hubungan antar manusia menggunakan teori graf. Implementasi SNA membantu menjelaskan relasi atau hubungan antar aktor melalui visualisasi berbentuk graf. Relasi dalam analisis jaringan sosial dihitung menggunakan ukuran **centrality**, sesuai dengan posisi masing-masing aktor di dalam struktur jaringan tersebut.

Dalam **social network**, terdapat:
- **Node**: Mewakili individu atau aktor.
- **Edges**: Relasi atau hubungan antar node.

Jaringan sosial terdiri dari banyak aktor yang saling berhubungan, membentuk peta jaringan sosial yang dinyatakan dengan graf.

## Centrality

Tidak semua node dalam jaringan adalah penting. **Centrality** digunakan untuk menentukan aktor yang paling penting dalam jaringan, yang dibagi menjadi empat jenis:
1. **Degree Centrality**
2. **Closeness Centrality**
3. **Betweenness Centrality**
4. **Eigenvector Centrality**

### 1. Degree Centrality
Degree centrality adalah jumlah **edges** yang terkoneksi dengan suatu node. Pentingnya node ditentukan oleh jumlah node yang berdekatan dengannya.

$$
C_D(v) = \deg(v)
$$

#### Normalisasi Degree Centrality
Untuk node \(v\) dengan total \(n\) node:
$$
C_D^{norm}(v) = \frac{\deg(v)}{n-1}
$$

Contoh:
- Degree centrality untuk node 1 adalah \(3\).
- Normalisasi degree centrality:
$$
C_D^{norm}(1) = \frac{3}{9-1} = \frac{3}{8}.
$$

---

### 2. Closeness Centrality
Closeness centrality mengukur kedekatan antara satu node dengan node lain dalam jaringan melalui rata-rata jarak terpendek:

$$
C_C(v) = \frac{1}{\sum_{u \neq v} d(u, v)}
$$

- Skor closeness centrality menunjukkan kecepatan penyebaran informasi.
- Contoh: Node 4 lebih central daripada node 3 karena rata-rata jaraknya lebih kecil.

---

### 3. Betweenness Centrality
Betweenness centrality mengukur seberapa besar informasi melewati suatu node. Node dengan skor tinggi memainkan peran penting sebagai penghubung dalam jaringan.

$$
C_B(v) = \sum_{s \neq v \neq t} \frac{\sigma_{st}(v)}{\sigma_{st}}
$$

Di mana:
- \(\sigma_{st}\): Jumlah lintasan terpendek antara \(s\) dan \(t\).
- \(\sigma_{st}(v)\): Jumlah lintasan terpendek antara \(s\) dan \(t\) yang melewati \(v\).

#### Normalisasi Betweenness Centrality
$$
C_B^{norm}(v) = \frac{C_B(v)}{(n-1)(n-2)/2}
$$

---


