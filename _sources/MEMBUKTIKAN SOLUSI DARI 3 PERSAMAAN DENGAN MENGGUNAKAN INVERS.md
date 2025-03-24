---
title: MEMBUKTIKAN SOLUSI DARI 3 PERSAMAAN DENGAN MENGGUNAKAN INVERS

---

# MEMBUKTIKAN SOLUSI DARI 3 PERSAMAAN DENGAN MENGGUNAKAN INVERS 1 0 0

## Persamaan:
$$4x1-x2+x3=4$$
$$x1+3x2-2x3=1$$
$$2x1+x2+x3=2$$

## Solusi

Membuat Matriks A dan Matriks Identitas I:


$$
A=
\left[
\begin{array}{ccc|ccc}
4 & -1 & 1 \\
1 & 3 & -2 \\
2 & 1 & 1
\end{array}
\right]
$$

Matriks Identitas I adalah:

$$
I=
\left[
\begin{array}{ccc|ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{array}
\right
]
$$

Gabungkan Matriks A dan Matriks Identitas I Menjadi [A|I]:

$$
[A|i]=
\left[
\begin{array}{ccc|ccc}
4&-1&1&1&0&0\\
1&3&-2&0&1&0\\
2&1&1&0&0&1
\end{array}
\right
]
$$

Lakukan Eliminasi Untuk mengubah Matriks A menjadi Matriks Identitas I

Eliminasi a11 menjadi 1:

$$
[A|i]=
\left[
\begin{array}{ccc|ccc}
1&-\frac{1}{4}&\frac{1}{4}&\frac{1}{4}&0&0\\
1&3&-2&0&1&0\\
2&1&1&0&0&1
\end{array}
\right
]
$$

buat elemen a21 dan a31 menjadi 0

$$R2=R2-R1$$

$$A21=1-1=0$$

$$A22=3 - (- \frac{1}{4} ) -3 + \frac{1}{4}=\frac{13}{4}$$

$$A23=-2-\frac{1}{4}=-\frac{9}{4}$$

---------

$$R3=R3-2R1$$

$$A31=2-2.1=0$$


$$A32=1-2.(-\frac{1}{4})-1+\frac{1}{2}=\frac{3}{2}$$

$$A33=1-2.\frac{1}{4}=1-\frac{1}{2}=\frac{1}{2}$$

$$
[A|I]=
\left[
\begin{array}{ccc|ccc}
1&-\frac{1}{4}&\frac{1}{4}&\frac{1}{4}&0&0\\
0&-\frac{13}{4}&-\frac{9}{4}&-\frac{1}{4}&1&0\\
0&\frac{3}{2}&\frac{1}{2}&-\frac{1}{2}&0&1
\end{array}
\right
]
$$

Membuat elemen a22 menjadi 1:

$$R2=\frac{4}{13}R2

$$
[A|I]=
\left[
\begin{array}{ccc|ccc}
1&-\frac{1}{4}&\frac{1}{4}&\frac{1}{4}&0&0\\
0&1&-\frac{9}{13}&-\frac{1}{13}&\frac{4}{13}&0\\
0&\frac{3}{2}&\frac{1}{2}&-\frac{1}{2}&0&1
\end{array}
\right
]
$$

Membuat Elemen a12 dan a32 menjadi 0

$$R1=R1+\frac{1}{4} R2$$
$$R3=R3-\frac{3}{2} R2$$
$$
[A|I]=
\left[
\begin{array}{ccc|ccc}
1&0&-\frac{1}{13}&\frac{3}{13}&\frac{1}{13}&0\\
0&1&-\frac{9}{13}&-\frac{1}{13}&\frac{4}{13}&0\\
0&0&\frac{20}{13}&-\frac{10}{13}&-\frac{6}{13}&1
\end{array}
\right
]
$$

Membuat Elemen A33 menjadi 1 :

$$R3=\frac{13}{20}R3$$
$$
[A|I]=
\left[
\begin{array}{ccc|ccc}
1&0&-\frac{1}{13}&\frac{3}{13}&\frac{1}{13}&0\\
0&1&-\frac{9}{13}&-\frac{1}{13}&\frac{4}{13}&0\\
0&0&1&-\frac{1}{2}&-\frac{3}{10}&\frac{13}{20}
\end{array}
\right
]
$$

Membuat elemen A13 dan A23 menjadi 0

$$R1=R1-\frac{1}{13}R3$$
$$R2=R2+\frac{9}{13}R3$$
$$
[A|I]=
\left[
\begin{array}{ccc|ccc}
1&0&0&\frac{1}{4}&\frac{1}{4}&-\frac{1}{20}\\
0&1&0&-\frac{1}{4}&\frac{1}{4}&\frac{9}{20}\\
0&0&1&-\frac{1}{2}&-\frac{3}{10}&\frac{13}{20}
\end{array}
\right
]
$$

Setelah eliminasi Gauss, matriks A telah Diubah menjadi matriks I dan matriks I telah menjadi invers matriks $A (A^{-1})$

$$
A^{-1}=
\left[
\begin{array}{ccc|ccc}
1&0&0&\frac{1}{4}&\frac{1}{4}&-\frac{1}{20}\\
0&1&0&-\frac{1}{4}&\frac{1}{4}&\frac{9}{20}\\
0&0&1&-\frac{1}{2}&-\frac{3}{10}&\frac{13}{20}
\end{array}
\right
]
$$

untuk memverifikasi bahwa $A^{-1}$ adalah invers dari A, kalikan A dengan $A^{-1}$ dan Pastikan hasilnya adalah matriks identitas I
$$A \times A^{-1}$$

yang akan menghasilkan matriks identitas:

$$
I=
\left[
\begin{array}{ccc|ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{array}
\right
]
$$

Untuk membuktikan 3 fungsi tersebut Memiliki solusi 1 0 0 maka dilakukanlah:

$$AX=b$$

$$A^{-1}AX=A^{-1}b$$

$$IX=A^{-1}b$$

$$X=A^{-1}b$$
$$
\left[
\begin{array}{ccc|ccc}
x1 \\
x2 \\
x3
\end{array}
\right
]
\left[
\begin{array}{ccc|ccc}
4&-1&3 \\
1&3&-2 \\
2&1&1
\end{array}
\right
]
{=}
\left[
\begin{array}{ccc|ccc}
4&-1&3 \\
1&3&-2 \\
2&1&1
\end{array}
\right
]
\left[
\begin{array}{ccc|ccc}
1 \\
0 \\
0
\end{array}
\right
]
$$
$$
\left[
\begin{array}{ccc|ccc}
4\times 1 +(-1\times 0)+3\times0 \\
1\times 1+3\times0+(-2\times0) \\
2\times0+1\times0+1\times0
\end{array}
\right
]
{=}
\left[
\begin{array}{ccc|ccc}
4 \\
1 \\
2
\end{array}
\right
]
$$

