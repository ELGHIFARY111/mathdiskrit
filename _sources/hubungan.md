---
title: 'G = nx.Graph([(0, 1), (0, 2), (0, 3), (1, 2), (1, 3)])'

---
# hubungan


![image](https://hackmd.io/_uploads/SJLbqI_z1x.png)



Materi tentang **centrality dalam graf graf** (graph centrality) merupakan salah satu bagian penting dari teori graf dalam ilmu matematika diskret dan ilmu komputer. Centrality adalah konsep yang digunakan untuk mengukur seberapa penting atau terhubungnya suatu simpul (node) dalam sebuah graf. Ada beberapa jenis ukuran centrality yang digunakan, masing-masing dengan pendekatan dan kegunaan yang berbeda:

---

### **1. Degree Centrality**
- **Definisi**: Mengukur jumlah hubungan langsung (edges) yang dimiliki suatu simpul.
- **Rumus**: 
  $[
  C_D(v) = \frac{\text{degree}(v)}{n-1}
  ]$
  di mana $(n)$ adalah jumlah simpul dalam graf, dan $(\text{degree}(v))$ adalah jumlah tetangga simpul $(v)$.
- Contoh Aplikasi:
Jaringan Sosial:
Dalam media sosial, simpul dengan degree centrality tinggi adalah akun yang memiliki banyak koneksi langsung, seperti teman atau pengikut.
Sistem Transportasi:
Dalam jaringan transportasi, simpul dengan degree tinggi dapat mewakili stasiun pusat yang memiliki banyak jalur langsung ke stasiun lain.
Ekosistem Biologi:
Pada graf interaksi spesies, simpul dengan degree tinggi adalah spesies yang memiliki banyak interaksi dengan spesies lain.
Kelebihan:
Mudah dihitung.
Memberikan wawasan langsung tentang konektivitas lokal simpul.
Kekurangan:
Tidak mempertimbangkan posisi simpul dalam graf secara keseluruhan.
Tidak relevan untuk jaringan di mana lintasan tidak langsung lebih penting.
---

### **2. Betweenness Centrality**
- **Definisi**: Mengukur seberapa sering sebuah simpul menjadi jembatan (penghubung) antara pasangan simpul lainnya.
- **Rumus**:
  $[
  C_B(v) = \sum_{s \neq v \neq t} \frac{\sigma_{st}(v)}{\sigma_{st}}
  ]$
  di mana:
  - $(\sigma_{st})$ adalah jumlah lintasan terpendek antara simpul $(s)$ dan $(t)$.
  - $(\sigma_{st}(v))$ adalah jumlah lintasan terpendek yang melalui $(v)$.
- **Kegunaan**:
  - Menentukan simpul yang memiliki peran penting dalam pengaliran informasi di jaringan.
Contoh Aplikasi:
Jaringan Komunikasi:
Simpul dengan betweenness centrality tinggi dapat menjadi simpul kunci dalam menyampaikan informasi antar kelompok.
Sistem Transportasi:
Dalam jaringan jalan, simpul dengan betweenness tinggi bisa menjadi kota transit utama.
Jaringan Sosial:
Dalam sebuah komunitas, simpul dengan betweenness tinggi sering berfungsi sebagai jembatan yang menghubungkan subkelompok.
Kelebihan:
Mampu mengidentifikasi simpul strategis yang mengendalikan aliran informasi atau sumber daya.
Sangat berguna dalam memahami struktur jaringan secara menyeluruh.
Kekurangan:
Perhitungan betweenness centrality sangat mahal secara komputasi untuk graf besar.
Tidak mempertimbangkan koneksi langsung simpul itu sendiri.
---

### **3. Closeness Centrality**
- **Definisi**: Mengukur kedekatan suatu simpul dengan semua simpul lain dalam graf.
- **Rumus**:
  $[
  C_C(v) = \frac{n-1}{\sum_{u \neq v} d(v, u)}
  ]$
  di mana $(d(v, u))$ adalah jarak terpendek antara simpul $(v)$ dan $(u)$.
- **Kegunaan**:
  - Menunjukkan simpul yang paling cepat menjangkau simpul lain dalam graf.
  - Sering digunakan dalam analisis jaringan komunikasi.
Contoh Aplikasi:
Jaringan Logistik:
Dalam jaringan distribusi, simpul dengan closeness tinggi menunjukkan lokasi strategis untuk pusat distribusi yang dapat menjangkau semua titik dengan cepat.
Epidemiologi:
Dalam graf penyebaran penyakit, simpul dengan closeness tinggi adalah individu atau lokasi yang berpotensi menjadi sumber penyebaran lebih cepat.
Sistem Informasi:
Dalam jaringan komputer, simpul dengan closeness tinggi memungkinkan akses data lebih efisien ke seluruh simpul lain.
Kelebihan:
Memberikan wawasan tentang efisiensi simpul dalam jaringan.
Berguna dalam jaringan yang mengutamakan kecepatan aliran informasi.
Kekurangan:
Tidak relevan untuk graf yang tidak terhubung secara sempurna (disconnected graph), karena jarak menjadi tak terhingga untuk beberapa pasangan simpul.
Mengabaikan faktor bobot dalam koneksi (kecuali diimplementasikan untuk graf berbobot).
---
