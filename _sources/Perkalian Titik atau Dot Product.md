---
title: Perkalian Titik atau Dot Product

---



# Perkalian Titik atau Dot Product

Perkalian Titik atau Dot Prouct dapat membantu dalam mengukur panjang vektor dan sudut yang dibentuk oleh sepadang vektor. Untuk vektor-vektor dua dimensi v dan w, hasil kali titik (v.w) didefinisikan sebagai bilangan skalar berikut:

$$
v.w=
\begin{bmatrix}
v_1\\
v_2
\end{bmatrix}.
\begin{bmatrix}
w_1\\
w_2
\end{bmatrix}=
v_1w_1+v_2w_2.
$$

## Geometri dari Hasil Kali Titik

Hasil kali dari dua titik akan menghasilkan sebuah bilangan skalar, Artinya dua vektor digabungkan dalam cara tertentu sehingga menghasilkan sebuah nilai. Hasil kali titik untuk dua vektor berdimensi m sebagai berikut:

$$
v.w=
\begin{bmatrix}
v_1\\
v_2\\
:\\
v_m
\end{bmatrix}.
\begin{bmatrix}
w_1\\
w_2\\
:\\
w_m
\end{bmatrix}=
v_1w_1+v_2w_2+...+v_m w_m
$$

contoh:

$$
v.w=
\begin{bmatrix}
2\\
0\\
-3\\
1
\end{bmatrix}.
\begin{bmatrix}
-1\\
3\\
1\\
2
\end{bmatrix}=
2(-1)+0(-3)+(-3)(1)+1(2)=-3
$$

## contoh penerapan Dot Product dalam Basis dua dimensi:

$$
A=
\begin{bmatrix}
1&0\\
0&1
\end{bmatrix}
$$

$$
v=
\begin{bmatrix}
1\\0
\end{bmatrix}
w=
\begin{bmatrix}
0\\1
\end{bmatrix}
$$

$$
\begin{bmatrix}
1\\
0
\end{bmatrix}.
\begin{bmatrix}
0\\
1
\end{bmatrix}=
1\times 0+0\times 1=0
$$

Digambar menggunakan geogebra:

<iframe src="https://www.geogebra.org/classic/ja8x3vuj?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

contoh lainnya:

$$
A=
\begin{bmatrix}
2&4\\
-3&1
\end{bmatrix}
$$

$$
v=
\begin{bmatrix}
2\\-3
\end{bmatrix}
w=
\begin{bmatrix}
4\\1
\end{bmatrix}
$$

$$
\begin{bmatrix}
2\\
-3
\end{bmatrix}.
\begin{bmatrix}
4\\
1
\end{bmatrix}=
2\times 4+(-3)\times 1=5
$$

jadi sumbu v dan w memiliki dot product dengan nilai 5 dengan sudut 70.35 derajat.

Digambar menggunakan geogebra:

<iframe src="https://www.geogebra.org/classic/aawhgt67?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

Jika terdapat dua titik yang menghasikan sudut 90 derajat, maka nilai Dot Product dari kedua titik tersebut. Contoh
$$
v=
\begin{bmatrix}
-1\\
2
\end{bmatrix}
u=
\begin{bmatrix}
2\\
1
\end{bmatrix}
$$

$$
v.w=
\begin{bmatrix}
v_1\\
v_2
\end{bmatrix}.
\begin{bmatrix}
w_1\\
w_2
\end{bmatrix}=
v_1w_1+v_2w_2.
$$

$$
v.w=
\begin{bmatrix}
-1\\
2
\end{bmatrix}.
\begin{bmatrix}
2\\
1
\end{bmatrix}=
-1\times 2+2\times 1=0
$$

# Perkalian titik dan panjang vektor

## Panjang Vektor di $\mathbb{R}^2$

Dalam ruang vektor dua dimensi panjang x=(x,y), didefinisikan sebagai jarak dari titik asal (0,0). Jarak ini dihitung menggunkan Teorema Pythagoras dimana:

$$\text{Panjang vektor } \mathbf{x} = \sqrt{x^2 + y^2}.$$

## Implementasi Geometris

vektor x=(x,y) dapat diwakili oleh garis lurus dari titik asal, hingga (x,y). Panjang ini adalah hipotenusa segitiga siku siku dengan kaki kakinya sepanjang x dan y.  $\mathbb{R}^2$ adalah jarak dari titik asal hingga x(x,y), yang digunakan untuk menghitung jarak;
$$d = \sqrt{x^2 + y^2}.$$

contoh:

<iframe src="https://www.geogebra.org/classic/j5xmhmxn?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

Misalkan vector $u=(3,4)$:

$$|\mathbf{U}| = \sqrt{3^2 + 4^2} = \sqrt{9 + 16} = \sqrt{25} = 5.$$

