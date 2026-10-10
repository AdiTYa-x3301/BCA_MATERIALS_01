# Matrices and Determinants 


---

##  — MATRICES

### Examples of Matrices

1. \(\begin{bmatrix}1&2&3\\0&6&8\end{bmatrix}\) — order \(2\times3\)
2. \(\begin{bmatrix}1&5&4\\7&8&9\\3&9&7\end{bmatrix}\) — order \(3\times3\)
3. \(\begin{bmatrix}1\\6\\7\\8\end{bmatrix}\) — order \(4\times1\)
4. \(\begin{bmatrix}x^2+1&4x-2\\x^3&x-3\end{bmatrix}\) — order \(2\times2\)

### Order of a Matrix

The order of a matrix is defined as:

**No. of Rows × No. of Cols.**

Examples:

- \(\begin{bmatrix}1&2&3\\0&6&8\end{bmatrix}\rightarrow 2\times3\)
- \(\begin{bmatrix}1&5&4\\7&8&9\\3&9&7\end{bmatrix}\rightarrow 3\times3\)
- \(\begin{bmatrix}1\\6\\7\\8\end{bmatrix}\rightarrow 4\times1\)
- \(\begin{bmatrix}x^2+1&4x-2\\x^3&x-3\end{bmatrix}\rightarrow 2\times2\)

### Elements of a Matrix

Let

\[
A=\begin{bmatrix}1&5&4\\7&8&9\\3&9&7\end{bmatrix}.
\]

The elements of \(A\) are denoted by \(a_{ij}\), where \(i\) = row number and \(j\) = column number.

\[
\begin{aligned}
a_{11}&=1 & a_{12}&=5 & a_{13}&=4\\
a_{21}&=7 & a_{22}&=8 & a_{23}&=9\\
a_{31}&=3 & a_{32}&=9 & a_{33}&=7
\end{aligned}
\]

---

## Page 2 — Construct a Matrix

**Question:** Construct a \(3\times4\) matrix \(A=[a_{ij}]\), whose element \(a_{ij}\) is given by

\[
a_{ij}=\frac{(i+j)^2}{2},\qquad 1\leq i\leq3,\quad 1\leq j\leq4.
\]

**Solution:** We have

\[
a_{ij}=\frac{(i+j)^2}{2},\qquad 1\leq i\leq3,\quad 1\leq j\leq4.
\]

To find \(a_{11}\), put \(i=1,j=1\) in \(a_{ij}\):

\[
a_{11}=\frac{(1+1)^2}{2}=\frac{2^2}{2}=\frac42=2.
\]

To find \(a_{12}\), put \(i=1,j=2\) in \(a_{ij}\):

\[
a_{12}=\frac{(1+2)^2}{2}=\frac{3^2}{2}=\frac92.
\]

To find \(a_{13}\), put \(i=1,j=3\) in \(a_{ij}\):

\[
a_{13}=\frac{(1+3)^2}{2}=\frac{4^2}{2}=\frac{16}{2}=8.
\]

To find \(a_{14}\), put \(i=1,j=4\) in \(a_{ij}\):

\[
a_{14}=\frac{(1+4)^2}{2}=\frac{5^2}{2}=\frac{25}{2}.
\]

To find \(a_{21}\), put \(i=2,j=1\) in \(a_{ij}\):

\[
a_{21}=\frac{(2+1)^2}{2}=\frac{3^2}{2}=\frac92.
\]

To find \(a_{22}\), put \(i=2,j=2\) in \(a_{ij}\):

\[
a_{22}=\frac{(2+2)^2}{2}=\frac{4^2}{2}=\frac{16}{2}=8.
\]

To find \(a_{23}\), put \(i=2,j=3\) in \(a_{ij}\):

\[
a_{23}=\frac{(2+3)^2}{2}=\frac{5^2}{2}=\frac{25}{2}.
\]

To find \(a_{24}\), put \(i=2,j=4\) in \(a_{ij}\):

\[
a_{24}=\frac{(2+4)^2}{2}=\frac{6^2}{2}=\frac{36}{2}=18.
\]

To find \(a_{31}\), put \(i=3,j=1\) in \(a_{ij}\):

\[
a_{31}=\frac{(3+1)^2}{2}=\frac{4^2}{2}=\frac{16}{2}=8.
\]

To find \(a_{32}\), put \(i=3,j=2\) in \(a_{ij}\):

\[
a_{32}=\frac{(3+2)^2}{2}=\frac{5^2}{2}=\frac{25}{2}.
\]

To find \(a_{33}\), put \(i=3,j=3\) in \(a_{ij}\):

\[
a_{33}=\frac{(3+3)^2}{2}=\frac{6^2}{2}=\frac{36}{2}=18.
\]

To find \(a_{34}\), put \(i=3,j=4\) in \(a_{ij}\):

\[
a_{34}=\frac{(3+4)^2}{2}=\frac{7^2}{2}=\frac{49}{2}.
\]

Hence,

\[
A=\begin{bmatrix}
2&\frac92&8&\frac{25}{2}\\
\frac92&8&\frac{25}{2}&18\\
8&\frac{25}{2}&18&\frac{49}{2}
\end{bmatrix}.
\]

---

## Page 3 — Types of Matrices

| S. No. | Type of matrix | Definition | Example shown in the source |
|---|---|---|---|
| 1 | Square Matrix | A matrix is called a square matrix if the number of rows and columns in the matrix are equal. | \(\begin{bmatrix}1&4&7\\2&5&2\\3&6&1\end{bmatrix}\), order \(3\times3\) |
| 2 | Row Matrix | A matrix is called a row matrix if it contains only one row. | \(\begin{bmatrix}1&5&4&3\end{bmatrix}\), order \(1\times4\) |
| 3 | Column Matrix | A matrix is called a column matrix if it contains only one column. | \(\begin{bmatrix}1\\4\\2\end{bmatrix}\), order \(3\times1\) |
| 4 | Zero (or Null) Matrix | A matrix is called a zero matrix if all its elements are zero. It is denoted by ‘0’. | \(\begin{bmatrix}0&0\\0&0\end{bmatrix}\), order \(2\times2\) |
| 5 | Diagonal Matrix | A square matrix is called a diagonal matrix if all its non-diagonal elements are zero. | \(\begin{bmatrix}1&0&0\\0&3&0\\0&0&6\end{bmatrix}\), order \(3\times3\) |
| 6 | Scalar Matrix | A square matrix is called a scalar matrix if all its non-diagonal elements are zero and all diagonal elements are equal. | \(\begin{bmatrix}4&0&0\\0&4&0\\0&0&4\end{bmatrix}\), order \(3\times3\) |
| 7 | Unit Matrix or Identity Matrix | A square matrix is called a unit matrix if all its non-diagonal elements are zero and all diagonal elements are unity. | \(\begin{bmatrix}1&0&0\\0&1&0\\0&0&1\end{bmatrix}\), order \(3\times3\) |
| 8 | Triangular Matrices | A square matrix is called a triangular matrix if all its elements either below or above the principal diagonal are zero. | Upper and lower triangular examples below. |

**(i) Upper Triangular Matrix:** If all elements below the principal diagonal are zero.

Example: \(\begin{bmatrix}1&2&3\\0&4&5\\0&0&7\end{bmatrix}\), order \(3\times3\).

**(ii) Lower Triangular Matrix:** If all elements above the principal diagonal are zero.

Example: \(\begin{bmatrix}1&0&0\\4&2&0\\5&6&3\end{bmatrix}\), order \(3\times3\).

---

## Page 4 — Comparable and Equal Matrices

### 9. Comparable Matrices

Two matrices are called comparable if they are of the same order (i.e., they have the same number of rows and the same number of columns).

Example: Let

\[
A=\begin{bmatrix}1&2&3\\4&5&6\end{bmatrix},\qquad
B=\begin{bmatrix}7&8&9\\1&2&3\end{bmatrix}.
\]

A and B are comparable. (Both are of order \(2\times3\).)

### 10. Equal Matrices

Two matrices are called equal matrices if they are of the same order and their corresponding elements are equal.

Example: Let

\[
A=\begin{bmatrix}2&3&4\\5&6&7\end{bmatrix},\qquad
B=\begin{bmatrix}2&3&4\\5&6&7\end{bmatrix}.
\]

A and B are equal matrices.

---

## Page 5 — Equality of Matrices: Finding \(x,y,z\)

**Question 1:** Find the values of \(x,y,z\) if

\[
\begin{bmatrix}2x+y&x-y\\x-z&x+y+z\end{bmatrix}
=
\begin{bmatrix}10&-1\\2&8\end{bmatrix}.
\]

**Solution:** By equality of matrices, corresponding elements are equal.

\[
\begin{aligned}
2x+y&=10 &&(1)\\
x-y&=-1 &&(2)\\
x-z&=2 &&(3)\\
x+y+z&=8 &&(4)
\end{aligned}
\]

\((1)+(2)\):

\[
(2x+y)+(x-y)=10+(-1),\qquad 3x=9,\qquad x=3.
\]

From (2):

\[
x-y=-1\Rightarrow3-y=-1\Rightarrow-y=-4\Rightarrow y=4.
\]

From (3):

\[
x-z=2\Rightarrow3-z=2\Rightarrow-z=-1\Rightarrow z=1.
\]

Therefore, \(x=3,\ y=4,\ z=1\).

### Question 2

If

\[
\begin{bmatrix}2x+1&2y\\0&y^2+1\end{bmatrix}
=
\begin{bmatrix}x+3&10\\0&26\end{bmatrix},
\]

find the value of \(x+y\).

**Solution:** By equality of matrices,

\[
2x+1=x+3\quad(1),\qquad 2y=10\quad(2),\qquad y^2+1=26\quad(3).
\]

From (1): \(2x+1=x+3\Rightarrow2x-x=3-1\Rightarrow x=2\).

From (2): \(2y=10\Rightarrow y=10/2\Rightarrow y=5\).

From (3): \(y^2+1=26\Rightarrow y^2=25\Rightarrow y=\pm5\). But from (2), \(y=5\).

Therefore, \(x+y=2+5=7\).

---

## Page 6 — Equality of Matrices: Finding \(x,y\)

**Question:** For what values of \(x\) and \(y\) are the following matrices equal?

\[
\begin{bmatrix}2x+1&3y\\0&y^2-5y\end{bmatrix},\qquad
\begin{bmatrix}x+3&y^2+2\\0&-6\end{bmatrix}.
\]

**Solution:** For two matrices to be equal, their corresponding elements must be equal. Equating corresponding elements, we get:

\[
\begin{aligned}
2x+1&=x+3 &&(1)\\
3y&=y^2+2 &&(2)\\
0&=0 &&(3)\\
y^2-5y&=-6 &&(4)
\end{aligned}
\]

From (1):

\[
2x+1=x+3\Rightarrow2x-x=3-1\Rightarrow x=2.
\]

From (2):

\[
3y=y^2+2\Rightarrow y^2-3y+2=0\Rightarrow(y-1)(y-2)=0,
\]

so \(y=1\) or \(y=2\).

From (4):

\[
y^2-5y=-6\Rightarrow y^2-5y+6=0\Rightarrow(y-2)(y-3)=0,
\]

so \(y=2\) or \(y=3\).

From both (2) and (4), the common value of \(y\) is \(y=2\).

Therefore, \(x=2,\ y=2\).

---

## Page 7 — Operations on Matrices

### 1. Addition of Matrices

Matrices should have same order.

\[
A=\begin{bmatrix}2&3&6\\4&0&9\end{bmatrix},\qquad
B=\begin{bmatrix}0&6&8\\7&0&8\end{bmatrix}.
\]

\[
A+B=\begin{bmatrix}2+0&3+6&6+8\\4+5&0+0&9+8\end{bmatrix}
=\begin{bmatrix}2&9&14\\11&0&17\end{bmatrix}.
\]

### 2. Subtraction of Matrices

Matrices should have same order.

\[
A-B=\begin{bmatrix}2-0&3-6&6-8\\4-7&0-0&9-8\end{bmatrix}
=\begin{bmatrix}2&-3&-2\\-3&0&1\end{bmatrix}.
\]

### 3. Scalar Multiplication of Matrix

\[
A=\begin{bmatrix}4&7&3\\2&1&2\end{bmatrix},\qquad
3A=\begin{bmatrix}3\times4&3\times7&3\times3\\3\times2&3\times1&3\times2\end{bmatrix}
=\begin{bmatrix}12&21&9\\6&3&6\end{bmatrix}.
\]

Another example shown:

\[
B=\begin{bmatrix}2&6&4\\8&12&8\end{bmatrix},\qquad
\frac12B=\begin{bmatrix}1&3&2\\4&6&4\end{bmatrix}.
\]

**Note:** In addition and subtraction, order must be same. In scalar multiplication, any scalar can be used.

---

## Page 8 — Solve the Matrix Equation

**Question:** Solve the matrix equation

\[
\begin{bmatrix}x^2\\y^2\end{bmatrix}
-3\begin{bmatrix}x\\2y\end{bmatrix}
=\begin{bmatrix}-2\\9\end{bmatrix}.
\]

**Solution:** We have

\[
\begin{bmatrix}x^2\\y^2\end{bmatrix}
-3\begin{bmatrix}x\\2y\end{bmatrix}
=\begin{bmatrix}-2\\9\end{bmatrix}
\Rightarrow
\begin{bmatrix}x^2\\y^2\end{bmatrix}
-\begin{bmatrix}3x\\6y\end{bmatrix}
=\begin{bmatrix}-2\\9\end{bmatrix}.
\]

\[
\begin{bmatrix}x^2-3x\\y^2-6y\end{bmatrix}
=\begin{bmatrix}-2\\9\end{bmatrix}.
\]

Thus,

\[
x^2-3x=-2\quad(1),\qquad y^2-6y=9\quad(2).
\]

From (1):

\[
x^2-3x+2=0\Rightarrow(x-1)(x-2)=0\Rightarrow x=1,2.
\]

From (2):

\[
y^2-6y-9=0\Rightarrow y^2-6y+9=0-9+9
\Rightarrow(y-3)^2=9.
\]

\[
y-3=\pm3\Rightarrow y=3\pm3\Rightarrow y=6,0.
\]

Therefore, \(x=1,2\) and \(y=6,0\).

---

## Page 9 — Find Matrices \(X\) and \(Y\)

**Question:** Find \(X\) and \(Y\) if

\[
2X+Y=\begin{bmatrix}4&4&7\\7&3&4\end{bmatrix}
\quad\text{and}\quad
X-2Y=\begin{bmatrix}-3&2&1\\1&-1&2\end{bmatrix}.
\]

**Solution:** We have

\[
2X+Y=\begin{bmatrix}4&4&7\\7&3&4\end{bmatrix}\quad(1)
\]

and

\[
X-2Y=\begin{bmatrix}-3&2&1\\1&-1&2\end{bmatrix}\quad(2).
\]

\((1)\times2\):

\[
4X+2Y=2\begin{bmatrix}4&4&7\\7&3&4\end{bmatrix}
=\begin{bmatrix}8&8&14\\14&6&8\end{bmatrix}\quad(3).
\]

\((2)+(3)\):

\[
5X=\begin{bmatrix}-3&2&1\\1&-1&2\end{bmatrix}
+\begin{bmatrix}8&8&14\\14&6&8\end{bmatrix}
=\begin{bmatrix}5&10&15\\15&5&10\end{bmatrix}.
\]

\[
X=\frac15\begin{bmatrix}5&10&15\\15&5&10\end{bmatrix}
=\begin{bmatrix}1&2&3\\3&1&2\end{bmatrix}.
\]

Putting the value of \(X\) in (1), we get

\[
\begin{aligned}
Y&=\begin{bmatrix}4&4&7\\7&3&4\end{bmatrix}-2X\\
&=\begin{bmatrix}4&4&7\\7&3&4\end{bmatrix}
-2\begin{bmatrix}1&2&3\\3&1&2\end{bmatrix}\\
&=\begin{bmatrix}4&4&7\\7&3&4\end{bmatrix}
-\begin{bmatrix}2&4&6\\6&2&4\end{bmatrix}
=\begin{bmatrix}2&0&1\\1&1&0\end{bmatrix}.
\end{aligned}
\]

Therefore,

\[
X=\begin{bmatrix}1&2&3\\3&1&2\end{bmatrix},\qquad
Y=\begin{bmatrix}2&0&1\\1&1&0\end{bmatrix}.
\]

---

## Page 10 — Multiplication of Matrices

Let \(A\) be of order \(m_1\times n_1\) and \(B\) be of order \(m_2\times n_2\). For multiplication, \(n_1\) should be the same as \(m_2\).

**Multiplication \(AB\) possible if:** No. of col in A = No. of Row B.

### (a)

\[
A=\begin{bmatrix}4&7\\6&2\end{bmatrix}_{2\times2},\qquad
B=\begin{bmatrix}1&8\\3&7\end{bmatrix}_{2\times2}.
\]

\[
AB=\begin{bmatrix}
4\times1+7\times3&4\times8+7\times7\\
6\times1+2\times3&6\times8+2\times7
\end{bmatrix}
=\begin{bmatrix}4+21&32+49\\6+6&48+14\end{bmatrix}
=\begin{bmatrix}25&81\\12&62\end{bmatrix}.
\]

### (b)

\[
A=\begin{bmatrix}1\\1\end{bmatrix}_{2\times1},\qquad
B=\begin{bmatrix}2\\4\end{bmatrix}_{2\times1}.
\]

No. of col of A \(\ne\) No. of Row B. **AB not possible.**

### (c)

\[
A=\begin{bmatrix}7&8\\9&8\\6&5\end{bmatrix}_{3\times2},\qquad
B=\begin{bmatrix}1&5&7\\0&6&8\end{bmatrix}_{2\times3}.
\]

\[
AB=\begin{bmatrix}
7\times1+8\times0&7\times5+8\times6&7\times7+8\times8\\
9\times1+8\times0&9\times5+8\times6&9\times7+8\times8\\
6\times1+5\times0&6\times5+5\times6&6\times7+5\times8
\end{bmatrix}
\]

\[
=\begin{bmatrix}
7&35+48&49+64\\
9&45+48&63+64\\
6&30+30&42+40
\end{bmatrix}
=\begin{bmatrix}7&83&113\\9&93&127\\6&60&82\end{bmatrix}.
\]

**Note:** It is not necessary \(AB=BA\).

For the example at the bottom of the page, \(A\) is \(2\times3\) and \(B\) is \(3\times4\); \(AB\) is \(2\times4\), while \(BA\) is not defined.

**Points to Remember:**

- In \(AB\), the number of columns of \(A\) must be equal to the number of rows of \(B\).
- In \(BA\), the number of columns of \(B\) must be equal to the number of rows of \(A\).

---

## Page 11 — Positive Integral Powers of Matrices

\[
A=\begin{bmatrix}2&-1\\3&2\end{bmatrix}.
\]

\[
A^2=A\cdot A
=\begin{bmatrix}2&-1\\3&2\end{bmatrix}
\begin{bmatrix}2&-1\\3&2\end{bmatrix}.
\]

\[
=\begin{bmatrix}
2\times2+(-1)\times3&2\times(-1)+(-1)\times2\\
3\times2+2\times3&3\times(-1)+2\times2
\end{bmatrix}
=\begin{bmatrix}4-3&-2-2\\6+6&-3+4\end{bmatrix}
=\begin{bmatrix}1&-4\\12&1\end{bmatrix}.
\]

Therefore,

\[
A^2=\begin{bmatrix}1&-4\\12&1\end{bmatrix}.
\]

\[
A^3=A^2\cdot A
=\begin{bmatrix}1&-4\\12&1\end{bmatrix}
\begin{bmatrix}2&-1\\3&2\end{bmatrix}
=\begin{bmatrix}2-12&-1-8\\24+3&-12+2\end{bmatrix}
=\begin{bmatrix}-10&-9\\27&-10\end{bmatrix}.
\]

Therefore,

\[
A^3=\begin{bmatrix}-10&-9\\27&-10\end{bmatrix}.
\]

\[
\boxed{A^3=A^2\cdot A\quad\text{or}\quad A\cdot A^2.}
\]

---

## Page 12 — Matrix Polynomial and Higher Powers

**Question:** Let

\[
A=\begin{bmatrix}2&3\\-1&2\end{bmatrix}
\quad\text{and}\quad f(x)=x^2-4x+7,
\]

show that \(f(A)=0\). Using this result, find \(A^5\).

**Solution:** We have

\[
A=\begin{bmatrix}2&3\\-1&2\end{bmatrix}.
\]

\(f(x)=x^2-4x+7\) implies \(f(A)=A^2-4A+7I_2\).

\[
f(A)=\begin{bmatrix}2&3\\-1&2\end{bmatrix}^2
-4\begin{bmatrix}2&3\\-1&2\end{bmatrix}
+7\begin{bmatrix}1&0\\0&1\end{bmatrix}.
\]

\[
=\begin{bmatrix}2&3\\-1&2\end{bmatrix}
\begin{bmatrix}2&3\\-1&2\end{bmatrix}
-\begin{bmatrix}8&12\\-4&8\end{bmatrix}
+\begin{bmatrix}7&0\\0&7\end{bmatrix}.
\]

\[
=\begin{bmatrix}4-3&6+6\\-2-2&-3+4\end{bmatrix}
-\begin{bmatrix}8&12\\-4&8\end{bmatrix}
+\begin{bmatrix}7&0\\0&7\end{bmatrix}
=\begin{bmatrix}1&12\\-4&1\end{bmatrix}
-\begin{bmatrix}8&12\\-4&8\end{bmatrix}
+\begin{bmatrix}7&0\\0&7\end{bmatrix}.
\]

\[
=\begin{bmatrix}1-8+7&12-12+0\\-4+4+0&1-8+7\end{bmatrix}
=\begin{bmatrix}0&0\\0&0\end{bmatrix}=0.
\]

Therefore, \(f(A)=0\), i.e.

\[
A^2-4A+7I_2=0,\qquad\text{i.e. }A^2=4A-7I_2.
\]

\[
\begin{aligned}
A^3&=A\cdot A^2=A(4A-7I_2)=4A^2-7A\\
&=4(4A-7I_2)-7A=9A-28I_2,\\[3pt]
A^4&=AA^3=A(9A-28I_2)=9A^2-28A\\
&=9(4A-7I_2)-28A=8A-63I_2,\\[3pt]
A^5&=AA^4=A(8A-63I_2)=8A^2-63A\\
&=8(4A-7I_2)-63A=-31A-56I_2.
\end{aligned}
\]

Therefore,

\[
A^5=-31\begin{bmatrix}2&3\\-1&2\end{bmatrix}
-56\begin{bmatrix}1&0\\0&1\end{bmatrix}
\]

\[
=\begin{bmatrix}-62&-93\\31&-62\end{bmatrix}
-\begin{bmatrix}56&0\\0&56\end{bmatrix}
=\begin{bmatrix}-118&-93\\31&-118\end{bmatrix}.
\]
---

## Page 13 — Special Square Matrices

**Note:** A square matrix \(A\) is said to be an **idempotent matrix** if \(A^2=A\).

A square matrix \(A\) is said to be an **involutory matrix** if \(A^2=I\).

A square matrix \(A\) is said to be a **nilpotent matrix** if there exists \(m\in\mathbb N\) such that \(A^m=0\).

If \(m\) is the least natural number such that \(A^m=0\), then \(m\) is called the **index of nilpotent matrix** \(A\).

---

## Page 14 — Matrix Power Example and Idempotent Matrix

### Question 1

If

\[
A=\begin{bmatrix}2&-1\\3&2\end{bmatrix},\qquad
B=\begin{bmatrix}0&4\\-1&7\end{bmatrix},
\]

find \(3A^2-2B\).

**Solution:**

\[
A^2=AA=
\begin{bmatrix}2&-1\\3&2\end{bmatrix}
\begin{bmatrix}2&-1\\3&2\end{bmatrix}
=\begin{bmatrix}4-3&-2-2\\6+6&-3+4\end{bmatrix}
=\begin{bmatrix}1&-4\\12&1\end{bmatrix}.
\]

\[
\begin{aligned}
3A^2-2B&=3\begin{bmatrix}1&-4\\12&1\end{bmatrix}
-2\begin{bmatrix}0&4\\-1&7\end{bmatrix}\\
&=\begin{bmatrix}3&-12\\36&3\end{bmatrix}
-\begin{bmatrix}0&8\\-2&14\end{bmatrix}\\
&=\begin{bmatrix}3-0&-12-8\\36+2&3-14\end{bmatrix}
=\begin{bmatrix}3&-20\\38&-11\end{bmatrix}.
\end{aligned}
\]

### Question 2

Show that the matrix

\[
A=\begin{bmatrix}2&-2&-4\\-1&3&4\\1&-2&-3\end{bmatrix}
\]

is idempotent.

**Solution:** Matrix \(A\) is idempotent if \(A^2=A\).

\[
A^2=AA=
\begin{bmatrix}2&-2&-4\\-1&3&4\\1&-2&-3\end{bmatrix}
\begin{bmatrix}2&-2&-4\\-1&3&4\\1&-2&-3\end{bmatrix}.
\]

\[
=\begin{bmatrix}
4+2-4&-4-6+8&-8-8+12\\
-2-3+4&2+9-8&4+12-12\\
2+2-3&-2-6+6&-4-8+9
\end{bmatrix}
=\begin{bmatrix}2&-2&-4\\-1&3&4\\1&-2&-3\end{bmatrix}=A.
\]

Therefore, matrix \(A\) is idempotent.

---

## Page 15 — Transpose of a Matrix

### Transpose of a Matrix

Example (i):

\[
A=\begin{bmatrix}2&3&6&8\\5&-3&-7&4\\9&8&2&1\end{bmatrix}_{3\times4}
\quad\Rightarrow\quad
A'=\begin{bmatrix}2&5&9\\3&-3&8\\6&-7&2\\8&4&1\end{bmatrix}_{4\times3}.
\]

Example (ii):

\[
A=\begin{bmatrix}5\\9\\0\end{bmatrix}_{3\times1},
\qquad A'=\begin{bmatrix}5&9&0\end{bmatrix}_{1\times3}.
\]

### Properties of Transpose

\[
(A')'=A,
\]

\[
(A+B)'=A'+B',
\]

\[
(kA)'=kA',
\]

\[
(AB)'=B'A'.
\]

---

## Page 16 — Orthogonal Matrix

A square matrix \(A\) is said to be an **orthogonal matrix** if

\[
AA'=I=A'A.
\]

Let

\[
A=\frac1{\sqrt2}\begin{bmatrix}1&-1\\1&1\end{bmatrix},\qquad
A'=\frac1{\sqrt2}\begin{bmatrix}1&1\\-1&1\end{bmatrix}.
\]

Then

\[
AA'=\frac1{\sqrt2}\begin{bmatrix}1&-1\\1&1\end{bmatrix}
\frac1{\sqrt2}\begin{bmatrix}1&1\\-1&1\end{bmatrix}
=\frac12\begin{bmatrix}1+1&1-1\\1-1&1+1\end{bmatrix}
=\frac12\begin{bmatrix}2&0\\0&2\end{bmatrix}=I.
\]

And

\[
A'A=\frac1{\sqrt2}\begin{bmatrix}1&1\\-1&1\end{bmatrix}
\frac1{\sqrt2}\begin{bmatrix}1&-1\\1&1\end{bmatrix}
=\frac12\begin{bmatrix}1+1&-1+1\\-1+1&1+1\end{bmatrix}
=\frac12\begin{bmatrix}2&0\\0&2\end{bmatrix}=I.
\]

Therefore, \(AA'=I=A'A\), and \(A\) is an orthogonal matrix.

---

## Page 17 — Symmetric Matrix and Skew-Symmetric Matrix

### Symmetric Matrix

**Property:** A square matrix \(A\) is said to be symmetric if \(A'=A\).

**Example:**

\[
A=\begin{bmatrix}3&4&7\\4&9&8\\7&8&11\end{bmatrix}.
\]

\[
A'=\begin{bmatrix}3&4&7\\4&9&8\\7&8&11\end{bmatrix}=A.
\]

Therefore, \(A'=A\), and \(A\) is symmetric.

### Skew-Symmetric Matrix

**Property:** A square matrix \(A\) is said to be skew-symmetric if \(A'=-A\).

**Example:**

\[
A=\begin{bmatrix}0&9&-6\\-9&0&8\\6&-8&0\end{bmatrix}.
\]

\[
A'=\begin{bmatrix}0&-9&6\\9&0&-8\\-6&8&0\end{bmatrix}
=-\begin{bmatrix}0&9&-6\\-9&0&8\\6&-8&0\end{bmatrix}=-A.
\]

Therefore, \(A'=-A\), and \(A\) is skew-symmetric.

### In General

- If \(A\) is symmetric, then \(a_{ij}=a_{ji}\) for all \(i,j\).
- If \(A\) is skew-symmetric, then \(a_{ij}=-a_{ji}\) for all \(i,j\).

---

## Page 18 — Sums and Differences with the Transpose

**Question:** If

\[
A=\begin{bmatrix}2&4\\5&6\end{bmatrix},
\]

show that:

(i) \(A+A'\) is symmetric.  
(ii) \(A-A'\) is skew-symmetric.

**Solution:** We have

\[
A=\begin{bmatrix}2&4\\5&6\end{bmatrix},\qquad
A'=\begin{bmatrix}2&5\\4&6\end{bmatrix}.
\]

(i)

\[
A+A'=\begin{bmatrix}2&4\\5&6\end{bmatrix}
+\begin{bmatrix}2&5\\4&6\end{bmatrix}
=\begin{bmatrix}2+2&4+5\\5+4&6+6\end{bmatrix}
=\begin{bmatrix}4&9\\9&12\end{bmatrix}.
\]

\((A+A')'=A+A'\). Thus, \(A+A'\) is symmetric.

(ii)

\[
A-A'=\begin{bmatrix}2&4\\5&6\end{bmatrix}
-\begin{bmatrix}2&5\\4&6\end{bmatrix}
=\begin{bmatrix}2-2&4-5\\5-4&6-6\end{bmatrix}
=\begin{bmatrix}0&-1\\1&0\end{bmatrix}.
\]

\((A-A')'=-(A-A')\). Thus, \(A-A'\) is skew-symmetric.

---

## Page 19 — Express a Matrix as a Sum of Symmetric and Skew-Symmetric Matrices

**Question:** Express

\[
\begin{bmatrix}4&3&7\\6&5&-8\\1&2&6\end{bmatrix}
\]

as the sum of a symmetric matrix and a skew-symmetric matrix.

**Solution:** Let

\[
A=\begin{bmatrix}4&3&7\\6&5&-8\\1&2&6\end{bmatrix},\qquad
A'=\begin{bmatrix}4&6&1\\3&5&2\\7&-8&6\end{bmatrix}.
\]

\[
A+A'=\begin{bmatrix}8&9&8\\9&10&-6\\8&-6&12\end{bmatrix},
\qquad
A-A'=\begin{bmatrix}0&-3&6\\3&0&-10\\-6&10&0\end{bmatrix}.
\]

Now,

\[
\frac12(A+A')=\begin{bmatrix}4&\frac92&4\\\frac92&5&-3\\4&-3&6\end{bmatrix},
\]

which is symmetric, and

\[
\frac12(A-A')=\begin{bmatrix}0&-\frac32&3\\\frac32&0&-5\\-3&5&0\end{bmatrix},
\]

which is skew-symmetric.

Therefore,

\[
A=\frac12(A+A')+\frac12(A-A')
\]

\[
=\begin{bmatrix}4&\frac92&4\\\frac92&5&-3\\4&-3&6\end{bmatrix}
+\begin{bmatrix}0&-\frac32&3\\\frac32&0&-5\\-3&5&0\end{bmatrix}.
\]

---

## Page 20 — Determinants

### (i)

\[
A=\begin{bmatrix}2&-3\\4&9\end{bmatrix}.
\]

\[
|A|=\begin{vmatrix}2&-3\\4&9\end{vmatrix}
=18-(-12)=18+12=30.
\]

### (ii)

\[
A=\begin{bmatrix}1&2&3\\4&5&6\\7&8&9\end{bmatrix}.
\]

\[
|A|=\begin{vmatrix}1&2&3\\4&5&6\\7&8&9\end{vmatrix}
=1\begin{vmatrix}5&6\\8&9\end{vmatrix}
-2\begin{vmatrix}4&6\\7&9\end{vmatrix}
+3\begin{vmatrix}4&5\\7&8\end{vmatrix}.
\]

\[
=1(45-48)-2(36-42)+3(32-35)
=(-3)-2(-6)+3(-3)
=-3+12-9=9-9=0.
\]

---

## Page 21 — Minors and Co-Factors

Let

\[
A=\begin{bmatrix}4&3&8\\6&7&5\\3&1&2\end{bmatrix}.
\]

### Minors

\(M_{ij}\) = minor of element \(a_{ij}\).

\[
M_{11}=\begin{vmatrix}7&5\\1&2\end{vmatrix}=14-5=9.
\]

\[
M_{12}=\begin{vmatrix}6&5\\3&2\end{vmatrix}=12-15=-3.
\]

\[
M_{13}=\begin{vmatrix}6&7\\3&1\end{vmatrix}=6-21=-15.
\]

\[
M_{21}=\begin{vmatrix}3&8\\1&2\end{vmatrix}=6-8=-2.
\]

\[
M_{22}=\begin{vmatrix}4&8\\3&2\end{vmatrix}=8-24=-16.
\]

\[
M_{23}=\begin{vmatrix}4&3\\3&1\end{vmatrix}=4-9=-5.
\]

\[
M_{31}=\begin{vmatrix}3&8\\7&5\end{vmatrix}=15-56=-41.
\]

\[
M_{32}=\begin{vmatrix}4&8\\6&5\end{vmatrix}=20-48=-28.
\]

\[
M_{33}=\begin{vmatrix}4&3\\6&7\end{vmatrix}=28-18=10.
\]

**Matrix of Minors** \([M_{ij}]\):

\[
[M_{ij}]=\begin{bmatrix}9&-3&-15\\-2&-16&-5\\-41&-28&10\end{bmatrix}.
\]

### Cofactors

\(A_{ij}\) = co-factor of element \(a_{ij}=(-1)^{i+j}M_{ij}\).

\[
A_{11}=(-1)^{1+1}M_{11}=(+1)(9)=9.
\]

\[
A_{12}=(-1)^{1+2}M_{12}=(-1)(-3)=3.
\]

\[
A_{13}=(-1)^{1+3}M_{13}=(+1)(-15)=-15.
\]

\[
A_{21}=(-1)^{2+1}M_{21}=(-1)(-2)=2.
\]

\[
A_{22}=(-1)^{2+2}M_{22}=(+1)(-16)=-16.
\]

\[
A_{23}=(-1)^{2+3}M_{23}=(-1)(-5)=5.
\]

\[
A_{31}=(-1)^{3+1}M_{31}=(+1)(-41)=-41.
\]

\[
A_{32}=(-1)^{3+2}M_{32}=(-1)(-28)=28.
\]

\[
A_{33}=(-1)^{3+3}M_{33}=(+1)(10)=10.
\]

**Matrix of Co-factors** \([A_{ij}]\):

\[
[A_{ij}]=\begin{bmatrix}9&3&-15\\2&-16&5\\-41&28&10\end{bmatrix}.
\]

---

## Page 22 — Notes on Determinants

**Note 1:**

\[
\begin{vmatrix}0&1&4\\0&2&5\\0&3&6\end{vmatrix}=0.
\]

\[
\begin{vmatrix}0&0&0\\1&2&3\\4&5&6\end{vmatrix}=0.
\]

**2.** The value of determinant of a skew-symmetric matrix of odd order is always zero.

**3.**

\[
a_{11}A_{21}+a_{12}A_{22}+a_{13}A_{23}=0.
\]

The sum of the products of the elements of any row (respectively, column) of a determinant with the cofactors of the corresponding elements of any other row (respectively, column) is zero.

---

## Page 23 — Sarrus Rule

**Sarrus Rule** — [only for determinants of order three.]

\[
A=\begin{bmatrix}2&1&3\\5&3&7\\1&2&6\end{bmatrix}.
\]

\[
|A|=\begin{vmatrix}2&1&3\\5&3&7\\1&2&6\end{vmatrix}.
\]

\[
=(2)(3)(6)+(1)(7)(1)+(3)(5)(2)
-(1)(3)(1)-(2)(7)(2)-(6)(5)(1).
\]

\[
=36+7+30-9-28-30=6.
\]

### Sarrus Rule for 3×3 Determinant

- Repeat the first two columns on the right side.
- Multiply the elements of the three downward diagonals and add them.
- Multiply the elements of the three upward diagonals and subtract them.
- \(|A|=(\text{Sum of downward products})-(\text{Sum of upward products})\).

---

## Page 24 — Singular and Non-Singular Matrices

**Singular Matrix:** A square matrix is called a singular matrix if its determinant is zero.

**Non-Singular Matrix:** A square matrix is called a non-singular matrix if its determinant is not zero.

### (i)

\[
A=\begin{bmatrix}4&3\\6&9\end{bmatrix}.
\]

\[
|A|=\begin{vmatrix}4&3\\6&9\end{vmatrix}=36-18=18\ne0.
\]

\(A\) is non-singular.

### (ii)

\[
A=\begin{bmatrix}1&4&3\\6&8&-5\\2&8&6\end{bmatrix}.
\]

\[
|A|=1\begin{vmatrix}8&-5\\8&6\end{vmatrix}
-4\begin{vmatrix}6&-5\\2&6\end{vmatrix}
+3\begin{vmatrix}6&8\\2&8\end{vmatrix}
=88-184+96=0.
\]

\(A\) is singular.

---

## Page 25 — Cramer's Rule

### Cramer's Rule: Solution Cases

- If \(D\ne0\): **Unique Solution**
  \[
  x=\frac{D_1}{D},\quad y=\frac{D_2}{D},\quad z=\frac{D_3}{D}.
  \]
- If \(D=0\) and \(D_1,D_2,D_3\) are not all zero: **No Solution**.
- If \(D=0\) and \(D_1,D_2,D_3\) are all zero: **Infinitely many Solutions or no Solution**.

### Question

The source heading reads: “Solve the the Using Determinants, solve the following System of equations.” The question is to solve the following system of equations using determinants:

\[
x+y+2z=0,
\]
\[
x-2y+2z=0,
\]
\[
x-z=0.
\]

**Solution:** The equations are

\[
x+y+2z=0,\qquad x-2y+2z=0,\qquad x+0y-z=0.
\]

\[
D=\begin{vmatrix}1&1&2\\1&-2&2\\1&0&-1\end{vmatrix}
=1(2-0)-1(-1-2)+2(0+2)=2+3+4=9\ne0.
\]

Unique solution.

\[
D_1=\begin{vmatrix}0&1&2\\0&-2&2\\0&0&-1\end{vmatrix}=0,
\quad
D_2=\begin{vmatrix}1&0&2\\1&0&2\\1&0&-1\end{vmatrix}=0,
\quad
D_3=\begin{vmatrix}1&1&0\\1&-2&0\\1&0&0\end{vmatrix}=0.
\]

\[
x=\frac{D_1}{D}=\frac09=0,\quad
 y=\frac{D_2}{D}=\frac09=0,\quad
 z=\frac{D_3}{D}=\frac09=0.
\]

\[
\boxed{x=0,\ y=0,\ z=0.}
\]

**Unique Solution.**

---

## Page 26 — Properties of the Adjugate

**Note:** If \(A\) is a square matrix of order \(n\), then

\[
A(\operatorname{adj}A)=(\operatorname{adj}A)A=|A|I_n.
\]

1. \(|\operatorname{adj}A|=|A|^{n-1}\).
2. \(\operatorname{adj}(\operatorname{adj}A)=|A|^{n-2}A\).
3. \(\operatorname{adj}A=(\operatorname{adj}A)'\).

---

## Page 27 — Inverse of a Matrix

**Step 1:** Find the value of \(|A|\).

**Step 2:** If \(|A|=0\), then \(A\) cannot have its inverse.

**Step 3:** If \(|A|\ne0\), then \(A\) has its inverse and is given by

\[
A^{-1}=\frac{\operatorname{adj}A}{|A|}.
\]

**Step 4:** Find cofactors of all elements of \(A\) and compute \(\operatorname{adj}A\).

**Step 5:** Compute \(\operatorname{adj}A\) (transpose of cofactor matrix).

**Step 6:** Multiply \(\operatorname{adj}A\) by \(\frac1{|A|}\). That is,

\[
A^{-1}=\frac1{|A|}(\operatorname{adj}A).
\]

**Step 7:** The result obtained is \(A^{-1}\).

---

## Page 28 — Find the Inverse and Verify the Result

**Question:** Find the inverse of the matrix

\[
A=\begin{bmatrix}1&-1&2\\0&2&-3\\3&-2&4\end{bmatrix}
\]

and verify the result.

**Solution:** Let

\[
A=\begin{bmatrix}1&-1&2\\0&2&-3\\3&-2&4\end{bmatrix}.
\]

\[
|A|=\begin{vmatrix}1&-1&2\\0&2&-3\\3&-2&4\end{vmatrix}
=1(8-6)+1(0+9)+2(0-6)=2+9-12=-1\ne0.
\]

Therefore, \(A\) is invertible and

\[
A^{-1}=\frac{\operatorname{adj}A}{|A|}.
\]

### We find \(\operatorname{adj}A\)

\[
A_{11}=+\begin{vmatrix}2&-3\\-2&4\end{vmatrix}=2,
\quad A_{12}=-\begin{vmatrix}0&-3\\3&4\end{vmatrix}=-9,
\quad A_{13}=+\begin{vmatrix}0&2\\3&-2\end{vmatrix}=-6.
\]

\[
A_{21}=-\begin{vmatrix}-1&2\\-2&4\end{vmatrix}=0,
\quad A_{22}=+\begin{vmatrix}1&2\\3&4\end{vmatrix}=-2,
\quad A_{23}=-\begin{vmatrix}1&-1\\3&-2\end{vmatrix}=-1.
\]

\[
A_{31}=+\begin{vmatrix}-1&2\\2&-3\end{vmatrix}=-1,
\quad A_{32}=-\begin{vmatrix}1&2\\0&-3\end{vmatrix}=3,
\quad A_{33}=+\begin{vmatrix}1&-1\\0&2\end{vmatrix}=2.
\]

Therefore, as shown in the source,

\[
\operatorname{adj}A=\begin{bmatrix}2&0&-1\\-9&-2&3\\-6&-1&2\end{bmatrix}.
\]

Hence,

\[
A^{-1}=\frac{\operatorname{adj}A}{|A|}
=\frac1{-1}\begin{bmatrix}2&0&-1\\-9&-2&3\\-6&-1&2\end{bmatrix}
=\begin{bmatrix}-2&0&1\\9&2&-3\\6&1&-2\end{bmatrix}.
\]

### Verification

\[
AA^{-1}=\begin{bmatrix}1&-1&2\\0&2&-3\\3&-2&4\end{bmatrix}
\begin{bmatrix}-2&0&1\\9&2&-3\\6&1&-2\end{bmatrix}.
\]

\[
=\begin{bmatrix}
-2-9+12&0-2+2&1+3-4\\
0+18-18&0+4-3&0-6+6\\
-6-18+24&0-4+4&-3+6-8
\end{bmatrix}
=\begin{bmatrix}1&0&0\\0&1&0\\0&0&1\end{bmatrix}=I.
\]

Similarly, it can be verified that \(A^{-1}A=I\).

---

## Page 29 — Further Properties of Inverses and Adjugates

**Note**

1. \((A^{-1})^{-1}=A\).
2. \((A')^{-1}=(A^{-1})'\).
3. \((\operatorname{adj}A)^{-1}=\operatorname{adj}(A^{-1})\).
4. \((AB)^{-1}=B^{-1}A^{-1}\).
5. \(\operatorname{adj}(AB)=(\operatorname{adj}B)(\operatorname{adj}A)\).

---

## Page 30 — Solution of System of Linear Equations by Matrix Method

**System:** \(AX=B\).

Find \(|A|\).

- If \(|A|\ne0\): **Unique solution**, \(X=A^{-1}B\).
- If \(|A|=0\): find \((\operatorname{adj}A)B\).
  - If \((\operatorname{adj}A)B\ne0\): **No solution**.
  - If \((\operatorname{adj}A)B=0\): **Infinitely many solutions or no solution**.

---

## Page 31 — Solve the Equations by Matrix Method

**Question:** Solve the equations:

\[
x+2y+z=7,\qquad x+3z=11,\qquad 2x-3y=1.
\]

**Solution:** The given equations are

\[
x+2y+z=7,
\]
\[
x+0y+3z=11,
\]
\[
2x-3y+0z=1.
\]

Let

\[
A=\begin{bmatrix}1&2&1\\1&0&3\\2&-3&0\end{bmatrix},\quad
X=\begin{bmatrix}x\\y\\z\end{bmatrix},\quad
B=\begin{bmatrix}7\\11\\1\end{bmatrix};\qquad AX=B.
\]

\[
|A|=\begin{vmatrix}1&2&1\\1&0&3\\2&-3&0\end{vmatrix}
=1(9)-2(-6)+1(-3)=18\ne0.
\]

Therefore, the system has unique solution \(X=A^{-1}B\).

For \(A\), we have

\[
\begin{aligned}
A_{11}&=0+9=9, & A_{12}&=-(0-6)=6, & A_{13}&=-3-0=-3,\\
A_{21}&=-(0+3)=-3, & A_{22}&=0-2=-2, & A_{23}&=-(-3-4)=7,\\
A_{31}&=6-0=6, & A_{32}&=-(3-1)=-2, & A_{33}&=0-2=-2.
\end{aligned}
\]

\[
\operatorname{adj}A=
\begin{bmatrix}9&6&-3\\-3&-2&7\\6&-2&-2\end{bmatrix}'
=\begin{bmatrix}9&-3&6\\6&-2&-2\\-3&7&-2\end{bmatrix}.
\]

\[
A^{-1}=\frac{\operatorname{adj}A}{|A|}
=\frac1{18}\begin{bmatrix}9&-3&6\\6&-2&-2\\-3&7&-2\end{bmatrix}.
\]

The solution is \(X=A^{-1}B\).

\[
\begin{bmatrix}x\\y\\z\end{bmatrix}
=\frac1{18}\begin{bmatrix}9&-3&6\\6&-2&-2\\-3&7&-2\end{bmatrix}
\begin{bmatrix}7\\11\\1\end{bmatrix}
=\frac1{18}\begin{bmatrix}63-33+6\\42-22-2\\-21+77-2\end{bmatrix}
=\frac1{18}\begin{bmatrix}36\\18\\54\end{bmatrix}
=\begin{bmatrix}2\\1\\3\end{bmatrix}.
\]

Therefore, \(x=2,\ y=1,\ z=3\).

---

## Page 32 — Solve the Equations with Reciprocals by Matrix Method

**Question:** Solve the equations:

\[
\frac2x+\frac3y+\frac{10}{z}=4,\qquad
\frac4x-\frac6y+\frac5z=1,\qquad
\frac6x+\frac9y-\frac{20}{z}=2.
\]

**Solution:** The given equations are

\[
2\left(\frac1x\right)+3\left(\frac1y\right)+10\left(\frac1z\right)=4\quad(1)
\]

\[
4\left(\frac1x\right)-6\left(\frac1y\right)+5\left(\frac1z\right)=1\quad(2)
\]

\[
6\left(\frac1x\right)+9\left(\frac1y\right)-20\left(\frac1z\right)=2\quad(3)
\]

Let

\[
A=\begin{bmatrix}2&3&10\\4&-6&5\\6&9&-20\end{bmatrix},\quad
X=\begin{bmatrix}1/x\\1/y\\1/z\end{bmatrix},\quad
B=\begin{bmatrix}4\\1\\2\end{bmatrix};\qquad AX=B.
\]

\[
|A|=\begin{vmatrix}2&3&10\\4&-6&5\\6&9&-20\end{vmatrix}
=2(120+45)-3(-80-30)+10(36+36)
\]

\[
=2(165)-3(-140)+10(72)=330+330+720=1380\ne0.
\]

Therefore, the system has unique solution \(X=A^{-1}B\).

For \(A\), we have

\[
\begin{aligned}
A_{11}&=(120+45)=165,& A_{12}&=-(-80-30)=110,& A_{13}&=(36+36)=72,\\
A_{21}&=-(-60-50)=110,& A_{22}&=(-40-60)=-100,& A_{23}&=-(-40-36)=76,\\
A_{31}&=(-18+24)=6,& A_{32}&=-(-40+20)=20,& A_{33}&=(-24-12)=-36.
\end{aligned}
\]

\[
\operatorname{adj}A=
\begin{bmatrix}165&110&72\\110&-100&76\\6&20&-36\end{bmatrix}'
=\begin{bmatrix}165&110&6\\110&-100&20\\72&76&-36\end{bmatrix}.
\]

\[
A^{-1}=\frac1{1380}\begin{bmatrix}165&110&6\\110&-100&20\\72&76&-36\end{bmatrix}.
\]

The solution is \(X=A^{-1}B\).

\[
\begin{bmatrix}1/x\\1/y\\1/z\end{bmatrix}
=\frac1{1380}\begin{bmatrix}165&110&6\\110&-100&20\\72&76&-36\end{bmatrix}
\begin{bmatrix}4\\1\\2\end{bmatrix}
=\frac1{1380}\begin{bmatrix}660+110+12\\440-100+40\\288+76-72\end{bmatrix}
=\frac1{1380}\begin{bmatrix}782\\380\\292\end{bmatrix}.
\]

The source then states:

\[
\frac1x=\frac{782}{1380}=\frac{17}{30},\qquad
\frac1y=\frac{380}{1380}=\frac{19}{69},\qquad
\frac1z=\frac{292}{1380}=\frac{73}{345}.
\]

Therefore, the printed answer is

\[
\boxed{x=\frac{30}{17},\quad y=\frac{69}{19},\quad z=\frac{345}{73}.}
\]

---

## Page 33 — Reciprocal Equations, Substitution, and Matrix Method

**Question:** Solve the equations:

\[
\frac2x+\frac3y+\frac{10}{z}=4,\qquad
\frac4x-\frac6y+\frac5z=1,\qquad
\frac6x+\frac9y-\frac{20}{z}=2.
\]

**Solution:** The given equations are

\[
2\left(\frac1x\right)+3\left(\frac1y\right)+10\left(\frac1z\right)=4,
\]

\[
4\left(\frac1x\right)-6\left(\frac1y\right)+5\left(\frac1z\right)=1,
\]

\[
6\left(\frac1x\right)+9\left(\frac1y\right)-20\left(\frac1z\right)=2.
\]

Let

\[
u=\frac1x,\qquad v=\frac1y,\qquad w=\frac1z.
\]

Then the equations become

\[
2u+3v+10w=4,
\]

\[
4u-6v+5w=1,
\]

\[
6u+9v-20w=2.
\]

Let

\[
A=\begin{bmatrix}2&3&10\\4&-6&5\\6&9&-20\end{bmatrix},\quad
X=\begin{bmatrix}u\\v\\w\end{bmatrix},\quad
B=\begin{bmatrix}4\\1\\2\end{bmatrix};\qquad AX=B.
\]

\[
|A|=\begin{vmatrix}2&3&10\\4&-6&5\\6&9&-20\end{vmatrix}
=2(120-45)-3(-80-30)+10(36+36)
\]

\[
=2(75)-3(-110)+10(72)=150+330+720=1200\ne0.
\]

Therefore, the system has unique solution \(X=A^{-1}B\).

For \(A\), we have

\[
\begin{aligned}
A_{11}&=120,& A_{12}&=-80,& A_{13}&=36,\\
A_{21}&=-45,& A_{22}&=75,& A_{23}&=-36,\\
A_{31}&=45,& A_{32}&=-30,& A_{33}&=-18.
\end{aligned}
\]

\[
\operatorname{adj}A=
\begin{bmatrix}120&-45&45\\-80&75&-30\\36&-36&-18\end{bmatrix}'
=\begin{bmatrix}120&-80&36\\-45&75&-36\\45&-30&-18\end{bmatrix}.
\]

\[
A^{-1}=\frac1{1200}
\begin{bmatrix}120&-80&36\\-45&75&-36\\45&-30&-18\end{bmatrix}.
\]

The solution is \(X=A^{-1}B\).

\[
\begin{bmatrix}u\\v\\w\end{bmatrix}
=\frac1{1200}
\begin{bmatrix}120&-80&36\\-45&75&-36\\45&-30&-18\end{bmatrix}
\begin{bmatrix}4\\1\\2\end{bmatrix}
=\frac1{1200}\begin{bmatrix}480-80+72\\-180+75-72\\180-30-36\end{bmatrix}
=\frac1{1200}\begin{bmatrix}472\\-177\\114\end{bmatrix}.
\]

Therefore,

\[
u=\frac{59}{150},\qquad v=-\frac{59}{400},\qquad w=\frac{19}{200}.
\]

That is,

\[
\frac1x=\frac{59}{150},\qquad \frac1y=-\frac{59}{400},\qquad \frac1z=\frac{19}{200}.
\]

Therefore,

\[
\boxed{x=\frac{150}{59},\quad y=-\frac{400}{59},\quad z=\frac{200}{19}.}
\]

---

## End of Transcription

**Transcription fidelity note:** This file follows the supplied PDF and preserves its stated answers, including any arithmetic or notation that may be inconsistent within the source. It does not silently replace the source's printed results with independently corrected answers.
