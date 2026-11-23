# Solusi Soal Latihan Kalkulus
## Notasi Sigma, Metode Trapesium, dan Integral Fungsi Dasar

---

## BAGIAN A: NOTASI SIGMA

### Soal 1
**Misalkan S adalah himpunan bilangan bulat positif yang habis dibagi oleh 4. Tentukan jumlah dari 50 bilangan terkecil anggota S.**

Himpunan S = {4, 8, 12, 16, ..., 200} (50 suku pertama)

Ini adalah barisan aritmetika dengan:
- a = 4 (suku pertama)
- b = 4 (beda)
- n = 50 (jumlah suku)

Suku ke-50: $U_{50} = 4 + (50-1) \times 4 = 4 + 196 = 200$

Jumlah 50 suku pertama:
$$S_{50} = \frac{n}{2}(a + U_n) = \frac{50}{2}(4 + 200) = 25 \times 204 = \boxed{5100}$$

---

### Soal 2
**Uraikan notasi sigma berikut dalam bentuk penjumlahan suku-sukunya.**

$$\sum_{i=1}^{n} \frac{3i - 1}{n}$$

Uraian:
$$\frac{3(1) - 1}{n} + \frac{3(2) - 1}{n} + \frac{3(3) - 1}{n} + \cdots + \frac{3(n) - 1}{n}$$

$$= \frac{2}{n} + \frac{5}{n} + \frac{8}{n} + \cdots + \frac{3n - 1}{n}$$

---

### Soal 3
**Tuliskan penjumlahan n suku berikut dalam notasi sigma.**

$$\left[\left(\frac{1}{n}\right)^3 + 1\right] + \left[\left(\frac{2}{n}\right)^3 + 2\right] + \cdots + \left[\left(\frac{n}{n}\right)^3 + n\right]$$

Polanya: $\left(\frac{i}{n}\right)^3 + i$ untuk $i = 1$ sampai $n$

Jawaban:
$$\sum_{i=1}^{n} \left[ \left(\frac{i}{n}\right)^3 + i \right]$$

---

### Soal 4
**Dengan sifat-sifat notasi sigma dan rumus-rumus jumlah ($\sum k$, $\sum k^2$, $\sum k^3$), carilah nilai notasi sigma berikut dalam bentuk paling sederhana (dalam n).**

$$\sum_{k=1}^{n} \frac{(3k - 2)k}{n^3} = \sum_{k=1}^{n} \frac{3k^2 - 2k}{n^3}$$

$$= \frac{1}{n^3} \sum_{k=1}^{n} (3k^2 - 2k)$$

$$= \frac{1}{n^3} \left( 3\sum_{k=1}^{n} k^2 - 2\sum_{k=1}^{n} k \right)$$

Rumus:
- $\sum_{k=1}^{n} k = \frac{n(n+1)}{2}$
- $\sum_{k=1}^{n} k^2 = \frac{n(n+1)(2n+1)}{6}$

Substitusi:
$$= \frac{1}{n^3} \left[ 3 \cdot \frac{n(n+1)(2n+1)}{6} - 2 \cdot \frac{n(n+1)}{2} \right]$$

$$= \frac{1}{n^3} \left[ \frac{n(n+1)(2n+1)}{2} - n(n+1) \right]$$

$$= \frac{1}{n^3} \cdot n(n+1) \left[ \frac{2n+1}{2} - 1 \right]$$

$$= \frac{n(n+1)}{n^3} \left[ \frac{2n+1 - 2}{2} \right]$$

$$= \frac{n(n+1)}{n^3} \cdot \frac{2n-1}{2}$$

$$= \frac{(n+1)(2n-1)}{2n^2} = \boxed{\frac{2n^2 + n - 1}{2n^2}} \text{ atau } \boxed{1 + \frac{1}{2n} - \frac{1}{2n^2}}$$

---

### Soal 5
**Hitunglah nilai dari**

$$\sum_{k=1}^{20} (2k^2 - 3k + 1)$$

$$= 2\sum_{k=1}^{20} k^2 - 3\sum_{k=1}^{20} k + \sum_{k=1}^{20} 1$$

Rumus:
- $\sum_{k=1}^{20} k = \frac{20(21)}{2} = 210$
- $\sum_{k=1}^{20} k^2 = \frac{20(21)(41)}{6} = 2870$
- $\sum_{k=1}^{20} 1 = 20$

Substitusi:
$$= 2(2870) - 3(210) + 20$$
$$= 5740 - 630 + 20$$
$$= \boxed{5130}$$

---

## BAGIAN B: LUAS DAERAH DENGAN METODE TRAPESIUM

### Soal 6
**Daerah dibatasi oleh kurva $f(x) = 4 - x^2$, sumbu-x, dan sumbu-y pada interval [0,2]. Dengan membagi daerah menjadi 4 partisi.**

**Diberikan:** $a = 0, b = 2, n = 4$

**(1) $\Delta x = \frac{b-a}{n} = \frac{2-0}{4} = \frac{1}{2} = 0.5$**

**(2) $x_i = a + i\Delta x$:**
- $x_0 = 0 + 0(0.5) = 0$
- $x_1 = 0 + 1(0.5) = 0.5$
- $x_2 = 0 + 2(0.5) = 1.0$
- $x_3 = 0 + 3(0.5) = 1.5$
- $x_4 = 0 + 4(0.5) = 2.0$

Jadi: $x_0, x_1, x_2, x_3, x_4 = \boxed{0,\ 0.5,\ 1.0,\ 1.5,\ 2.0}$

**(3) $f(x) = 4 - x^2$:**
- $f(x_0) = f(0) = 4 - 0 = 4$
- $f(x_1) = f(0.5) = 4 - 0.25 = 3.75$
- $f(x_2) = f(1.0) = 4 - 1 = 3$
- $f(x_3) = f(1.5) = 4 - 2.25 = 1.75$
- $f(x_4) = f(2.0) = 4 - 4 = 0$

Jadi: $f(x_0), f(x_1), f(x_2), f(x_3), f(x_4) = \boxed{4,\ 3.75,\ 3,\ 1.75,\ 0}$

**(4) Substitusi ke rumus trapesium:**

$$\int_0^2 f(x) dx \approx \frac{\Delta x}{2} [f(x_0) + 2f(x_1) + 2f(x_2) + 2f(x_3) + f(x_4)]$$

$$= \frac{0.5}{2} [4 + 2(3.75) + 2(3) + 2(1.75) + 0]$$

$$= 0.25 [4 + 7.5 + 6 + 3.5 + 0]$$

$$= 0.25 [21] = \boxed{5.25}$$

**(5) Luas sebenarnya = $\frac{16}{3} \approx 5.333\ldots$**

Galat = $|Luas\ sebenarnya - Taksiran| = \left|\frac{16}{3} - 5.25\right| = \left|5.333\ldots - 5.25\right| = \boxed{0.083\ldots = \frac{1}{12}}$

---

### Soal 7
**Taksirlah nilai integral berikut dengan metode trapesium menggunakan n = 3 dan n = 6, lalu tentukan taksiran mana yang lebih akurat.**

$$\int_0^3 (x^2 + 1) dx$$

**Luas sebenarnya:**
$$\int_0^3 (x^2 + 1) dx = \left[\frac{x^3}{3} + x\right]_0^3 = \frac{27}{3} + 3 = 9 + 3 = 12$$

---

#### Untuk n = 3:
$a = 0, b = 3, n = 3, \Delta x = \frac{3-0}{3} = 1$

Titik-titik: $x_0 = 0, x_1 = 1, x_2 = 2, x_3 = 3$

$f(x) = x^2 + 1$:
- $f(0) = 1$
- $f(1) = 2$
- $f(2) = 5$
- $f(3) = 10$

Trapesium:
$$\approx \frac{1}{2} [1 + 2(2) + 2(5) + 10] = 0.5 [1 + 4 + 10 + 10] = 0.5 [25] = \boxed{12.5}$$

---

#### Untuk n = 6:
$a = 0, b = 3, n = 6, \Delta x = \frac{3-0}{6} = 0.5$

Titik-titik: $x_0 = 0, x_1 = 0.5, x_2 = 1.0, x_3 = 1.5, x_4 = 2.0, x_5 = 2.5, x_6 = 3.0$

$f(x) = x^2 + 1$:
- $f(0) = 1$
- $f(0.5) = 1.25$
- $f(1.0) = 2$
- $f(1.5) = 3.25$
- $f(2.0) = 5$
- $f(2.5) = 7.25$
- $f(3.0) = 10$

Trapesium:
$$\approx \frac{0.5}{2} [1 + 2(1.25) + 2(2) + 2(3.25) + 2(5) + 2(7.25) + 10]$$

$$= 0.25 [1 + 2.5 + 4 + 6.5 + 10 + 14.5 + 10]$$

$$= 0.25 [48.5] = \boxed{12.125}$$

---

**Kesimpulan:**
- n = 3: taksiran = 12.5, galat = |12 - 12.5| = 0.5
- n = 6: taksiran = 12.125, galat = |12 - 12.125| = 0.125

**Taksiran dengan n = 6 lebih akurat** karena semakin banyak partisi (semakin kecil $\Delta x$), semakin dekat taksiran trapesium dengan nilai sebenarnya.

---

## BAGIAN C: INTEGRAL FUNGSI DASAR

### Soal 8
$$\int (6x^2 - 4x + 5) dx$$

$$= 6\int x^2 dx - 4\int x dx + 5\int dx$$

$$= 6\left(\frac{x^3}{3}\right) - 4\left(\frac{x^2}{2}\right) + 5x + C$$

$$= \boxed{2x^3 - 2x^2 + 5x + C}$$

---

### Soal 9
$$\int_0^2 (4 - x^2) dx$$

$$= \left[4x - \frac{x^3}{3}\right]_0^2$$

$$= \left(4(2) - \frac{2^3}{3}\right) - (0)$$

$$= 8 - \frac{8}{3} = \frac{24 - 8}{3} = \boxed{\frac{16}{3}}$$

**Perbandingan dengan Soal 6:**
- Soal 6 (Metode Trapesium n=4): taksiran = 5.25 = $\frac{21}{4} = 5.25$
- Soal 9 (Integral Tentu): hasil = $\frac{16}{3} \approx 5.333\ldots$

**Mengapa tandanya berbeda?**
Tanda **tidak berbeda** — keduanya **positif**. Keduanya menghitung luas daerah yang sama (di atas sumbu-x pada interval [0,2]). 

Perbedaan hanya pada **nilai**:
- Integral tentu memberikan nilai **eksak** ($\frac{16}{3}$)
- Metode trapesium memberikan **taksiran/nilai pendekatan** (5.25)

Jika soal memaksudkan "mengapa **nilainya** berbeda": karena metode trapesium adalah metode numerik pendekatan, sedangkan integral tentu memberikan nilai eksak analitik.

---

### Soal 10
$$\int (3\sqrt{x} - x^2) dx = \int (3x^{1/2} - x^2) dx$$

$$= 3\int x^{1/2} dx - \int x^2 dx$$

$$= 3\left(\frac{x^{3/2}}{3/2}\right) - \frac{x^3}{3} + C$$

$$= 3\left(\frac{2}{3}x^{3/2}\right) - \frac{x^3}{3} + C$$

$$= \boxed{2x^{3/2} - \frac{x^3}{3} + C} \text{ atau } \boxed{2\sqrt{x^3} - \frac{x^3}{3} + C}$$

---

### Soal 11
$$\int \frac{x^3 + 2x}{x} dx = \int \left(\frac{x^3}{x} + \frac{2x}{x}\right) dx = \int (x^2 + 2) dx$$

$$= \int x^2 dx + \int 2 dx$$

$$= \frac{x^3}{3} + 2x + C$$

$$= \boxed{\frac{x^3}{3} + 2x + C}$$

---

### Soal 12
$$\int (2x + 1)^2 dx$$

Ekspansi: $(2x + 1)^2 = 4x^2 + 4x + 1$

$$= \int (4x^2 + 4x + 1) dx$$

$$= 4\int x^2 dx + 4\int x dx + \int dx$$

$$= 4\left(\frac{x^3}{3}\right) + 4\left(\frac{x^2}{2}\right) + x + C$$

$$= \boxed{\frac{4}{3}x^3 + 2x^2 + x + C}$$

---

### Soal 13
$$\int (\sin x + 3\cos x) dx$$

$$= \int \sin x dx + 3\int \cos x dx$$

$$= -\cos x + 3\sin x + C$$

$$= \boxed{3\sin x - \cos x + C}$$

---

### Soal 14
Soal 14 tidak ada di daftar (melompat dari 13 ke 15)

---

### Soal 15
$$\int_0^{\pi/2} \cos x dx$$

$$= [\sin x]_0^{\pi/2}$$

$$= \sin(\pi/2) - \sin(0) = 1 - 0 = \boxed{1}$$

---

### Soal 16
$$\int_{-1}^2 (3x^2 - 2x + 1) dx$$

$$= \left[3\left(\frac{x^3}{3}\right) - 2\left(\frac{x^2}{2}\right) + x\right]_{-1}^2$$

$$= \left[x^3 - x^2 + x\right]_{-1}^2$$

Hitung di batas atas (x=2):
$$(2)^3 - (2)^2 + 2 = 8 - 4 + 2 = 6$$

Hitung di batas bawah (x=-1):
$$(-1)^3 - (-1)^2 + (-1) = -1 - 1 - 1 = -3$$

Hasil:
$$6 - (-3) = 6 + 3 = \boxed{9}$$

---

## RINGKASAN JAWABAN

| Soal | Jawaban |
|------|---------|
| 1 | 5100 |
| 2 | $\frac{2}{n} + \frac{5}{n} + \frac{8}{n} + \cdots + \frac{3n-1}{n}$ |
| 3 | $\sum_{i=1}^{n} \left[ \left(\frac{i}{n}\right)^3 + i \right]$ |
| 4 | $\frac{2n^2 + n - 1}{2n^2}$ |
| 5 | 5130 |
| 6(1) | $\Delta x = 0.5$ |
| 6(2) | $x_0=0, x_1=0.5, x_2=1, x_3=1.5, x_4=2$ |
| 6(3) | $f(x_0)=4, f(x_1)=3.75, f(x_2)=3, f(x_3)=1.75, f(x_4)=0$ |
| 6(4) | 5.25 |
| 6(5) | $\frac{1}{12} \approx 0.0833$ |
| 7 (n=3) | 12.5 (galat 0.5) |
| 7 (n=6) | 12.125 (galat 0.125) — **lebih akurat** |
| 8 | $2x^3 - 2x^2 + 5x + C$ |
| 9 | $\frac{16}{3}$ |
| 10 | $2x^{3/2} - \frac{x^3}{3} + C$ |
| 11 | $\frac{x^3}{3} + 2x + C$ |
| 12 | $\frac{4}{3}x^3 + 2x^2 + x + C$ |
| 13 | $3\sin x - \cos x + C$ |
| 15 | 1 |
| 16 | 9 |
