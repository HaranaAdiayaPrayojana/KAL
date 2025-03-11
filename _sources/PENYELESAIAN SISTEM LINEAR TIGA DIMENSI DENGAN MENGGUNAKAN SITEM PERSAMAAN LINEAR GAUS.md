---
title: PENYELESAIAN SISTEM LINEAR TIGA DIMENSI DENGAN MENGGUNAKAN SITEM PERSAMAAN LINEAR GAUS

---

# PENYELESAIAN SISTEM LINEAR TIGA DIMENSI DENGAN MENGGUNAKAN SITEM PERSAMAAN LINEAR GAUS

## SISTEM PERSAMAAN LINIER TIGA DIMENSI DENGAN SATU SOLUSI

Sistem persamaan linier tiga dimensi terdiri dari tiga persamaan dengan tiga variabel, umumnya x, y, dan z. Jika sistem tersebut memiliki satu solusi artinya ketiga persamaan tersebut saling berpotongan pada satu titik tunggal di ruang tiga dimensi. Berikut bentuk umum sistem persamaan linear tiga dimensi:

- a11x+a12y+a13z=b1
- a21x+a22y+a23z=b2
- a31x+a32y+a33z=b3

Dimana aij adalah koefisien dari variabel x, y, dan z. bi adalah konstanta di ruas kanan persamaan. Contoh:

$$
\begin{aligned}
x + 2y + 3z &= 10 \\
2x - y + z &= 5 \\
3x + y - 2z &= 1
\end{aligned}
$$

Sistem persamaan linear tiga dimensi dapat direpresentasikan dalam bentuk metriks augmented [A|B], di mana A adalah matriks koefisien dari variabel, dan B adalah matriks konstanta. contoh

$$
\left[
\begin{array}{ccc|c}
1 & 2 & 3 & 10 \\
2 & -1 & 1 & 5 \\
3 & 1 & -2 & 1
\end{array}
\right]
$$

Menentukan Titik potong dengan eliminasi Gauss

$$
\left[
\begin{array}{ccc|c}
1 & 2 & 3 & 10 \\
2 & -1 & 1 & 5 \\
3 & 1 & -2 & 1
\end{array}
\right]
$$

Eliminasi Kolom Kedua
- R2 -> R2 - 2R1
- R3 -> R3 - 3R1

$$
\left[
\begin{array}{ccc|c}
1 & 2 & 3 & 10 \\
0 & -5 & -5 & -15 \\
0 & -5 & -11 & -29
\end{array}
\right]
$$

Eliminasi Kolom Ketiga
- R3 -> R3 - R2

$$
\left[
\begin{array}{ccc|c}
1 & 2 & 3 & 10 \\
0 & -5 & -5 & -15 \\
0 & 0 & -6 & -14
\end{array}
\right]
$$

Substitusikan:

$$
-6z = 14 \Rightarrow z = \frac{14}{6} = \frac{7}{3}
$$
$$
-5y-5x \frac{7}{3}=-15
$$
$$-5y -\frac{35}{3}=-15$$
$$-5y=-15+\frac{35}{3}$$
$$-5y=-45+\frac{35}{3}=-\frac{10}{3}$$
$$y=\frac{2}{3}$$

$$x+2x\frac{2}{3}+3x\frac{7}{3}=10$$
$$x+\frac{4}{3}+7=10$$
$$x+\frac{4}{3}=3$$
$$=3-\frac{4}{3}=\frac{9}{3}-\frac{4}{3}=\frac{5}{3}$$

<iframe src="https://www.geogebra.org/3d/bdjtbh5h?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

## Sistem Persamaan Linear Tiga Dimensi dengan Solusi Tak Hingga

Sistem Persamaan Linear 3 Dimensi dengan solusi tak hingga terjadi ketika persamaan persamaan tersebut saling bergantung secara linear, sehingga sistem memiliki lebih dari satu solusi. Solusi ini biasanya dinyatakan dalam bentuk parameter. Bentuk umum sistem persamaan linear tiga dimensi dapat ditulis sebagai:

- a11x+a12y+a13z=b1
- a21x+a22y+a23z=b2
- a31x+a32y+a33z=b3

Di mana:
- aij adalah koefisien dari variabel x, y, dan z.
- bi adalah konstanta di ruas kanan persamaan.

contoh persamaan sistem:

$$
\begin{aligned}
x + y + z &= 4 \\
2x - 2y + 2z &= 8 \\
3x + 3y + 3z &= 12
\end{aligned}
$$


1. Penyelesaian dengan Eliminasi Gauss
    Eliminasi Kolom pertama
    - R2->R2-2R1
    - R3->R3-3R1
    
$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 4 \\
2 & 2 & 2 & 8 \\
3 & 3 & 3 & 12
\end{array}
\right]
$$
    
$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 4 \\
0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0
\end{array}
\right] 
$$
    Baris Kedua dan ketiga menjadi baris nol(0=0), yang berarti persamaan ini bergantung satu sama lain dan g=hanya memberi dua persamaan yang sama. Karena hanya memiliki satu persamaan independen dengan tiga variabel, maka sistem memiliki solusi tak hingga.

2. Penyelesaian dalam Bentuk Parameter

    - Persamaan Pertama:
    $$x+y+z=4$$
    
    - Mengubah z menjadi t karena z adalah parameter bebas:
    $$x+y=4-t$$
    
    - mengubah parameter y menjadi s:
   $$x=4-s-t$$
    
    - Sehingga solusi dapat ditulis sebagai:
    $$(x, y, z)=(4-s-t,s,t)$$

    dengan s dan t bebas dalam bilangan real. Karena ada dua parameter bebas (s,t), solusi sistem ini tak hingga banyaknya. Secara geometris, tiga bidang ini berpotongan sepanjang satu garis lurus di ruang tiga dimensi.
    
<iframe src="https://www.geogebra.org/3d/xv2tcdff?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

## Sistem Persamaan Linear Tiga Dimensi Tanpa Solusi

 Sistem persamaan linear tiga variabel tanpa solusi terjadi ketika tiga bidang dalam ruang tiga dimensi tidak memiliki titik potong yang sama. Hal ini bisa terjadi dalam beberapa kasus seperti:
 - Tiga Bidang sejajar tetapi tidak saling memotong
 -  Dua bidang sejajar dan bidang ketiga memotong salah satunya.
 -  Setiap dua bidang berpotongan tetapu ketiganya tidak bertemu di satu titik yang sama
 
 Bentuk umum sistem persamaan linear tiga dimensi dapat ditulis sebagai:

- a11x+a12y+a13z=b1
- a21x+a22y+a23z=b2
- a31x+a32y+a33z=b3

Di mana:
- aij adalah koefisien dari variabel x, y, dan z.
- bi adalah konstanta di ruas kanan persamaan.

Contoh Persamaan:

$$x+y+z=4$$
$$x+y+z=5$$
$$ x+y+z=6$$

1. Penyelesaian dengan Eliminasi Gauss

Eliminasi Baris kedua dan beris ketiga dengan baris pertama:
R2->R2-R1
R3->R3-R1

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 4 \\
1 & 1 & 1 & 5 \\
1 & 1 & 1 & 6
\end{array}
\right] 
$$

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 4 \\
0 & 0 & 0 & 1 \\
0 & 0 & 0 & 2
\end{array}
\right] 
$$

Karena terdapat persamaan yang bertentangan (0 tidak bisa sama dengan 1 atau 2), maka persamaan ini tidak memiliki solusi. Hal ini dikarenakan tiga bidangnya sejajar tetapu berbeda posisi dan tidak akan pernah berpotongan dalam ruang tiga dimensi.

<iframe src="https://www.geogebra.org/3d/qvwkhcyh?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>