<h>Tugas Membuktikan Rumus</h1>

# himpunan

## 1. Hukum De Morgan

Hukum De Morgan menyatakan bahwa:

$$\overline{A \cap B} = \overline{A} \cup \overline{B}$$
$$\overline{A \cup B} = \overline{A} \cap \overline{B}$$

<p><strong>PEMBUKTIAN</strong></p>

### Contoh Hukum De Morgan dengan Himpunan

Misalkan kita memiliki dua himpunan berikut:

- $A = \{2, 4, 6\}$
- $B = \{4, 5, 7\}$

Dan ruang semesta$U$adalah:

- $U = \{1, 2, 3, 4, 5, 6, 7, 8\}$

#### a. Hukum De Morgan untuk Irisan

$$\overline{A \cap B} = \overline{A} \cup \overline{B}$$

**Langkah-langkah:**

1. **Cari irisan$A \cap B$:**

  $A \cap B = \{4\}$

2. **Hitung komplemen dari$A \cap B$di ruang semesta$U$:**

  $$\overline{(A \cap B)} = U - (A \cap B) = \{1, 2, 3, 4, 5, 6, 7, 8\} - \{4\} = \{1, 2, 3, 5, 6, 7, 8\}$$

3. **Hitung komplemen dari masing-masing himpunan$A$dan$B$:**

   - $$\overline{A} = U - A = \{1, 2, 3, 4, 5, 6, 7, 8\} - \{2, 4, 6\} = \{1, 3, 5, 7, 8\}$$
   - $$\overline{B} = U - B = \{1, 2, 3, 4, 5, 6, 7, 8\} - \{4, 5, 7\} = \{1, 2, 3, 6, 8\}$$

4. **Hitung gabungan dari$( \overline{A} )$dan$( \overline{B} )$:**

  $$\overline{A} \cup \overline{B} = \{1, 3, 5, 7, 8\} \cup \{1, 2, 3, 6, 8\} = \{1, 2, 3, 5, 6, 7, 8\}$$

5. **Bandingkan hasilnya:**

   - $$\overline{(A \cap B)} = \{1, 2, 3, 5, 6, 7, 8\}$$
   - $$\overline{A} \cup \overline{B} = \{1, 2, 3, 5, 6, 7, 8\}$$

Dengan demikian, kita dapat lihat bahwa:
$$\overline{(A \cap B)} = \overline{A} \cup \overline{B}$$

#### b. Hukum De Morgan untuk Gabungan

$$\overline{(A \cup B)} = \overline{A} \cap \overline{B}$$

**Langkah-langkah:**

1. **Cari gabungan$A \cup B$:**

  $( A \cup B = \{2, 4, 6\} \cup \{4, 5, 7\} = \{2, 4, 5, 6, 7\} )$

2. **Hitung komplemen dari$A \cup B$di ruang semesta$U$:**

  $$\overline{(A \cup B)} = U - (A \cup B) = \{1, 2, 3, 4, 5, 6, 7, 8\} - \{2, 4, 5, 6, 7\} = \{1, 3, 8\}$$

3. **Hitung irisan dari$\overline{A}$dan$\overline{B}$:**

   - $$\overline{A} = \{1, 3, 5, 7, 8\}$$
   - $$\overline{B} = \{1, 2, 3, 6, 8\}$$
   - $$\overline{A} \cap \overline{B} = \{1, 3, 5, 7, 8\} \cap \{1, 2, 3, 6, 8\} = \{1, 3, 8\}$$

4. **Bandingkan hasilnya:**

   - $$\overline{(A \cup B)} = \{1, 3, 8\}$$
   - $$\overline{A} \cap \overline{B} = \{1, 3, 8\}$$

Dengan demikian, kita dapat lihat bahwa:
$$\overline{(A \cup B)} = \overline{A} \cap \overline{B}$$

### Kesimpulan

Kedua hukum De Morgan terbukti benar dengan contoh ini.

---

## 2. Hukum Absorption

Hukum Absorpsi dalam teori himpunan menyatakan dua hal berikut:

- **Hukum Absorpsi untuk Gabungan (Union):**
  
 $$A \cup (A \cap B) = A$$

- **Hukum Absorpsi untuk Irisan (Intersection):**

 $$A \cap (A \cup B) = A$$

### Contoh Hukum Absorpsi dengan Himpunan

Misalkan kita memiliki dua himpunan berikut:

- $A = \{1, 2, 3\}$
- $B = \{3, 4, 5\}$

Dan ruang semesta$U$adalah:

- $U = \{1, 2, 3, 4, 5, 6\}$

#### a. Hukum Absorpsi untuk Gabungan

$$A \cup (A \cap B) = A$$

**Langkah-langkah:**

1. **Hitung irisan$A \cap B$:**

  $$A \cap B = \{3\}$$

2. **Hitung gabungan$A \cup (A \cap B)$:**

  $$A \cup (A \cap B) = \{1, 2, 3\} \cup \{3\} = \{1, 2, 3\}$$

   Dengan demikian:

  $$A \cup (A \cap B) = A$$

   Jadi, hukum absorpsi untuk gabungan terbukti benar.

#### b. Hukum Absorpsi untuk Irisan

$$A \cap (A \cup B) = A$$

**Langkah-langkah:**

1. **Hitung gabungan$A \cup B$:**

  $$A \cup B = \{1, 2, 3\} \cup \{3, 4, 5\} = \{1, 2, 3, 4, 5\}$$

2. **Hitung irisan$A \cap (A \cup B)$:**

  $$A \cap (A \cup B) = \{1, 2, 3\} \cap \{1, 2, 3, 4, 5\} = \{1, 2, 3\}$$

   Dengan demikian:

  $$A \cap (A \cup B) = A$$

   Jadi, hukum absorpsi untuk irisan terbukti benar.

### Kesimpulan

Dengan menggunakan contoh ini, kita telah membuktikan bahwa hukum absorpsi dalam teori himpunan benar:

- **Hukum Absorpsi untuk Gabungan:** 
 $$A \cup (A \cap B) = A$$
- **Hukum Absorpsi untuk Irisan:** 
 $$A \cap (A \cup B) = A$$

---

## 3. Hukum Komplemen

Hukum Komplemen dalam teori himpunan menyatakan dua hal berikut:

- **Hukum Komplemen untuk Gabungan (Union):**

 $$A \cup \overline{A} = U$$

- **Hukum Komplemen untuk Irisan (Intersection):**

 $$A \cap \overline{A} = \emptyset$$

### Contoh Hukum Komplemen dengan Himpunan

Misalkan kita memiliki himpunan berikut:

- $A = \{2, 4, 6\}$
- Ruang semesta$U = \{1, 2, 3, 4, 5, 6, 7, 8\}$

#### a. Hukum Komplemen untuk Gabungan

$$A \cup \overline{A} = U$$

**Langkah-langkah:**

1. **Hitung komplemen dari$A$di ruang semesta$U$:**

  $$\overline{A} = U - A = \{1, 2, 3, 4, 5, 6, 7, 8\} - \{2, 4, 6\} = \{1, 3, 5, 7, 8\}$$

2. **Hitung gabungan$A \cup \overline{A}$:**

  $$A \cup \overline{A} = \{2, 4, 6\} \cup \{1, 3, 5, 7, 8\} = \{1, 2, 3, 4, 5, 6, 7, 8\}$$

   Dengan demikian:

  $$A \cup \overline{A} = U$$

   Jadi, hukum komplemen untuk gabungan terbukti benar.

#### b. Hukum Komplemen untuk Irisan

$$A \cap \overline{A} = \emptyset$$

**Langkah-langkah:**

1. **Hitung komplemen dari$A$di ruang semesta$U$(sudah dihitung di atas):**

  $$\overline{A} = \{1, 3, 5, 7, 8\}$$

2. **Hitung irisan$A \cap \overline{A}$:**

  $$A \cap \overline{A} = \{2, 4, 6\} \cap \{1, 3, 5, 7, 8\} = \emptyset$$

   Dengan demikian:

  $$A \cap \overline{A} = \emptyset$$

   Jadi, hukum komplemen untuk irisan terbukti benar.

### Kesimpulan

Dengan menggunakan contoh ini, kita telah membuktikan bahwa hukum komplemen dalam teori himpunan benar:

- **Hukum Komplemen untuk Gabungan:** 
 $$A \cup \overline{A} = U$$
  
- **Hukum Komplemen untuk Irisan:**
 $$A \cap \overline{A} = \emptyset$$

Hukum ini membantu dalam memahami bagaimana komplemen himpunan berinteraksi dengan himpunan itu sendiri dan ruang semesta.


