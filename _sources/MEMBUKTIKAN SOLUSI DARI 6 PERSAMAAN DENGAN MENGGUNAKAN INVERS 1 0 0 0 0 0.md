---
title: MEMBUKTIKAN SOLUSI DARI 6 PERSAMAAN DENGAN MENGGUNAKAN INVERS 1 0 0 0 0 0

---

# MEMBUKTIKAN SOLUSI DARI 6 PERSAMAAN DENGAN MENGGUNAKAN INVERS 1 0 0 0 0 0

## Persamaan:
$4x1-x2+x3+x4-x5+x6=4$
$x1+3x2-2x3+3x4+x5+4x6=1$
$2x1+x2+x3-x4+x5+x6=2$
$3x1+x2+2x3+5x4+x5+x6=3$
$6x1+x2+x3-x4+x5+x6=6$
$5x1+3x2+x3+2x4+x5+x6=5$

## Solusi

Membuat Matriks A dan Matriks Identitas I:


$$
A=
\left[
\begin{array}{cccccc|cccccc}
4 & -1 & 1 &1&-1&1\\
1 & 3 & -2 &3&1&4\\
2 & 1 & 1&-1&1&1\\
3&1&2&5&1&1\\
6&1&1&-1&1&1\\
5&3&1&2&1&1
\end{array}
\right]
$$

Matriks Identitas I adalah:

$$
i=
\left[
\begin{array}{cccccc|cccccc}
1&0&0&0&0&0\\
0&1&0&0&0&0\\
0&0&1&0&0&0\\
0&0&0&1&0&0\\
0&0&0&0&1&0\\
0&0&0&0&0&1
\end{array}
\right]
$$

Gabungkan Matriks A dan Matriks Identitas I Menjadi [A|I]:

$$
[A|i]=
\left[
\begin{array}{cccccc|cccccc}
4 & -1 & 1 &1&-1&1&1&0&0&0&0&0\\
1 & 3 & -2 &3&1&4&0&1&0&0&0&0\\
2 & 1 & 1&-1&1&1&0&0&1&0&0&0\\
3&1&2&5&1&1&0&0&0&1&0&0\\
6&1&1&-1&1&1&0&0&0&0&1&0\\
5&3&1&2&1&1&0&0&0&0&0&1
\end{array}
\right]
$$

Lakukan Eliminasi Untuk mengubah Matriks A menjadi Matriks Identitas I

Eliminasi A11 menjadi 1:

$$
[A|i]=
\left[
\begin{array}{cccccc|cccccc}
1&-\frac{1}{4}&\frac{1}{4}&\frac{1}{4}&-\frac{1}{4}&\frac{1}{4}&\frac{1}{4}&0&0&0&0&0\\
1 & 3 & -2 &3&1&4&0&1&0&0&0&0\\
2 & 1 & 1&-1&1&1&0&0&1&0&0&0\\
3&1&2&5&1&1&0&0&0&1&0&0\\
6&1&1&-1&1&1&0&0&0&0&1&0\\
5&3&1&2&1&1&0&0&0&0&0&1
\end{array}
\right]
$$

buat elemen A21, A31, A41, A51, dan A61 menjadi 0

$$R2=R2-R1$$

$$A21=1-1=0$$
$$R3=R3-2R1$$

$$A31=2-2.1=0$$
$$R4=R3-3R1$$

$$A41=3-3.1=0$$
$$R5=R5-6R1$$

$$A51=6-6.1=0$$
$$R6=R6-5.R1$$

$$A61=5-5.1=0$$
$$
[A|I]=
\left[
\begin{array}{cccccc|cccccc}
1&-\frac{1}{4}&\frac{1}{4}&\frac{1}{4}&-\frac{1}{4}&\frac{1}{4}&\frac{1}{4}&0&0&0&0&0\\
0 & -\frac{13}{4} & -\frac{9}{4} &\frac{11}{4}&\frac{5}{4}&\frac{15}{4}&-\frac{1}{4}&1&0&0&0&0\\
0 & \frac{3}{2} & \frac{1}{2}&-\frac{3}{2}&\frac{3}{2}&\frac{1}{2}&-\frac{1}{2}&0&1&0&0&0\\
0&\frac{7}{4}&\frac{5}{4}&\frac{17}{4}&\frac{7}{4}&\frac{1}{4}&-\frac{3}{4}&0&0&1&0&0\\
0&\frac{3}{2}&-\frac{1}{2}&-\frac{5}{2}&\frac{5}{2}&-\frac{1}{2}&-\frac{3}{2}&0&0&0&1&0\\
0&\frac{17}{4}&-\frac{1}{4}&\frac{3}{4}&\frac{9}{4}&-\frac{1}{4}&-\frac{5}{4}&0&0&0&0&1
\end{array}
\right]
$$

Membuat elemen A22 menjadi 1:

$$R2=\frac{4}{13}R2$$
$$
[A|I]=
\left[
\begin{array}{cccccc|cccccc}
1&-\frac{1}{4}&\frac{1}{4}&\frac{1}{4}&-\frac{1}{4}&\frac{1}{4}&\frac{1}{4}&0&0&0&0&0\\
0 & 1 & -\frac{9}{13} &\frac{11}{13}&\frac{5}{13}&\frac{15}{13}&-\frac{1}{13}&\frac{4}{13}&0&0&0&0\\
0 & \frac{3}{2} & \frac{1}{2}&-\frac{3}{2}&\frac{3}{2}&\frac{1}{2}&-\frac{1}{2}&0&1&0&0&0\\
0&\frac{7}{4}&\frac{5}{4}&\frac{17}{4}&\frac{7}{4}&\frac{1}{4}&-\frac{3}{4}&0&0&1&0&0\\
0&\frac{3}{2}&-\frac{1}{2}&-\frac{5}{2}&\frac{5}{2}&-\frac{1}{2}&-\frac{3}{2}&0&0&0&1&0\\
0&\frac{17}{4}&-\frac{1}{4}&\frac{3}{4}&\frac{9}{4}&-\frac{1}{4}&-\frac{5}{4}&0&0&0&0&1
\end{array}
\right]
$$
Membuat Elemen A12, A32, A42, A52, dan A62 menjadi 0

$$R1=R1+\frac{1}{4} R2$$
$$R3=R3-\frac{3}{2} R2$$
$$R4=R4-\frac{7}{4} R2$$
$$R5=R5-\frac{5}{2} R2$$
$$R6=R6-\frac{17}{4} R2$$
$$
[A|I]=
\left[
\begin{array}{cccccc|cccccc}
1&0&\frac{1}{13}&\frac{6}{13}&-\frac{2}{13}&\frac{7}{13}&\frac{3}{13}&\frac{1}{13}&0&0&0&0\\
0 & 1 & -\frac{9}{13} &\frac{11}{13}&\frac{5}{13}&\frac{15}{13}&-\frac{1}{13}&\frac{4}{13}&0&0&0&0\\
0 & 0 & \frac{20}{13}&-\frac{36}{13}&\frac{12}{13}&\frac{16}{13}&-\frac{5}{13}&\frac{6}{13}&1&0&0&0\\
0&0&\frac{32}{13}&\frac{36}{13}&\frac{14}{13}&-\frac{23}{13}&-\frac{8}{13}&-\frac{7}{13}&0&1&0&0\\
0&0&-\frac{16}{13}&-\frac{60}{13}&\frac{20}{13}&-\frac{44}{13}&-\frac{17}{13}&-\frac{10}{13}&0&0&1&0\\
0&0&-\frac{35}{13}&-\frac{37}{13}&\frac{8}{13}&-\frac{67}{13}&-\frac{12}{13}&-\frac{17}{13}&0&0&0&1
\end{array}
\right]
$$

Membuat Elemen A33 menjadi 1 :

$$R3=\frac{13}{20}R3$$
$$
[A|I]=
\left[
\begin{array}{cccccc|cccccc}
1&0&\frac{1}{13}&\frac{6}{13}&-\frac{2}{13}&\frac{7}{13}&\frac{3}{13}&\frac{1}{13}&0&0&0&0\\
0 & 1 & -\frac{9}{13} &\frac{11}{13}&\frac{5}{13}&\frac{15}{13}&-\frac{1}{13}&\frac{4}{13}&0&0&0&0\\
0 & 0 & 1&-\frac{9}{5}&\frac{3}{5}&-\frac{4}{5}&-\frac{1}{4}&-\frac{3}{10}&\frac{13}{20}&0&0&0\\
0&0&\frac{32}{13}&\frac{36}{13}&\frac{14}{13}&-\frac{23}{13}&-\frac{8}{13}&-\frac{7}{13}&0&1&0&0\\
0&0&-\frac{16}{13}&-\frac{60}{13}&\frac{20}{13}&-\frac{44}{13}&-\frac{17}{13}&-\frac{10}{13}&0&0&1&0\\
0&0&-\frac{35}{13}&-\frac{37}{13}&\frac{8}{13}&-\frac{67}{13}&-\frac{12}{13}&-\frac{17}{13}&0&0&0&1
\end{array}
\right]
$$

Membuat elemen A13, A23, A43, A53, dan A63 menjadi 0

$$R1=R1-\frac{1}{13}R3$$
$$R2=R2+\frac{9}{13}R3$$
$$R4=R4-\frac{32}{13}R3$$
$$R5=R5-\frac{16}{13}R3$$
$$R6=R6-\frac{35}{13}R3$$
$$
[A|I]=
\left[
\begin{array}{cccccc|cccccc}
1&0&0&\frac{3}{5}&-\frac{1}{5}&\frac{3}{5}&\frac{1}{4}&\frac{1}{10}&-\frac{1}{20}&0&0&0\\
0 & 1 & 0 &-\frac{2}{5}&\frac{4}{5}&\frac{3}{5}&-\frac{1}{4}&\frac{1}{10}&\frac{9}{20}&0&0&0\\
0 & 0 & 1&-\frac{9}{5}&\frac{3}{5}&-\frac{4}{5}&-\frac{1}{4}&-\frac{3}{10}&\frac{13}{20}&0&0&0\\
0&0&0&\frac{36}{5}&-\frac{2}{5}&\frac{1}{5}&0&-\frac{1}{5}&\frac{4}{5}&1&0&0\\
0&0&0&-\frac{12}{5}&\frac{4}{5}&-\frac{12}{5}&-1&-\frac{2}{5}&\frac{4}{5}&0&1&0\\
0&0&0&2&-1&-3&-\frac{1}{4}&-\frac{1}{2}&-\frac{7}{4}&0&0&1
\end{array}
\right]
$$

Membuat elemen A44 menjadi 1:

$$R4=\frac{5}{36}R4$$
$$
[A|I]=
\left[
\begin{array}{cccccc|cccccc}
1&0&0&\frac{3}{5}&-\frac{1}{5}&\frac{3}{5}&\frac{1}{4}&\frac{1}{10}&-\frac{1}{20}&0&0&0\\
0 & 1 & 0 &-\frac{2}{5}&\frac{4}{5}&\frac{3}{5}&-\frac{1}{4}&\frac{1}{10}&\frac{9}{20}&0&0&0\\
0 & 0 & 1&-\frac{9}{5}&\frac{3}{5}&-\frac{4}{5}&-\frac{1}{4}&-\frac{3}{10}&\frac{13}{20}&0&0&0\\
0&0&0&1&-\frac{1}{18}&\frac{1}{36}&0&-\frac{1}{36}&-\frac{2}{9}&\frac{5}{36}&0&0\\
0&0&0&-\frac{12}{5}&\frac{4}{5}&-\frac{12}{5}&-1&-\frac{2}{5}&\frac{4}{5}&0&1&0\\
0&0&0&2&-1&-3&-\frac{1}{4}&-\frac{1}{2}&-\frac{7}{4}&0&0&1
\end{array}
\right]
$$

Membuat elemen A14, A24, A34, A54, dan A64 menjadi 0

$$R1=R1-\frac{3}{5}R4$$
$$R2=R2+\frac{2}{5}R4$$
$$R3=R3+\frac{9}{5}R4$$
$$R5=R5+\frac{12}{5}R4$$
$$R6=R6-2R4$$

$$
[A|I]=
\left[
\begin{array}{cccccc|cccccc}
1&0&0&0&-\frac{1}{6}&\frac{7}{12}&\frac{1}{4}&\frac{1}{12}&-\frac{1}{12}&-\frac{1}{12}&0&0\\
0 & 1 & 0 &0&\frac{7}{9}&\frac{11}{18}&-\frac{1}{4}&\frac{1}{9}&\frac{13}{36}&\frac{1}{18}&0&0\\
0 & 0 & 1&0&\frac{1}{2}&-\frac{3}{4}&-\frac{1}{4}&-\frac{1}{4}&\frac{1}{4}&\frac{1}{4}&0&0\\
0&0&0&1&-\frac{1}{18}&\frac{1}{36}&0&-\frac{1}{36}&-\frac{2}{9}&\frac{5}{36}&0&0\\
0&0&0&0&\frac{2}{3}&-\frac{7}{3}&-1&-\frac{1}{3}&-\frac{4}{3}&\frac{1}{3}&1&0\\
0&0&0&0&-\frac{8}{9}&-\frac{55}{18}&-\frac{1}{4}&-\frac{5}{9}&-\frac{47}{36}&\frac{5}{18}&0&1
\end{array}
\right]
$$

Membuat elemen A55 menjadi 0:
$$R5=\frac{3}{2}R5$$
$$
[A|I]=
\left[
\begin{array}{cccccc|cccccc}
1&0&0&0&-\frac{1}{6}&\frac{7}{12}&\frac{1}{4}&\frac{1}{12}&-\frac{1}{12}&-\frac{1}{12}&0&0\\
0 & 1 & 0 &0&\frac{7}{9}&\frac{11}{18}&-\frac{1}{4}&\frac{1}{9}&\frac{13}{36}&\frac{1}{18}&0&0\\
0 & 0 & 1&0&\frac{1}{2}&-\frac{3}{4}&-\frac{1}{4}&-\frac{1}{4}&\frac{1}{4}&\frac{1}{4}&0&0\\
0&0&0&1&-\frac{1}{18}&\frac{1}{36}&0&-\frac{1}{36}&-\frac{2}{9}&\frac{5}{36}&0&0\\
0&0&0&0&1&-\frac{7}{2}&-\frac{5}{2}&-\frac{1}{2}&-2&\frac{1}{2}&\frac{5}{2}&0\\
0&0&0&0&-\frac{8}{9}&-\frac{55}{18}&-\frac{1}{4}&-\frac{5}{9}&-\frac{47}{36}&\frac{5}{18}&0&1
\end{array}
\right]
$$

Membuat elemen A15, A25, A35, A45, dan A65 menjadi 0
$$R1=R1+\frac{1}{6}R5$$
$$R2=R2+\frac{7}{9}R5$$
$$R3=R3-\frac{1}{2}R5$$
$$R4=R4+\frac{1}{18}R5$$
$$R6=R6+\frac{8}{9}R5$$

$$
[A|I]=
\left[
\begin{array}{cccccc|cccccc}
1&0&0&0&0&0&0&0&-\frac{1}{4}&0&\frac{1}{4}&0\\
0 & 1 & 0 &0&0&\frac{10}{3}&\frac{11}{12}&\frac{1}{2}&\frac{23}{12}&-\frac{1}{3}&-\frac{7}{6}&0\\
0 & 0 & 1&0&0&1&\frac{1}{2}&0&\frac{5}{4}&0&-\frac{3}{4}&0\\
0&0&0&1&0&-\frac{1}{6}&-\frac{1}{12}&0&-\frac{1}{3}&\frac{1}{6}&\frac{1}{12}&0\\
0&0&0&0&1&-\frac{7}{2}&-\frac{5}{2}&-\frac{1}{2}&-2&\frac{1}{2}&\frac{5}{2}&0\\
0&0&0&0&0&-\frac{37}{6}&-\frac{19}{12}&-1&-\frac{37}{12}&\frac{1}{6}&\frac{4}{3}&1
\end{array}
\right]
$$

Membuat elemen A66 menjadi 0
$$R6=-\frac{6}{37}R6$$
$$
[A|I]=
\left[
\begin{array}{cccccc|cccccc}
1&0&0&0&0&0&0&0&-\frac{1}{4}&0&\frac{1}{4}&0\\
0 & 1 & 0 &0&0&\frac{10}{3}&\frac{11}{12}&\frac{1}{2}&\frac{23}{12}&-\frac{1}{3}&-\frac{7}{6}&0\\
0 & 0 & 1&0&0&1&\frac{1}{2}&0&\frac{5}{4}&0&-\frac{3}{4}&0\\
0&0&0&1&0&-\frac{1}{6}&-\frac{1}{12}&0&-\frac{1}{3}&\frac{1}{6}&\frac{1}{12}&0\\
0&0&0&0&1&-\frac{7}{2}&-\frac{5}{2}&-\frac{1}{2}&-2&\frac{1}{2}&\frac{5}{2}&0\\
0&0&0&0&0&1&\frac{19}{74}&\frac{6}{37}&\frac{1}{2}&-\frac{1}{37}&-\frac{8}{37}&\frac{6}{3}
\end{array}
\right]
$$

Membuat elemen A26, A36, A46, dan A56 menjadi 0
$$R2=R2-\frac{10}{3}R6$$
$$R3=R3-1R6$$
$$R4=R4+\frac{1}{6}R6$$
$$R5=R5+\frac{7}{2}R6$$
$$
[A|I]=
\left[
\begin{array}{cccccc|cccccc}
1&0&0&0&0&0&0&0&-\frac{1}{4}&0&\frac{1}{4}&0\\
0 & 1 & 0 &0&0&0&\frac{2}{33}&-\frac{3}{74}&\frac{1}{4}&-\frac{9}{37}&-\frac{33}{74}&\frac{20}{37}\\
0 & 0 & 1&0&0&0&\frac{9}{37}&-\frac{6}{37}&\frac{3}{4}&\frac{1}{37}&-\frac{8}{15}&\frac{6}{37}\\
0&0&0&1&0&0&-\frac{3}{74}&-\frac{1}{37}&-\frac{1}{4}&\frac{6}{37}&\frac{1}{21}&-\frac{1}{37}\\
0&0&0&0&1&0&-\frac{3}{5}&\frac{5}{74}&-\frac{1}{4}&\frac{15}{37}&\frac{55}{74}&\frac{21}{37}\\
0&0&0&0&0&1&\frac{19}{74}&\frac{6}{37}&\frac{1}{2}&-\frac{1}{37}&-\frac{8}{37}&-\frac{6}{37}
\end{array}
\right]
$$

Setelah eliminasi Gauss, matriks A telah Diubah menjadi matriks I dan matriks I telah menjadi invers matriks $A (A^{-1})$

$$
A^{-1}=
\left[
\begin{array}{cccccc|cccccc}
1&0&0&0&0&0&0&0&-\frac{1}{4}&0&\frac{1}{4}&0\\
0 & 1 & 0 &0&0&0&\frac{2}{33}&-\frac{3}{74}&\frac{1}{4}&-\frac{9}{37}&-\frac{33}{74}&\frac{20}{37}\\
0 & 0 & 1&0&0&0&\frac{9}{37}&-\frac{6}{37}&\frac{3}{4}&\frac{1}{37}&-\frac{8}{15}&\frac{6}{37}\\
0&0&0&1&0&0&-\frac{3}{74}&-\frac{1}{37}&-\frac{1}{4}&\frac{6}{37}&\frac{1}{21}&-\frac{1}{37}\\
0&0&0&0&1&0&-\frac{3}{5}&\frac{5}{74}&-\frac{1}{4}&\frac{15}{37}&\frac{55}{74}&\frac{21}{37}\\
0&0&0&0&0&1&\frac{19}{74}&\frac{6}{37}&\frac{1}{2}&-\frac{1}{37}&-\frac{8}{37}&-\frac{6}{37}
\end{array}
\right]
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
x3 \\
x4 \\
x5 \\
x6
\end{array}
\right
]
\left[
\begin{array}{cccccc|cccccc}
4 & -1 & 1 &1&-1&1\\
1 & 3 & -2 &3&1&4\\
2 & 1 & 1&-1&1&1\\
3&1&2&5&1&1\\
6&1&1&-1&1&1\\
5&3&1&2&1&1
\end{array}
\right
]
{=}
\left[
\begin{array}{cccccc|cccccc}
4 & -1 & 1 &1&-1&1\\
1 & 3 & -2 &3&1&4\\
2 & 1 & 1&-1&1&1\\
3&1&2&5&1&1\\
6&1&1&-1&1&1\\
5&3&1&2&1&1
\end{array}
\right
]
\left[
\begin{array}{ccc|ccc}
1 \\
0 \\
0 \\
0 \\
0 \\
0
\end{array}
\right
]
$$
$$
\left[
\begin{array}{cccccc|cccccc}
4\times1+(-1\times0) + 1\times0 +1\times0+(-1\times0)+1\times0\\
1\times1+ 3\times0 + (-2\times0) +3\times0+1\times0+4\times0\\
2\times1+ 1\times0 + 1\times0+(-1\times0)+1\times0+1\times0\\
3\times1+1\times0+2\times0+5\times0+1\times0+1\times0\\
6\times1+1\times0+1\times0+(-1\times0)+1\times0+1\times0\\
5\times1+3\times0+1\times0+2\times0+1\times0+1\times0
\end{array}
\right
]
{=}
\left[
\begin{array}{ccc|ccc}
4 \\
1 \\
2\\
3\\
6\\
5
\end{array}
\right
]
$$

