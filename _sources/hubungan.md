---
title: 'G = nx.Graph([(0, 1), (0, 2), (0, 3), (1, 2), (1, 3)])'

---



![image](https://hackmd.io/_uploads/SJLbqI_z1x.png)



Materi tentang **centrality dalam graf graf** (graph centrality) merupakan salah satu bagian penting dari teori graf dalam ilmu matematika diskret dan ilmu komputer. Centrality adalah konsep yang digunakan untuk mengukur seberapa penting atau terhubungnya suatu simpul (node) dalam sebuah graf. Ada beberapa jenis ukuran centrality yang digunakan, masing-masing dengan pendekatan dan kegunaan yang berbeda:

---

### **1. Degree Centrality**
- **Definisi**: Mengukur jumlah hubungan langsung (edges) yang dimiliki suatu simpul.
- **Rumus**: 
  \[
  C_D(v) = \frac{\text{degree}(v)}{n-1}
  \]
  di mana \(n\) adalah jumlah simpul dalam graf, dan \(\text{degree}(v)\) adalah jumlah tetangga simpul \(v\).
- **Kegunaan**:
  - Menunjukkan simpul yang paling terhubung langsung dengan simpul lain.
  - Cocok untuk graf tidak berarah.

---

### **2. Betweenness Centrality**
- **Definisi**: Mengukur seberapa sering sebuah simpul menjadi jembatan (penghubung) antara pasangan simpul lainnya.
- **Rumus**:
  \[
  C_B(v) = \sum_{s \neq v \neq t} \frac{\sigma_{st}(v)}{\sigma_{st}}
  \]
  di mana:
  - \(\sigma_{st}\) adalah jumlah lintasan terpendek antara simpul \(s\) dan \(t\).
  - \(\sigma_{st}(v)\) adalah jumlah lintasan terpendek yang melalui \(v\).
- **Kegunaan**:
  - Menentukan simpul yang memiliki peran penting dalam pengaliran informasi di jaringan.

---

### **3. Closeness Centrality**
- **Definisi**: Mengukur kedekatan suatu simpul dengan semua simpul lain dalam graf.
- **Rumus**:
  \[
  C_C(v) = \frac{n-1}{\sum_{u \neq v} d(v, u)}
  \]
  di mana \(d(v, u)\) adalah jarak terpendek antara simpul \(v\) dan \(u\).
- **Kegunaan**:
  - Menunjukkan simpul yang paling cepat menjangkau simpul lain dalam graf.
  - Sering digunakan dalam analisis jaringan komunikasi.

