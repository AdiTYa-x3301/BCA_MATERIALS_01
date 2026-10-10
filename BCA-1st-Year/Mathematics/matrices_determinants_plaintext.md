# Matrices and Determinants — Full Page-by-Page Transcription

**Source:** *Matrices Determinants One Shot.pdf* (33 pages; author metadata: Manpreet Singh).  
**Transcription note:** Page order and all visible lesson headings, definitions, questions, examples, and worked solutions are retained. Mathematical expressions and matrices have been typeset for readability; layout and line breaks may differ from the scan. The repeated diagonal watermark on the pages reads **DREAM MATHS**.

---

## Page 1 — MATRICES

### Examples of Matrices

1. [1 2 3; 0 6 8] — order 2×3
2. [1 5 4; 7 8 9; 3 9 7] — order 3×3
3. [1; 6; 7; 8] — order 4×1
4. [x²+1 4x-2; x³ x-3] — order 2×2

### Order of a Matrix

The order of a matrix is defined as:

**No. of Rows × No. of Cols.**

Examples:

- [1 2 3; 0 6 8]→ 2×3
- [1 5 4; 7 8 9; 3 9 7]→ 3×3
- [1; 6; 7; 8]→ 4×1
- [x²+1 4x-2; x³ x-3]→ 2×2

### Elements of a Matrix

Let

A=[1 5 4; 7 8 9; 3 9 7].

The elements of A are denoted by a_ij, where i = row number and j = column number.

a_11=1 a_12=5 a_13=4; a_21=7 a_22=8 a_23=9; a_31=3 a_32=9 a_33=7

---

## Page 2 — Construct a Matrix

**Question:** Construct a 3×4 matrix A=[a_ij], whose element a_ij is given by

a_ij=(i+j)²/2, 1≤ i≤3, 1≤ j≤4.

**Solution:** We have

a_ij=(i+j)²/2, 1≤ i≤3, 1≤ j≤4.

To find a_11, put i=1,j=1 in a_ij:

a_11=(1+1)²/2=(2²)/2=4/2=2.

To find a_12, put i=1,j=2 in a_ij:

a_12=(1+2)²/2=(3²)/2=9/2.

To find a_13, put i=1,j=3 in a_ij:

a_13=(1+3)²/2=(4²)/2=16/2=8.

To find a_14, put i=1,j=4 in a_ij:

a_14=(1+4)²/2=(5²)/2=25/2.

To find a_21, put i=2,j=1 in a_ij:

a_21=(2+1)²/2=(3²)/2=9/2.

To find a_22, put i=2,j=2 in a_ij:

a_22=(2+2)²/2=(4²)/2=16/2=8.

To find a_23, put i=2,j=3 in a_ij:

a_23=(2+3)²/2=(5²)/2=25/2.

To find a_24, put i=2,j=4 in a_ij:

a_24=(2+4)²/2=(6²)/2=36/2=18.

To find a_31, put i=3,j=1 in a_ij:

a_31=(3+1)²/2=(4²)/2=16/2=8.

To find a_32, put i=3,j=2 in a_ij:

a_32=(3+2)²/2=(5²)/2=25/2.

To find a_33, put i=3,j=3 in a_ij:

a_33=(3+3)²/2=(6²)/2=36/2=18.

To find a_34, put i=3,j=4 in a_ij:

a_34=(3+4)²/2=(7²)/2=49/2.

Hence,

A=[2 9/2 8 25/2; 9/2 8 25/2 18; 8 25/2 18 49/2].

---

## Page 3 — Types of Matrices

| S. No. | Type of matrix | Definition | Example shown in the source |
|---|---|---|---|
| 1 | Square Matrix | A matrix is called a square matrix if the number of rows and columns in the matrix are equal. | [1 4 7; 2 5 2; 3 6 1], order 3×3 |
| 2 | Row Matrix | A matrix is called a row matrix if it contains only one row. | [1 5 4 3], order 1×4 |
| 3 | Column Matrix | A matrix is called a column matrix if it contains only one column. | [1; 4; 2], order 3×1 |
| 4 | Zero (or Null) Matrix | A matrix is called a zero matrix if all its elements are zero. It is denoted by ‘0’. | [0 0; 0 0], order 2×2 |
| 5 | Diagonal Matrix | A square matrix is called a diagonal matrix if all its non-diagonal elements are zero. | [1 0 0; 0 3 0; 0 0 6], order 3×3 |
| 6 | Scalar Matrix | A square matrix is called a scalar matrix if all its non-diagonal elements are zero and all diagonal elements are equal. | [4 0 0; 0 4 0; 0 0 4], order 3×3 |
| 7 | Unit Matrix or Identity Matrix | A square matrix is called a unit matrix if all its non-diagonal elements are zero and all diagonal elements are unity. | [1 0 0; 0 1 0; 0 0 1], order 3×3 |
| 8 | Triangular Matrices | A square matrix is called a triangular matrix if all its elements either below or above the principal diagonal are zero. | Upper and lower triangular examples below. |

**(i) Upper Triangular Matrix:** If all elements below the principal diagonal are zero.

Example: [1 2 3; 0 4 5; 0 0 7], order 3×3.

**(ii) Lower Triangular Matrix:** If all elements above the principal diagonal are zero.

Example: [1 0 0; 4 2 0; 5 6 3], order 3×3.

---

## Page 4 — Comparable and Equal Matrices

### 9. Comparable Matrices

Two matrices are called comparable if they are of the same order (i.e., they have the same number of rows and the same number of columns).

Example: Let

A=[1 2 3; 4 5 6], B=[7 8 9; 1 2 3].

A and B are comparable. (Both are of order 2×3.)

### 10. Equal Matrices

Two matrices are called equal matrices if they are of the same order and their corresponding elements are equal.

Example: Let

A=[2 3 4; 5 6 7], B=[2 3 4; 5 6 7].

A and B are equal matrices.

---

## Page 5 — Equality of Matrices: Finding x,y,z

**Question 1:** Find the values of x,y,z if

[2x+y x-y; x-z x+y+z] = [10 -1; 2 8].

**Solution:** By equality of matrices, corresponding elements are equal.

2x+y=10 (1); x-y=-1 (2); x-z=2 (3); x+y+z=8 (4)

(1)+(2):

(2x+y)+(x-y)=10+(-1), 3x=9, x=3.

From (2):

x-y=-1⇒3-y=-1⇒-y=-4⇒ y=4.

From (3):

x-z=2⇒3-z=2⇒-z=-1⇒ z=1.

Therefore, x=3, y=4, z=1.

### Question 2

If

[2x+1 2y; 0 y²+1] = [x+3 10; 0 26],

find the value of x+y.

**Solution:** By equality of matrices,

2x+1=x+3 (1), 2y=10 (2), y²+1=26 (3).

From (1): 2x+1=x+3⇒2x-x=3-1⇒ x=2.

From (2): 2y=10⇒ y=10/2⇒ y=5.

From (3): y²+1=26⇒ y²=25⇒ y=±5. But from (2), y=5.

Therefore, x+y=2+5=7.

---

## Page 6 — Equality of Matrices: Finding x,y

**Question:** For what values of x and y are the following matrices equal?

[2x+1 3y; 0 y²-5y], [x+3 y²+2; 0 -6].

**Solution:** For two matrices to be equal, their corresponding elements must be equal. Equating corresponding elements, we get:

2x+1=x+3 (1); 3y=y²+2 (2); 0=0 (3); y²-5y=-6 (4)

From (1):

2x+1=x+3⇒2x-x=3-1⇒ x=2.

From (2):

3y=y²+2⇒ y²-3y+2=0⇒(y-1)(y-2)=0,

so y=1 or y=2.

From (4):

y²-5y=-6⇒ y²-5y+6=0⇒(y-2)(y-3)=0,

so y=2 or y=3.

From both (2) and (4), the common value of y is y=2.

Therefore, x=2, y=2.

---

## Page 7 — Operations on Matrices

### 1. Addition of Matrices

Matrices should have same order.

A=[2 3 6; 4 0 9], B=[0 6 8; 7 0 8].

A+B=[2+0 3+6 6+8; 4+5 0+0 9+8] =[2 9 14; 11 0 17].

### 2. Subtraction of Matrices

Matrices should have same order.

A-B=[2-0 3-6 6-8; 4-7 0-0 9-8] =[2 -3 -2; -3 0 1].

### 3. Scalar Multiplication of Matrix

A=[4 7 3; 2 1 2], 3A=[3×4 3×7 3×3; 3×2 3×1 3×2] =[12 21 9; 6 3 6].

Another example shown:

B=[2 6 4; 8 12 8], 1/2B=[1 3 2; 4 6 4].

**Note:** In addition and subtraction, order must be same. In scalar multiplication, any scalar can be used.

---

## Page 8 — Solve the Matrix Equation

**Question:** Solve the matrix equation

[x²; y²] -3[x; 2y] =[-2; 9].

**Solution:** We have

[x²; y²] -3[x; 2y] =[-2; 9] ⇒ [x²; y²] -[3x; 6y] =[-2; 9].

[x²-3x; y²-6y] =[-2; 9].

Thus,

x²-3x=-2 (1), y²-6y=9 (2).

From (1):

x²-3x+2=0⇒(x-1)(x-2)=0⇒ x=1,2.

From (2):

y²-6y-9=0⇒ y²-6y+9=0-9+9 ⇒(y-3)²=9.

y-3=±3⇒ y=3±3⇒ y=6,0.

Therefore, x=1,2 and y=6,0.

---

## Page 9 — Find Matrices X and Y

**Question:** Find X and Y if

2X+Y=[4 4 7; 7 3 4] and X-2Y=[-3 2 1; 1 -1 2].

**Solution:** We have

2X+Y=[4 4 7; 7 3 4] (1)

and

X-2Y=[-3 2 1; 1 -1 2] (2).

(1)×2:

4X+2Y=2[4 4 7; 7 3 4] =[8 8 14; 14 6 8] (3).

(2)+(3):

5X=[-3 2 1; 1 -1 2] +[8 8 14; 14 6 8] =[5 10 15; 15 5 10].

X=1/5[5 10 15; 15 5 10] =[1 2 3; 3 1 2].

Putting the value of X in (1), we get

Y=[4 4 7; 7 3 4]-2X; =[4 4 7; 7 3 4] -2[1 2 3; 3 1 2]; =[4 4 7; 7 3 4] -[2 4 6; 6 2 4] =[2 0 1; 1 1 0].

Therefore,

X=[1 2 3; 3 1 2], Y=[2 0 1; 1 1 0].

---

## Page 10 — Multiplication of Matrices

Let A be of order m_1× n_1 and B be of order m_2× n_2. For multiplication, n_1 should be the same as m_2.

**Multiplication AB possible if:** No. of col in A = No. of Row B.

### (a)

A=[4 7; 6 2] (order 2×2), B=[1 8; 3 7] (order 2×2).

AB=[4×1+7×3 4×8+7×7; 6×1+2×3 6×8+2×7] =[4+21 32+49; 6+6 48+14] =[25 81; 12 62].

### (b)

A=[1; 1] (order 2×1), B=[2; 4] (order 2×1).

No. of col of A ≠ No. of Row B. **AB not possible.**

### (c)

A=[7 8; 9 8; 6 5] (order 3×2), B=[1 5 7; 0 6 8] (order 2×3).

AB=[7×1+8×0 7×5+8×6 7×7+8×8; 9×1+8×0 9×5+8×6 9×7+8×8; 6×1+5×0 6×5+5×6 6×7+5×8]

=[7 35+48 49+64; 9 45+48 63+64; 6 30+30 42+40] =[7 83 113; 9 93 127; 6 60 82].

**Note:** It is not necessary AB=BA.

For the example at the bottom of the page, A is 2×3 and B is 3×4; AB is 2×4, while BA is not defined.

**Points to Remember:**

- In AB, the number of columns of A must be equal to the number of rows of B.
- In BA, the number of columns of B must be equal to the number of rows of A.

---

## Page 11 — Positive Integral Powers of Matrices

A=[2 -1; 3 2].

A²=A· A =[2 -1; 3 2] [2 -1; 3 2].

=[2×2+(-1)×3 2×(-1)+(-1)×2; 3×2+2×3 3×(-1)+2×2] =[4-3 -2-2; 6+6 -3+4] =[1 -4; 12 1].

Therefore,

A²=[1 -4; 12 1].

A³=A²· A =[1 -4; 12 1] [2 -1; 3 2] =[2-12 -1-8; 24+3 -12+2] =[-10 -9; 27 -10].

Therefore,

A³=[-10 -9; 27 -10].

A³=A²· A or A· A².

---

## Page 12 — Matrix Polynomial and Higher Powers

**Question:** Let

A=[2 3; -1 2] and f(x)=x²-4x+7,

show that f(A)=0. Using this result, find A⁵.

**Solution:** We have

A=[2 3; -1 2].

f(x)=x²-4x+7 implies f(A)=A²-4A+7I_2.

f(A)=[2 3; -1 2]² -4[2 3; -1 2] +7[1 0; 0 1].

=[2 3; -1 2] [2 3; -1 2] -[8 12; -4 8] +[7 0; 0 7].

=[4-3 6+6; -2-2 -3+4] -[8 12; -4 8] +[7 0; 0 7] =[1 12; -4 1] -[8 12; -4 8] +[7 0; 0 7].

=[1-8+7 12-12+0; -4+4+0 1-8+7] =[0 0; 0 0]=0.

Therefore, f(A)=0, i.e.

A²-4A+7I_2=0, i.e.A²=4A-7I_2.

A³=A· A²=A(4A-7I_2)=4A²-7A; =4(4A-7I_2)-7A=9A-28I_2,; A⁴=AA³=A(9A-28I_2)=9A²-28A; =9(4A-7I_2)-28A=8A-63I_2,; A⁵=AA⁴=A(8A-63I_2)=8A²-63A; =8(4A-7I_2)-63A=-31A-56I_2.

Therefore,

A⁵=-31[2 3; -1 2] -56[1 0; 0 1]

=[-62 -93; 31 -62] -[56 0; 0 56] =[-118 -93; 31 -118].

---

## Page 13 — Special Square Matrices

**Note:** A square matrix A is said to be an **idempotent matrix** if A²=A.

A square matrix A is said to be an **involutory matrix** if A²=I.

A square matrix A is said to be a **nilpotent matrix** if there exists m∈mathbb N such that A^m=0.

If m is the least natural number such that A^m=0, then m is called the **index of nilpotent matrix** A.

---

## Page 14 — Matrix Power Example and Idempotent Matrix

### Question 1

If

A=[2 -1; 3 2], B=[0 4; -1 7],

find 3A²-2B.

**Solution:**

A²=AA= [2 -1; 3 2] [2 -1; 3 2] =[4-3 -2-2; 6+6 -3+4] =[1 -4; 12 1].

3A²-2B=3[1 -4; 12 1] -2[0 4; -1 7]; =[3 -12; 36 3] -[0 8; -2 14]; =[3-0 -12-8; 36+2 3-14] =[3 -20; 38 -11].

### Question 2

Show that the matrix

A=[2 -2 -4; -1 3 4; 1 -2 -3]

is idempotent.

**Solution:** Matrix A is idempotent if A²=A.

A²=AA= [2 -2 -4; -1 3 4; 1 -2 -3] [2 -2 -4; -1 3 4; 1 -2 -3].

=[4+2-4 -4-6+8 -8-8+12; -2-3+4 2+9-8 4+12-12; 2+2-3 -2-6+6 -4-8+9] =[2 -2 -4; -1 3 4; 1 -2 -3]=A.

Therefore, matrix A is idempotent.

---

## Page 15 — Transpose of a Matrix

### Transpose of a Matrix

Example (i):

A=[2 3 6 8; 5 -3 -7 4; 9 8 2 1] (order 3×4) ⇒ A'=[2 5 9; 3 -3 8; 6 -7 2; 8 4 1] (order 4×3).

Example (ii):

A=[5; 9; 0] (order 3×1), A'=[5 9 0] (order 1×3).

### Properties of Transpose

(A')'=A,

(A+B)'=A'+B',

(kA)'=kA',

(AB)'=B'A'.

---

## Page 16 — Orthogonal Matrix

A square matrix A is said to be an **orthogonal matrix** if

AA'=I=A'A.

Let

A=1/√(2)[1 -1; 1 1], A'=1/√(2)[1 1; -1 1].

Then

AA'=1/√(2)[1 -1; 1 1] 1/√(2)[1 1; -1 1] =1/2[1+1 1-1; 1-1 1+1] =1/2[2 0; 0 2]=I.

And

A'A=1/√(2)[1 1; -1 1] 1/√(2)[1 -1; 1 1] =1/2[1+1 -1+1; -1+1 1+1] =1/2[2 0; 0 2]=I.

Therefore, AA'=I=A'A, and A is an orthogonal matrix.

---

## Page 17 — Symmetric Matrix and Skew-Symmetric Matrix

### Symmetric Matrix

**Property:** A square matrix A is said to be symmetric if A'=A.

**Example:**

A=[3 4 7; 4 9 8; 7 8 11].

A'=[3 4 7; 4 9 8; 7 8 11]=A.

Therefore, A'=A, and A is symmetric.

### Skew-Symmetric Matrix

**Property:** A square matrix A is said to be skew-symmetric if A'=-A.

**Example:**

A=[0 9 -6; -9 0 8; 6 -8 0].

A'=[0 -9 6; 9 0 -8; -6 8 0] =-[0 9 -6; -9 0 8; 6 -8 0]=-A.

Therefore, A'=-A, and A is skew-symmetric.

### In General

- If A is symmetric, then a_ij=a_ji for all i,j.
- If A is skew-symmetric, then a_ij=-a_ji for all i,j.

---

## Page 18 — Sums and Differences with the Transpose

**Question:** If

A=[2 4; 5 6],

show that:

(i) A+A' is symmetric.  
(ii) A-A' is skew-symmetric.

**Solution:** We have

A=[2 4; 5 6], A'=[2 5; 4 6].

(i)

A+A'=[2 4; 5 6] +[2 5; 4 6] =[2+2 4+5; 5+4 6+6] =[4 9; 9 12].

(A+A')'=A+A'. Thus, A+A' is symmetric.

(ii)

A-A'=[2 4; 5 6] -[2 5; 4 6] =[2-2 4-5; 5-4 6-6] =[0 -1; 1 0].

(A-A')'=-(A-A'). Thus, A-A' is skew-symmetric.

---

## Page 19 — Express a Matrix as a Sum of Symmetric and Skew-Symmetric Matrices

**Question:** Express

[4 3 7; 6 5 -8; 1 2 6]

as the sum of a symmetric matrix and a skew-symmetric matrix.

**Solution:** Let

A=[4 3 7; 6 5 -8; 1 2 6], A'=[4 6 1; 3 5 2; 7 -8 6].

A+A'=[8 9 8; 9 10 -6; 8 -6 12], A-A'=[0 -3 6; 3 0 -10; -6 10 0].

Now,

1/2(A+A')=[4 9/2 4; 9/2 5 -3; 4 -3 6],

which is symmetric, and

1/2(A-A')=[0 -3/2 3; 3/2 0 -5; -3 5 0],

which is skew-symmetric.

Therefore,

A=1/2(A+A')+1/2(A-A')

=[4 9/2 4; 9/2 5 -3; 4 -3 6] +[0 -3/2 3; 3/2 0 -5; -3 5 0].

---

## Page 20 — Determinants

### (i)

A=[2 -3; 4 9].

|A|=det([2 -3; 4 9]) =18-(-12)=18+12=30.

### (ii)

A=[1 2 3; 4 5 6; 7 8 9].

|A|=det([1 2 3; 4 5 6; 7 8 9]) =1det([5 6; 8 9]) -2det([4 6; 7 9]) +3det([4 5; 7 8]).

=1(45-48)-2(36-42)+3(32-35) =(-3)-2(-6)+3(-3) =-3+12-9=9-9=0.

---

## Page 21 — Minors and Co-Factors

Let

A=[4 3 8; 6 7 5; 3 1 2].

### Minors

M_ij = minor of element a_ij.

M_11=det([7 5; 1 2])=14-5=9.

M_12=det([6 5; 3 2])=12-15=-3.

M_13=det([6 7; 3 1])=6-21=-15.

M_21=det([3 8; 1 2])=6-8=-2.

M_22=det([4 8; 3 2])=8-24=-16.

M_23=det([4 3; 3 1])=4-9=-5.

M_31=det([3 8; 7 5])=15-56=-41.

M_32=det([4 8; 6 5])=20-48=-28.

M_33=det([4 3; 6 7])=28-18=10.

**Matrix of Minors** [M_ij]:

[M_ij]=[9 -3 -15; -2 -16 -5; -41 -28 10].

### Cofactors

A_ij = co-factor of element a_ij=(-1)^(i+j)M_ij.

A_11=(-1)^¹⁺¹M_11=(+1)(9)=9.

A_12=(-1)^¹⁺²M_12=(-1)(-3)=3.

A_13=(-1)^¹⁺³M_13=(+1)(-15)=-15.

A_21=(-1)^²⁺¹M_21=(-1)(-2)=2.

A_22=(-1)^²⁺²M_22=(+1)(-16)=-16.

A_23=(-1)^²⁺³M_23=(-1)(-5)=5.

A_31=(-1)^³⁺¹M_31=(+1)(-41)=-41.

A_32=(-1)^³⁺²M_32=(-1)(-28)=28.

A_33=(-1)^³⁺³M_33=(+1)(10)=10.

**Matrix of Co-factors** [A_ij]:

[A_ij]=[9 3 -15; 2 -16 5; -41 28 10].

---

## Page 22 — Notes on Determinants

**Note 1:**

det([0 1 4; 0 2 5; 0 3 6])=0.

det([0 0 0; 1 2 3; 4 5 6])=0.

**2.** The value of determinant of a skew-symmetric matrix of odd order is always zero.

**3.**

a_11A_21+a_12A_22+a_13A_23=0.

The sum of the products of the elements of any row (respectively, column) of a determinant with the cofactors of the corresponding elements of any other row (respectively, column) is zero.

---

## Page 23 — Sarrus Rule

**Sarrus Rule** — [only for determinants of order three.]

A=[2 1 3; 5 3 7; 1 2 6].

|A|=det([2 1 3; 5 3 7; 1 2 6]).

=(2)(3)(6)+(1)(7)(1)+(3)(5)(2) -(1)(3)(1)-(2)(7)(2)-(6)(5)(1).

=36+7+30-9-28-30=6.

### Sarrus Rule for 3×3 Determinant

- Repeat the first two columns on the right side.
- Multiply the elements of the three downward diagonals and add them.
- Multiply the elements of the three upward diagonals and subtract them.
- |A|=(Sum of downward products)-(Sum of upward products).

---

## Page 24 — Singular and Non-Singular Matrices

**Singular Matrix:** A square matrix is called a singular matrix if its determinant is zero.

**Non-Singular Matrix:** A square matrix is called a non-singular matrix if its determinant is not zero.

### (i)

A=[4 3; 6 9].

|A|=det([4 3; 6 9])=36-18=18≠0.

A is non-singular.

### (ii)

A=[1 4 3; 6 8 -5; 2 8 6].

|A|=1det([8 -5; 8 6]) -4det([6 -5; 2 6]) +3det([6 8; 2 8]) =88-184+96=0.

A is singular.

---

## Page 25 — Cramer's Rule

### Cramer's Rule: Solution Cases

- If D≠0: **Unique Solution**
  

x=D_1/D, y=D_2/D, z=D_3/D.

- If D=0 and D_1,D_2,D_3 are not all zero: **No Solution**.
- If D=0 and D_1,D_2,D_3 are all zero: **Infinitely many Solutions or no Solution**.

### Question

The source heading reads: “Solve the the Using Determinants, solve the following System of equations.” The question is to solve the following system of equations using determinants:

x+y+2z=0,

x-2y+2z=0,

x-z=0.

**Solution:** The equations are

x+y+2z=0, x-2y+2z=0, x+0y-z=0.

D=det([1 1 2; 1 -2 2; 1 0 -1]) =1(2-0)-1(-1-2)+2(0+2)=2+3+4=9≠0.

Unique solution.

D_1=det([0 1 2; 0 -2 2; 0 0 -1])=0, D_2=det([1 0 2; 1 0 2; 1 0 -1])=0, D_3=det([1 1 0; 1 -2 0; 1 0 0])=0.

x=D_1/D=0/9=0, y=D_2/D=0/9=0, z=D_3/D=0/9=0.

x=0, y=0, z=0.

**Unique Solution.**

---

## Page 26 — Properties of the Adjugate

**Note:** If A is a square matrix of order n, then

A(adj(A))=(adj(A))A=|A|I_n.

1. |adj(A)|=|A|^(n-1).
2. adj(adj(A))=|A|^(n-2)A.
3. adj(A)=(adj(A))'.

---

## Page 27 — Inverse of a Matrix

**Step 1:** Find the value of |A|.

**Step 2:** If |A|=0, then A cannot have its inverse.

**Step 3:** If |A|≠0, then A has its inverse and is given by

A⁻¹=(adj(A))/|A|.

**Step 4:** Find cofactors of all elements of A and compute adj(A).

**Step 5:** Compute adj(A) (transpose of cofactor matrix).

**Step 6:** Multiply adj(A) by 1/|A|. That is,

A⁻¹=1/|A|(adj(A)).

**Step 7:** The result obtained is A⁻¹.

---

## Page 28 — Find the Inverse and Verify the Result

**Question:** Find the inverse of the matrix

A=[1 -1 2; 0 2 -3; 3 -2 4]

and verify the result.

**Solution:** Let

A=[1 -1 2; 0 2 -3; 3 -2 4].

|A|=det([1 -1 2; 0 2 -3; 3 -2 4]) =1(8-6)+1(0+9)+2(0-6)=2+9-12=-1≠0.

Therefore, A is invertible and

A⁻¹=(adj(A))/|A|.

### We find adj(A)

A_11=+det([2 -3; -2 4])=2, A_12=-det([0 -3; 3 4])=-9, A_13=+det([0 2; 3 -2])=-6.

A_21=-det([-1 2; -2 4])=0, A_22=+det([1 2; 3 4])=-2, A_23=-det([1 -1; 3 -2])=-1.

A_31=+det([-1 2; 2 -3])=-1, A_32=-det([1 2; 0 -3])=3, A_33=+det([1 -1; 0 2])=2.

Therefore, as shown in the source,

adj(A)=[2 0 -1; -9 -2 3; -6 -1 2].

Hence,

A⁻¹=(adj(A))/|A| =1/(-1)[2 0 -1; -9 -2 3; -6 -1 2] =[-2 0 1; 9 2 -3; 6 1 -2].

### Verification

AA⁻¹=[1 -1 2; 0 2 -3; 3 -2 4] [-2 0 1; 9 2 -3; 6 1 -2].

=[-2-9+12 0-2+2 1+3-4; 0+18-18 0+4-3 0-6+6; -6-18+24 0-4+4 -3+6-8] =[1 0 0; 0 1 0; 0 0 1]=I.

Similarly, it can be verified that A⁻¹A=I.

---

## Page 29 — Further Properties of Inverses and Adjugates

**Note**

1. (A⁻¹)⁻¹=A.
2. (A')⁻¹=(A⁻¹)'.
3. (adj(A))⁻¹=adj(A⁻¹).
4. (AB)⁻¹=B⁻¹A⁻¹.
5. adj(AB)=(adjB)(adj(A)).

---

## Page 30 — Solution of System of Linear Equations by Matrix Method

**System:** AX=B.

Find |A|.

- If |A|≠0: **Unique solution**, X=A⁻¹B.
- If |A|=0: find (adj(A))B.
  - If (adj(A))B≠0: **No solution**.
  - If (adj(A))B=0: **Infinitely many solutions or no solution**.

---

## Page 31 — Solve the Equations by Matrix Method

**Question:** Solve the equations:

x+2y+z=7, x+3z=11, 2x-3y=1.

**Solution:** The given equations are

x+2y+z=7,

x+0y+3z=11,

2x-3y+0z=1.

Let

A=[1 2 1; 1 0 3; 2 -3 0], X=[x; y; z], B=[7; 11; 1]; AX=B.

|A|=det([1 2 1; 1 0 3; 2 -3 0]) =1(9)-2(-6)+1(-3)=18≠0.

Therefore, the system has unique solution X=A⁻¹B.

For A, we have

A_11=0+9=9, A_12=-(0-6)=6, A_13=-3-0=-3,; A_21=-(0+3)=-3, A_22=0-2=-2, A_23=-(-3-4)=7,; A_31=6-0=6, A_32=-(3-1)=-2, A_33=0-2=-2.

adj(A)= [9 6 -3; -3 -2 7; 6 -2 -2]' =[9 -3 6; 6 -2 -2; -3 7 -2].

A⁻¹=(adj(A))/|A| =1/18[9 -3 6; 6 -2 -2; -3 7 -2].

The solution is X=A⁻¹B.

[x; y; z] =1/18[9 -3 6; 6 -2 -2; -3 7 -2] [7; 11; 1] =1/18[63-33+6; 42-22-2; -21+77-2] =1/18[36; 18; 54] =[2; 1; 3].

Therefore, x=2, y=1, z=3.

---

## Page 32 — Solve the Equations with Reciprocals by Matrix Method

**Question:** Solve the equations:

2/x+3/y+10/z=4, 4/x-6/y+5/z=1, 6/x+9/y-20/z=2.

**Solution:** The given equations are

2(1/x)+3(1/y)+10(1/z)=4 (1)

4(1/x)-6(1/y)+5(1/z)=1 (2)

6(1/x)+9(1/y)-20(1/z)=2 (3)

Let

A=[2 3 10; 4 -6 5; 6 9 -20], X=[1/x; 1/y; 1/z], B=[4; 1; 2]; AX=B.

|A|=det([2 3 10; 4 -6 5; 6 9 -20]) =2(120+45)-3(-80-30)+10(36+36)

=2(165)-3(-140)+10(72)=330+330+720=1380≠0.

Therefore, the system has unique solution X=A⁻¹B.

For A, we have

A_11=(120+45)=165, A_12=-(-80-30)=110, A_13=(36+36)=72,; A_21=-(-60-50)=110, A_22=(-40-60)=-100, A_23=-(-40-36)=76,; A_31=(-18+24)=6, A_32=-(-40+20)=20, A_33=(-24-12)=-36.

adj(A)= [165 110 72; 110 -100 76; 6 20 -36]' =[165 110 6; 110 -100 20; 72 76 -36].

A⁻¹=1/1380[165 110 6; 110 -100 20; 72 76 -36].

The solution is X=A⁻¹B.

[1/x; 1/y; 1/z] =1/1380[165 110 6; 110 -100 20; 72 76 -36] [4; 1; 2] =1/1380[660+110+12; 440-100+40; 288+76-72] =1/1380[782; 380; 292].

The source then states:

1/x=782/1380=17/30, 1/y=380/1380=19/69, 1/z=292/1380=73/345.

Therefore, the printed answer is

x=30/17, y=69/19, z=345/73.

---

## Page 33 — Reciprocal Equations, Substitution, and Matrix Method

**Question:** Solve the equations:

2/x+3/y+10/z=4, 4/x-6/y+5/z=1, 6/x+9/y-20/z=2.

**Solution:** The given equations are

2(1/x)+3(1/y)+10(1/z)=4,

4(1/x)-6(1/y)+5(1/z)=1,

6(1/x)+9(1/y)-20(1/z)=2.

Let

u=1/x, v=1/y, w=1/z.

Then the equations become

2u+3v+10w=4,

4u-6v+5w=1,

6u+9v-20w=2.

Let

A=[2 3 10; 4 -6 5; 6 9 -20], X=[u; v; w], B=[4; 1; 2]; AX=B.

|A|=det([2 3 10; 4 -6 5; 6 9 -20]) =2(120-45)-3(-80-30)+10(36+36)

=2(75)-3(-110)+10(72)=150+330+720=1200≠0.

Therefore, the system has unique solution X=A⁻¹B.

For A, we have

A_11=120, A_12=-80, A_13=36,; A_21=-45, A_22=75, A_23=-36,; A_31=45, A_32=-30, A_33=-18.

adj(A)= [120 -45 45; -80 75 -30; 36 -36 -18]' =[120 -80 36; -45 75 -36; 45 -30 -18].

A⁻¹=1/1200 [120 -80 36; -45 75 -36; 45 -30 -18].

The solution is X=A⁻¹B.

[u; v; w] =1/1200 [120 -80 36; -45 75 -36; 45 -30 -18] [4; 1; 2] =1/1200[480-80+72; -180+75-72; 180-30-36] =1/1200[472; -177; 114].

Therefore,

u=59/150, v=-59/400, w=19/200.

That is,

1/x=59/150, 1/y=-59/400, 1/z=19/200.

Therefore,

x=150/59, y=-400/59, z=200/19.

---

## End of Transcription

**Transcription fidelity note:** This file follows the supplied PDF and preserves its stated answers, including any arithmetic or notation that may be inconsistent within the source. It does not silently replace the source's printed results with independently corrected answers.
