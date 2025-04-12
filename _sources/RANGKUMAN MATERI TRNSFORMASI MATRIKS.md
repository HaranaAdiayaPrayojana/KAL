---
title: RANGKUMAN MATERI TRNSFORMASI MATRIKS

---

# RANGKUMAN MATERI TRNSFORMASI MATRIKS

Bab ini akan mempelajari tentang transformasi matriks, yaitu fungsi yang memetakan vektor ke vektor lain menggunakan perkalian matriks. Transformasi ini memiliki aplikasi luas dalam matematika, fisika, dan teknik.

## Transformasi Matriks

Sebuah transformasi matriks adalah fungsi $T:\mathbb{R}^3 \rightarrow \mathbb{R}^2$ yang didefinisikan oleh; $$T(\vec{x})=A\vec{x}$$

dimana A adalah berukuran $m\times n$ dan $\vec{x}$ adalah vektor di $\mathbb{R}^n$.

Transformasi matriks bersifat linear, yang berarti memenuhi dua sifat berikut:
$$1. T(\vec{u}+\vec{v})=T(\vec{u})+T(\vec{v})$$

$$2. T(c\vec{u})= cT(\vec{u}), untuk\space skalar\space c.$$

## Matriks - Perkalian Vektor

Untuk menyederhanakan pembahasan, dan memudahkan kita untuk menggambarkan apa yang sedang terjadi, kita akan membatasi diri (untuk saat ini) pada vektor di $\mathbb{R}^2$. Kita ingin memvisualisasikan hasil perkalian vektor dengan matriks. Untuk mengalikan vektor 2D dengan matriks dan mendapatkan kembali vektor 2D, matriks kita harus berupa matriks persegi 2 × 2.

Misalkan A adalah suatu matriks, dan $\vec{x},\space \vec{y},\space dan\space \vec{z}\space$ adalah vektor seperti yang diberikan di bawah ini.

$$
A=
\left[
\begin{array}{cc}
1 & 4\\
2 & 3 
\end{array}
\right],\space
\vec{x}=
\left[
\begin{array}{cc}
1 \\
1 
\end{array}
\right],\space
\vec{y}=
\left[
\begin{array}{cc}
-1 \\
1 
\end{array}
\right],\space
\vec{z}=
\left[
\begin{array}{cc}
3 \\
-1 
\end{array}
\right]\space
$$

Grafik  $\vec{x},\space \vec{y},\space dan\space \vec{z}\space$, serta $A\vec{x},\space A\vec{y},\space dan\space A\vec{z}\space$

Ada beberapa hal yang perlu diperhatikan. Ketika setiap vektor dikalikan dengan A, hasilnya adalah vektor dengan panjang yang berbeda (dalam contoh ini, selalu lebih panjang), dan dalam dua kasus (untuk $\vec{y}$ dan \vz), vektor yang dihasilkan menunjuk ke arah yang berbeda.

contoh Menggabungkan penjumlahan dan perkalian martiks:

$$
A=
\left[
\begin{array}{cc}
1 & 1\\
1 & 2 
\end{array}
\right],\space
\vec{x}=
\left[
\begin{array}{cc}
2 \\
1 
\end{array}
\right],\space
\vec{y}=
\left[
\begin{array}{cc}
-1 \\
1 
\end{array}
\right],\space
$$

$$
\vec{x}+\vec{y}=
\left[
\begin{array}{cc}
1\\
2 
\end{array}
\right]; \space
A\vec{x}=
\left[
\begin{array}{cc}
3 \\
4 
\end{array}
\right],\space
A\vec{y}=
\left[
\begin{array}{cc}
0 \\
1 
\end{array}
\right],\space
A(\vec{x}+\vec{y})=
\left[
\begin{array}{cc}
3 \\
5 
\end{array}
\right]
$$

## Transformasi Bidang Cartesian
Transformasi Bidang Cartesian adalah operasi matematis yang mengubah posisi, bentuk, atau orientasi objek dalam sistem koordinat Cartesian dua dimensi ($\mathbb{R}^2$) atau tiga dimensi ($\mathbb{R}^3$) menggunakan matriks transformasi. Transformasi ini bersifat linear dan mempertahankan garis lurus serta origin (titik pusat koordinat).

### Jenis Jenis Transformasi Bidang Cartesian
#### 1. Translasi (Pergeseran)
- memindahkan objek sejauh vektor tertentu $\vec{v}=[a,b]$ dengan menggunakan rumus $T(\vec{x})=\vec{x}+\vec{v}$
-contoh:
$$
T
\left(
\left[
\begin{array}{cc}
x\\
y 
\end{array}
\right]
\right)= \space
\left[
\begin{array}{cc}
x+3 \\
y-3 
\end{array}
\right] \space \space (Geser 2 satuan kanan, 3 satuan bawah)
$$

#### 2. Rotasi (Perputaran)
memutar objek dengan sudut θ terhadap origin. contoh matriks rotasi 2D: 

$$
R_θ = 
\left[
\begin{array}{cc}
cosθ&-sinθ \\
sinθ&cosθ 
\end{array}
\right]
$$

contoh rotasi $90^\circ$ berlawanan jarum jam:

$$
R_θ = 
\left[
\begin{array}{cc}
0&-1 \\
1&0 
\end{array}
\right],\space Hasil\space R_{90^\circ}
\left[
\begin{array}{cc}
1 \\
0 
\end{array}
\right] =
\left[
\begin{array}{cc}
0 \\
1 
\end{array}
\right]
$$

#### 3. Penskalaan(Scaling):
mengubah ukuran objek dengan faktor skala $s_x$ (sumbu x) dan $s_y$ (sumbu y). Contoh Matriks Penskalaan:

$$
S = 
\left[
\begin{array}{cc}
s_x&0 \\
0&s_y 
\end{array}
\right]
$$

contoh penskalaan 2 kali di sumbu x:

$$
S
\left[
\begin{array}{cc}
3 \\
4 
\end{array}
\right] =
\left[
\begin{array}{cc}
6 \\
4 
\end{array}
\right]
$$

#### 4. Refleksi(Pencerminan)
Mencerminkan objeck terhadap sumbu garis. contoh Matriks Refleksi:
- Terhadap sumbu x : $\left[\begin{array}{cc}1&0\\0&-1\end{array}\right]$
- Terhadap sumbu y=x : $\left[\begin{array}{cc}1&0\\0&-1\end{array}\right]$

#### 5. Shear (Pergeseran Geser)
Menggeser objek sepanjang sumbu tertentu. Contoh Matriks Shear:
$$Shear horizontal:\space \left[\begin{array}{cc}1&k\\0&1\end{array}\right]$$

### Sifat Transformasi Linear
- Mempertahankan Garis Lurus: Garis tetap lurus setelah transformasi.
- Origin Tidak Berubah: $T(\vec{0})=\vec{0}$ (kecuali translasi).
- Kombinasi Transformasi: Dapat dikomposisikan menggunakan perkalian matriks.
Contoh: Rotasi + Penskalaan = $R_θ\times S$.

## 5.1.4 Exercises

latihan kelompok. Diberikan matriks A. Gambarlah $\vec{x},\space \vec{y},\space A\vec{x},\space dan\space A\vec{y}$ pada sumbu Cartesian yang sama, dimana;
$$\vec{x}=\left[\begin{array}{cc}1\\1\end{array}\right]\space and\space\vec{y}=\left[\begin{array}{cc}-1\\2\end{array}\right]$$

$1.\space A=\left[\begin{array}{cc}1&-1\\2&3\end{array}\right]$

Menghitung $A\vec{x}$:

$$
A\vec{x}=\left[\begin{array}{cc}1&-1\\2&3\end{array}\right]
\left[\begin{array}{cc}1\\1\end{array}\right]=
\left[\begin{array}{cc}1(1)+(-1)(1)\\2(1)+3(1)\end{array}\right]=
\left[\begin{array}{cc}0\\5\end{array}\right]
$$

Menghitung $A\vec{y}$:

$$
A\vec{x}=\left[\begin{array}{cc}1&-1\\2&3\end{array}\right]
\left[\begin{array}{cc}-1\\2\end{array}\right]=
\left[\begin{array}{cc}1(-1)+(-1)(2)\\2(1)+3(1)\end{array}\right]=
\left[\begin{array}{cc}1-2\\-2+6\end{array}\right]=
\left[\begin{array}{cc}-3\\4\end{array}\right]
$$

kesimpulan no 1:
$$
\vec{x}=\left[\begin{array}{cc}1\\1\end{array}\right]
\vec{y}=\left[\begin{array}{cc}-1\\2\end{array}\right]
A\vec{x}=\left[\begin{array}{cc}0\\5\end{array}\right]
A\vec{y}=\left[\begin{array}{cc}-3\\4\end{array}\right]
$$

gambar sket:
![1](https://hackmd.io/_uploads/B1Z0EdDA1g.png)



$2.\space A=\left[\begin{array}{cc}2&0\\-1&3\end{array}\right]$

Menghitung $A\vec{x}$:

$$
A\vec{x}=\left[\begin{array}{cc}2&0\\-1&3\end{array}\right]
\left[\begin{array}{cc}1\\1\end{array}\right]=
\left[\begin{array}{cc}2(1)+0(1)\\-1(1)+3(1)\end{array}\right]=
\left[\begin{array}{cc}2\\2\end{array}\right]
$$

Menghitung $A\vec{y}$:

$$
A\vec{y}=\left[\begin{array}{cc}2&0\\-1&3\end{array}\right]
\left[\begin{array}{cc}-1\\2\end{array}\right]=
\left[\begin{array}{cc}2(-1)+0(2)\\-1(-1)+3(2)\end{array}\right]=
\left[\begin{array}{cc}-2\\7\end{array}\right]
$$

kesimpulan no 2:

$$
\vec{x}=\left[\begin{array}{cc}1\\1\end{array}\right]
\vec{y}=\left[\begin{array}{cc}-1\\2\end{array}\right]
A\vec{x}=\left[\begin{array}{cc}2\\2\end{array}\right]
A\vec{y}=\left[\begin{array}{cc}-2\\7\end{array}\right]
$$

gambar sket:

![2](https://hackmd.io/_uploads/rkyU8dP01l.png)


$3.\space A=\left[\begin{array}{cc}1&1\\1&1\end{array}\right]$

Menghitung $A\vec{x}$:

$$
A\vec{x}=\left[\begin{array}{cc}1&1\\1&1\end{array}\right]
\left[\begin{array}{cc}1\\1\end{array}\right]=
\left[\begin{array}{cc}1(1)+(1)(1)\\1(1)+1(1)\end{array}\right]=
\left[\begin{array}{cc}2\\2\end{array}\right]
$$

Menghitung $A\vec{y}$:

$$
A\vec{y}=\left[\begin{array}{cc}1&1\\1&1\end{array}\right]
\left[\begin{array}{cc}-1\\2\end{array}\right]=
\left[\begin{array}{cc}1(-1)+1(2)\\1(-1)+1(2)\end{array}\right]=
\left[\begin{array}{cc}1\\1\end{array}\right]
$$

Kesimpulan no 3:

$$
\vec{x}=\left[\begin{array}{cc}1\\1\end{array}\right]
\vec{y}=\left[\begin{array}{cc}-1\\2\end{array}\right]
A\vec{x}=\left[\begin{array}{cc}2\\2\end{array}\right]
A\vec{y}=\left[\begin{array}{cc}1\\1\end{array}\right]
$$

Gambar sket:

![3](https://hackmd.io/_uploads/Bkia8_PAkg.png)



$4.\space A=\left[\begin{array}{cc}1&2\\-1&3\end{array}\right]$

Menghitung $A\vec{x}$:

$$
A\vec{x}=\left[\begin{array}{cc}1&2\\-1&3\end{array}\right]
\left[\begin{array}{cc}1\\1\end{array}\right]=
\left[\begin{array}{cc}1(1)+2(1)\\-1(1)+3(1)\end{array}\right]=
\left[\begin{array}{cc}3\\2\end{array}\right]
$$

Menghitung $A\vec{y}$:

$$
A\vec{y}=\left[\begin{array}{cc}1&2\\-1&3\end{array}\right]
\left[\begin{array}{cc}-1\\2\end{array}\right]=
\left[\begin{array}{cc}1(-1)+2(2)\\1(-1)+3(2)\end{array}\right]=
\left[\begin{array}{cc}3\\7\end{array}\right]
$$

Kesimpulan no 4:



$$
\vec{x}=\left[\begin{array}{cc}1\\1\end{array}\right]
\vec{y}=\left[\begin{array}{cc}-1\\2\end{array}\right]
A\vec{x}=\left[\begin{array}{cc}3\\2\end{array}\right]
A\vec{y}=\left[\begin{array}{cc}3\\7\end{array}\right]
$$

Gambar Graf

![4](https://hackmd.io/_uploads/HJrNGtvAkl.png)
Latihan Kelompok: Sketsa unit persegi yang ditransformasikan diberikan. Temukan matriks A yang melakukan transformasi ini.

5. ![5](https://hackmd.io/_uploads/rkLjXYwAkl.png)

Titik asal=(0,0), lalu titik persegi Vektor awal $\vec{x}=\left[\begin{array}{cc}1\\0\end{array}\right]$, titik segitiga vektor kedua $\vec{y}=\left[\begin{array}{cc}0\\1\end{array}\right]$, titik bulat hasil penjumlahan dua vaktor= $\left[\begin{array}{cc}1\\1\end{array}\right]$

- Persegi berada di (0.5,1) hasil dari $A\left[\begin{array}{cc}1\\0\end{array}\right]$
- Segitiga berada di (1,2) hasil dari $A\left[\begin{array}{cc}0\\1\end{array}\right]$
- Buletan berada di (1.5,3) hasil dari $A\left[\begin{array}{cc}1\\1\end{array}\right]$

maka
$$A=\left[\begin{array}{cc}0.5&1\\1&2\end{array}\right]$$

6. ![6](https://hackmd.io/_uploads/H1S5IFwCJx.png)

Titik asal=(0,0), lalu titik persegi Vektor awal $\vec{x}=\left[\begin{array}{cc}1\\0\end{array}\right]$, titik segitiga vektor kedua $\vec{y}=\left[\begin{array}{cc}0\\1\end{array}\right]$, titik bulat hasil penjumlahan dua vaktor= $\left[\begin{array}{cc}1\\1\end{array}\right]$

- Persegi berada di (-1,1) hasil dari $A\left[\begin{array}{cc}1\\0\end{array}\right]$
- Segitiga berada di (1,1) hasil dari $A\left[\begin{array}{cc}0\\1\end{array}\right]$
- Buletan berada di (0,2) hasil dari $A\left[\begin{array}{cc}1\\1\end{array}\right]$

maka
$$A=\left[\begin{array}{cc}-1&1\\1&1\end{array}\right]$$