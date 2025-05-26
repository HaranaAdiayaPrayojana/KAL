---
title: EigenVektor dan EigenValue

---

# EigenVektor dan EigenValue

- EigenVektor adalah skalar (angka) yang menyatakan berapa kali EigenVector berubah karena transformasi itu, Atau digunakan untuk mengubah atau meregangkan EigenVector.
- EigenValue adalah vektor spesial yang tidak berubah arah saat transformasi-panjangnya bisa berubah (diperbesar atau diperkecil), tapi arahnya tetap.

## Penggunaan EigenValues dan EigenVector

### Cara yang biasa

$$Av=\lambda v$$

Matriks A:
$$
A=
\begin{bmatrix}
2&1\\
1&2
\end{bmatrix}
$$

solusi:

- mencari nilai eigen:
$$Av=\lambda v$$

$$
A =
\begin{bmatrix}
2&1\\
1&2
\end{bmatrix}
$$

- Nilai Eigen $\lambda_1$=3, vektor Eigen $v_1 =\begin{bmatrix}1\\1\end{bmatrix}$

- Nilai Eigen $\lambda_2$=1, vektor eigen $v_2=\begin{bmatrix}-1\\1\end{bmatrix}$

### Dengan menggunakan Code Python

```python
# Codenya.
import numpy as np

# Matriks A
A = np.array([[2, 1],[1, 2]])

# Hitung eigenvalue dan eigenvector
eigenvalues, eigenvectors = np.linalg.eig(A)

# Urutkan indeks berdasarkan eigenvalue dari besar ke kecil
sorted_indices = np.argsort(eigenvalues)[::-1]

# Urutkan eigenvalue dan eigenvector sesuai indeks
eigenvalues_sorted = eigenvalues[sorted_indices]
eigenvectors_sorted = eigenvectors[:, sorted_indices]

# Cetak hasil
print("Eigenvalues (terurut):")
print(eigenvalues_sorted)
print(" ")
print("Eigenvectors (mengikuti eigenvalues):")
print(eigenvectors_sorted)
```
output:

```python
Eigenvalues (terurut):
[3. 1.]
 
Eigenvectors (mengikuti eigenvalues):
[[ 0.70710678 -0.70710678]
 [ 0.70710678  0.70710678]]
```

## Cara Menentukan Nilai EigenVektor dan EigenValue

### Menggunkan Rumus:

- Diberikan sebuah matriks A berukuran n x n. Vektor eigen dan nilai eigen
dari matriks A dihitung sebagai berikut:
$Av=\lambda v$
$(A-\lambda i)v=0$

v=0 adalah solusi trivial dari $(A-\lambda i)v=0$

agar $(A-\lambda i)v=0$ memiliki solusi tidak-nol, maka haruslah $det(A-\lambda i)=0$



$$
A=
\begin{bmatrix}
8&-10\\
5&-7
\end{bmatrix}
$$

- menentukan nilai-nilai Eigen

$$A-\lambda i=0$$

$$
\lambda\times
\begin{bmatrix}
1&0\\
0&1
\end{bmatrix}-
\begin{bmatrix}
8&-10\\
5&-7
\end{bmatrix}=0
$$

$$
\begin{bmatrix}
8-\lambda &-10\\
5&-7-\lambda
\end{bmatrix}=0
$$

$$(8-\lambda)(-7-\lambda)-(-10)(5)$$

$$\lambda^2 - \lambda-6=0$$

$$(\lambda-3)(\lambda+2)=0$$

$$\lambda_1 =3$$

$$\lambda_2 =-2$$

jadi, nilai-nilai eigen dari matrix A adalah $\lambda_1=3$ dan $\lambda_2=-2$.

- Menentukan Vektor Eigen
$$
(\lambda i -A)v=0 \rightarrow
\begin{bmatrix}
8-\lambda &-10\\
5&-7-\lambda
\end{bmatrix}
\begin{bmatrix}
v_1\\
v_2
\end{bmatrix}=
\begin{bmatrix}
0\\
0
\end{bmatrix}
$$

$$
Untuk\space \lambda_1 =3 \rightarrow
\begin{bmatrix}
5 &-10\\
5&-10
\end{bmatrix}
\begin{bmatrix}
v_1\\
v_2
\end{bmatrix}=
\begin{bmatrix}
0\\
0
\end{bmatrix}
$$

$$5v_1 - 10v_2 =0 \rightarrow v_1=2v_2\space atau 
\begin{bmatrix}
2\\
1
\end{bmatrix}
$$
$$
Untuk\space \lambda_2 =-2 \rightarrow
\begin{bmatrix}
10 &-10\\
5&-5
\end{bmatrix}
\begin{bmatrix}
v_1\\
v_2
\end{bmatrix}=
\begin{bmatrix}
0\\
0
\end{bmatrix}
$$

$$10v_1 - 10v_2 =0 \rightarrow v_1=v_2\space atau 
\begin{bmatrix}
1\\
1
\end{bmatrix}
$$

- Dengan Code Python:

```python=
import numpy as np

# Matriks A
A = np.array([[8, -10],[5, -7]])

# Hitung eigenvalue dan eigenvector
eigenvalues, eigenvectors = np.linalg.eig(A)

# Urutkan indeks berdasarkan eigenvalue dari besar ke kecil
sorted_indices = np.argsort(eigenvalues)[::-1]

# Urutkan eigenvalue dan eigenvector sesuai indeks
eigenvalues_sorted = eigenvalues[sorted_indices]
eigenvectors_sorted = eigenvectors[:, sorted_indices]

# Cetak hasil
print("Eigenvalues (terurut):")
print(eigenvalues_sorted)
print(" ")
print("Eigenvectors (mengikuti eigenvalues):")
print(eigenvectors_sorted)
```
Output:
```python=
Eigenvalues (terurut):
[ 3. -2.]
 
Eigenvectors (mengikuti eigenvalues):
[[0.89442719 0.70710678]
 [0.4472136  0.70710678]]
```
hasil jika digambarkan di geogebra:

<iframe src="https://www.geogebra.org/graphing/mctm85af?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

## Alasan Perbedaan output
Alasan mengapa Terdapat perbedaan dari hasil code python dan menghitungnya dengan cara manual yaitu Python (NumPy) secara default menghasilkan eigenvector yang dinormalisasi, yaitu memiliki panjang (norma) = 1.
Sedangkan secara manual, kita sering mendapatkan bentuk proporsional (bebas skalar).

contoh:
- hasil manual=$\begin{bmatrix}
2\\
1
\end{bmatrix}$

- hasil python=$\begin{bmatrix}
0.8944\\
0.4472
\end{bmatrix}$
(Memiliki arah yang sama, hanya berbeda skala saja)