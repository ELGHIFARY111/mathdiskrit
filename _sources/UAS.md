---
title: UAS

---
# UAS
## soal 1
| P | Q | R | S |P>Q|R>S| (P>Q)>(R>S) |
| -- | -- | -- | -- |  -- |  -- |  -- |
|  T   | T     |  T    |    T  | T |T | T |
|  T   |  F    |  F    |    F  | F |T | T |
|  T   |  T    |  F    |    T  | T |T | T |
|  T   |  T    |  T    |    F  | T |F | F |
|  T   |  F    |  T    |    F  | F |F | T |
|  F   |  F    |  F    |    F  | T |T | T |
|  T   |  T    |  F    |    T  | T |T | T |
|  F   |  F    |  T    |    T  | T |T | T |

## soal 2

![image](https://hackmd.io/_uploads/HJeepM44kl.png)




### 1. Hitung closeness centrality G
| NODE | A | B | C |D|E|F|G|
| -- | -- | -- | -- |  -- |  -- |  -- | --|
|  G   | 3     |  1    |2  | 3 |3 | 2 |0|

$Cc(G)=\frac{7-1}{(3+1+2+3+3+2)}=\frac{6}{14}$
### 2. Hitung betwennesse centrality F
$C_B(v_i) = \sum_{v_s \neq v_i \neq v_t \in V, s < t} \frac{\sigma s_{t}(v_i)}{\sigma s_t)}$

| NODE | s=B |s=C | s=G |
| -- | -- | -- | -- | 
|  t=A   |  1/1  |  1/1 | 1/1  |
|  t=D   |  1/1  |  1/1 | 1/1  |
|  t=E   |  1/1  |  1/1 | 1/1  |

$Cb(G)=6$
