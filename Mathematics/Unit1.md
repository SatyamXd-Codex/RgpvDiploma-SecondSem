# UNIT - I: Determinants and Matrices

This unit forms the bedrock of linear algebra, a fundamental branch of mathematics extensively used in engineering, computer science, physics, economics, and many other fields. Determinants and matrices provide powerful tools for solving systems of linear equations, transforming coordinates, and analyzing linear transformations.

---

## 1. Determinants

A **determinant** is a scalar value that can be computed from the elements of a square matrix. It provides important information about the matrix, such as whether a system of linear equations has a unique solution.

### 1.1 Elementary Properties of Determinants (up to 3rd Order)

A determinant is denoted by $|A|$ or $\det(A)$ for a matrix $A$.

**1st Order Determinant:**
For a $1 \times 1$ matrix $A = [a_{11}]$, the determinant is simply the value of the element itself.
$|A| = a_{11}$

**2nd Order Determinant:**
For a $2 \times 2$ matrix $A = \begin{pmatrix} a_{11} & a_{12} \\ a_{21} & a_{22} \end{pmatrix}$, the determinant is calculated as:
$|A| = a_{11}a_{22} - a_{12}a_{21}$

**Example Calculation (2nd Order):**
If $A = \begin{pmatrix} 3 & 1 \\ 4 & 2 \end{pmatrix}$
$|A| = (3)(2) - (1)(4) = 6 - 4 = 2$

**3rd Order Determinant:**
For a $3 \times 3$ matrix $A = \begin{pmatrix} a_{11} & a_{12} & a_{13} \\ a_{21} & a_{22} & a_{23} \\ a_{31} & a_{32} & a_{33} \end{pmatrix}$, the determinant can be calculated using the cofactor expansion method (usually along the first row for simplicity, but any row or column can be chosen):

$|A| = a_{11} \begin{vmatrix} a_{22} & a_{23} \\ a_{32} & a_{33} \end{vmatrix} - a_{12} \begin{vmatrix} a_{21} & a_{23} \\ a_{31} & a_{33} \end{vmatrix} + a_{13} \begin{vmatrix} a_{21} & a_{22} \\ a_{31} & a_{32} \end{vmatrix}$

Which expands to:
$|A| = a_{11}(a_{22}a_{33} - a_{23}a_{32}) - a_{12}(a_{21}a_{33} - a_{23}a_{31}) + a_{13}(a_{21}a_{32} - a_{22}a_{31})$

**Example Calculation (3rd Order):**
If $A = \begin{pmatrix} 1 & 2 & 3 \\ 0 & 1 & 4 \\ 5 & 6 & 0 \end{pmatrix}$

$|A| = 1 \begin{vmatrix} 1 & 4 \\ 6 & 0 \end{vmatrix} - 2 \begin{vmatrix} 0 & 4 \\ 5 & 0 \end{vmatrix} + 3 \begin{vmatrix} 0 & 1 \\ 5 & 6 \end{vmatrix}$
$|A| = 1((1)(0) - (4)(6)) - 2((0)(0) - (4)(5)) + 3((0)(6) - (1)(5))$
$|A| = 1(0 - 24) - 2(0 - 20) + 3(0 - 5)$
$|A| = -24 - 2(-20) + 3(-5)$
$|A| = -24 + 40 - 15$
$|A| = 16 - 15 = 1$

**Key Properties of Determinants:**
* **Property 1: Row/Column Swap:** If any two rows (or columns) of a determinant are interchanged, the sign of the determinant changes.
    * Example: $\begin{vmatrix} 1 & 2 \\ 3 & 4 \end{vmatrix} = -2$, but $\begin{vmatrix} 3 & 4 \\ 1 & 2 \end{vmatrix} = 2$.
* **Property 2: Identical Rows/Columns:** If any two rows (or columns) of a determinant are identical, the value of the determinant is zero.
    * Example: $\begin{vmatrix} 1 & 2 \\ 1 & 2 \end{vmatrix} = (1)(2) - (2)(1) = 0$.
* **Property 3: Scalar Multiplication:** If all elements of a row (or column) are multiplied by a constant $k$, the value of the determinant is multiplied by $k$.
    * Example: $\begin{vmatrix} 2 & 4 \\ 3 & 5 \end{vmatrix} = 10-12 = -2$. If $R_1 \to 2R_1$, $\begin{vmatrix} 4 & 8 \\ 3 & 5 \end{vmatrix} = 20-24 = -4 = 2 \times (-2)$.
* **Property 4: Row/Column Operation (Elementary Row/Column Operation):** If to any row (or column) of a determinant, a scalar multiple of another row (or column) is added, the value of the determinant remains unchanged. This property is very useful for simplifying determinants.
    * Example: $\begin{vmatrix} 1 & 2 \\ 3 & 4 \end{vmatrix} = -2$. If $R_2 \to R_2 - 3R_1$, $\begin{vmatrix} 1 & 2 \\ 3-3(1) & 4-3(2) \end{vmatrix} = \begin{vmatrix} 1 & 2 \\ 0 & -2 \end{vmatrix} = (1)(-2) - (2)(0) = -2$.
* **Property 5: Transpose:** The value of the determinant remains unchanged if its rows and columns are interchanged (i.e., $|A^T| = |A|$).
* **Property 6: Row/Column of Zeros:** If all elements of any row or column are zero, the value of the determinant is zero.

### 1.2 Consistency of Equations

Determinants are crucial for determining the consistency of a system of linear equations. A system of linear equations is consistent if it has at least one solution. It is inconsistent if it has no solution.

Consider a system of linear equations:
$a_1x + b_1y + c_1z = d_1$
$a_2x + b_2y + c_2z = d_2$
$a_3x + b_3y + c_3z = d_3$

Let $\Delta$ (or $D$) be the determinant of the coefficient matrix:
$\Delta = \begin{vmatrix} a_1 & b_1 & c_1 \\ a_2 & b_2 & c_2 \\ a_3 & b_3 & c_3 \end{vmatrix}$

**Conditions for Consistency:**
1.  **Unique Solution:** If $\Delta \neq 0$, the system is **consistent** and has a **unique solution**.
2.  **No Solution (Inconsistent):** If $\Delta = 0$, then we need to check further determinants.
    * Calculate $\Delta_x, \Delta_y, \Delta_z$ (as defined in Cramer's Rule below).
    * If $\Delta = 0$ AND at least one of $\Delta_x, \Delta_y, \Delta_z$ is **non-zero**, then the system is **inconsistent** (no solution).
3.  **Infinitely Many Solutions (Consistent):** If $\Delta = 0$ AND $\Delta_x = 0$, $\Delta_y = 0$, $\Delta_z = 0$, then the system is **consistent** and has **infinitely many solutions**.

**Problem-Solving Steps for Consistency:**
1.  Form the coefficient matrix $A$ and calculate its determinant $\Delta$.
2.  If $\Delta \neq 0$, a unique solution exists (consistent).
3.  If $\Delta = 0$, calculate $\Delta_x, \Delta_y, \Delta_z$.
4.  If any of $\Delta_x, \Delta_y, \Delta_z$ is non-zero, it's inconsistent.
5.  If all of $\Delta_x, \Delta_y, \Delta_z$ are zero, it's consistent with infinitely many solutions.

### 1.3 Cramer's Rule

Cramer's Rule is a method for solving systems of linear equations using determinants. It is particularly useful for systems with a unique solution (i.e., when $\Delta \neq 0$).

For the system:
$a_1x + b_1y + c_1z = d_1$
$a_2x + b_2y + c_2z = d_2$
$a_3x + b_3y + c_3z = d_3$

Define the following determinants:
$\Delta = \begin{vmatrix} a_1 & b_1 & c_1 \\ a_2 & b_2 & c_2 \\ a_3 & b_3 & c_3 \end{vmatrix}$ (Determinant of the coefficient matrix)

$\Delta_x = \begin{vmatrix} d_1 & b_1 & c_1 \\ d_2 & b_2 & c_2 \\ d_3 & b_3 & c_3 \end{vmatrix}$ (Replace x-coefficients column with constants)

$\Delta_y = \begin{vmatrix} a_1 & d_1 & c_1 \\ a_2 & d_2 & c_2 \\ a_3 & d_3 & c_3 \end{vmatrix}$ (Replace y-coefficients column with constants)

$\Delta_z = \begin{vmatrix} a_1 & b_1 & d_1 \\ a_2 & b_2 & d_2 \\ a_3 & b_3 & d_3 \end{vmatrix}$ (Replace z-coefficients column with constants)

If $\Delta \neq 0$, then the unique solution is given by:

$$
\boxed{
x = \frac{\Delta_x}{\Delta}, \quad y = \frac{\Delta_y}{\Delta}, \quad z = \frac{\Delta_z}{\Delta}
}
$$

**Problem-Solving Steps using Cramer's Rule:**
1.  Write the system of equations in standard form.
2.  Calculate the determinant of the coefficient matrix, $\Delta$.
3.  If $\Delta = 0$, Cramer's Rule cannot be directly applied for a unique solution (refer to consistency conditions).
4.  If $\Delta \neq 0$, calculate $\Delta_x, \Delta_y, \Delta_z$.
5.  Apply the formulas to find $x, y, z$.

**Example Problem (Cramer's Rule):**
Solve the system:
$x + 2y - z = 3$
$3x + y + 2z = 1$
$x - 3y - z = -2$

**Step 1: Calculate $\Delta$**
$\Delta = \begin{vmatrix} 1 & 2 & -1 \\ 3 & 1 & 2 \\ 1 & -3 & -1 \end{vmatrix}$
$\Delta = 1((1)(-1) - (2)(-3)) - 2((3)(-1) - (2)(1)) + (-1)((3)(-3) - (1)(1))$
$\Delta = 1(-1 + 6) - 2(-3 - 2) - 1(-9 - 1)$
$\Delta = 1(5) - 2(-5) - 1(-10)$
$\Delta = 5 + 10 + 10 = 25$

Since $\Delta = 25 \neq 0$, a unique solution exists.

**Step 2: Calculate $\Delta_x$**
$\Delta_x = \begin{vmatrix} 3 & 2 & -1 \\ 1 & 1 & 2 \\ -2 & -3 & -1 \end{vmatrix}$
$\Delta_x = 3((1)(-1) - (2)(-3)) - 2((1)(-1) - (2)(-2)) + (-1)((1)(-3) - (1)(-2))$
$\Delta_x = 3(-1 + 6) - 2(-1 + 4) - 1(-3 + 2)$
$\Delta_x = 3(5) - 2(3) - 1(-1)$
$\Delta_x = 15 - 6 + 1 = 10$

**Step 3: Calculate $\Delta_y$**
$\Delta_y = \begin{vmatrix} 1 & 3 & -1 \\ 3 & 1 & 2 \\ 1 & -2 & -1 \end{vmatrix}$
$\Delta_y = 1((1)(-1) - (2)(-2)) - 3((3)(-1) - (2)(1)) + (-1)((3)(-2) - (1)(1))$
$\Delta_y = 1(-1 + 4) - 3(-3 - 2) - 1(-6 - 1)$
$\Delta_y = 1(3) - 3(-5) - 1(-7)$
$\Delta_y = 3 + 15 + 7 = 25$

**Step 4: Calculate $\Delta_z$**
$\Delta_z = \begin{vmatrix} 1 & 2 & 3 \\ 3 & 1 & 1 \\ 1 & -3 & -2 \end{vmatrix}$
$\Delta_z = 1((1)(-2) - (1)(-3)) - 2((3)(-2) - (1)(1)) + 3((3)(-3) - (1)(1))$
$\Delta_z = 1(-2 + 3) - 2(-6 - 1) + 3(-9 - 1)$
$\Delta_z = 1(1) - 2(-7) + 3(-10)$
$\Delta_z = 1 + 14 - 30 = -15$

**Step 5: Find $x, y, z$**
$x = \frac{\Delta_x}{\Delta} = \frac{10}{25} = \frac{2}{5}$
$y = \frac{\Delta_y}{\Delta} = \frac{25}{25} = 1$
$z = \frac{\Delta_z}{\Delta} = \frac{-15}{25} = -\frac{3}{5}$

---

## 2. Matrices

A **matrix** is a rectangular array of numbers (or elements) arranged in rows and columns. Matrices are used to represent linear transformations, store data, and solve systems of equations efficiently.

### 2.1 Algebra of Matrices

Matrices can be added, subtracted, and multiplied under specific conditions.

* **Order of a Matrix:** An $m \times n$ matrix has $m$ rows and $n$ columns.

* **Types of Matrices:**
    * **Row Matrix:** A matrix with only one row.
    * **Column Matrix:** A matrix with only one column.
    * **Square Matrix:** A matrix with an equal number of rows and columns ($m=n$).
    * **Diagonal Matrix:** A square matrix where all non-diagonal elements are zero.
    * **Scalar Matrix:** A diagonal matrix where all diagonal elements are equal.
    * **Identity Matrix ($I$):** A square matrix with ones on the main diagonal and zeros elsewhere. It acts like the number '1' in matrix multiplication ($AI = IA = A$).
    * **Zero Matrix ($O$):** A matrix where all elements are zero.
    * **Symmetric Matrix:** A square matrix where $A^T = A$ (elements are symmetric about the main diagonal).
    * **Skew-Symmetric Matrix:** A square matrix where $A^T = -A$ (diagonal elements are zero, and elements are negative symmetric).

* **Equality of Matrices:** Two matrices $A$ and $B$ are equal if and only if they have the same order AND their corresponding elements are equal ($a_{ij} = b_{ij}$ for all $i, j$).

* **Addition and Subtraction:**
    * Matrices can be added or subtracted **only if they have the same order**.
    * The operation is performed element-wise.
    * If $A = [a_{ij}]$ and $B = [b_{ij}]$, then $A \pm B = [a_{ij} \pm b_{ij}]$.

    **Example:**
    If $A = \begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix}$ and $B = \begin{pmatrix} 5 & 6 \\ 7 & 8 \end{pmatrix}$
    $A + B = \begin{pmatrix} 1+5 & 2+6 \\ 3+7 & 4+8 \end{pmatrix} = \begin{pmatrix} 6 & 8 \\ 10 & 12 \end{pmatrix}$

* **Scalar Multiplication:**
    * To multiply a matrix $A$ by a scalar $k$, multiply every element of the matrix by $k$.
    * If $A = [a_{ij}]$, then $kA = [ka_{ij}]$.

    **Example:**
    If $A = \begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix}$ and $k=3$
    $3A = \begin{pmatrix} 3 \times 1 & 3 \times 2 \\ 3 \times 3 & 3 \times 4 \end{pmatrix} = \begin{pmatrix} 3 & 6 \\ 9 & 12 \end{pmatrix}$

* **Matrix Multiplication:**
    * The product $AB$ of two matrices $A$ and $B$ is defined **only if the number of columns in $A$ is equal to the number of rows in $B$**.
    * If $A$ is an $m \times n$ matrix and $B$ is an $n \times p$ matrix, then the product $AB$ will be an $m \times p$ matrix.
    * The element in the $i$-th row and $j$-th column of $AB$ is found by taking the dot product of the $i$-th row of $A$ with the $j$-th column of $B$.

    **Formula for $C = AB$ where $C = [c_{ij}]$:**
    $c_{ij} = \sum_{k=1}^{n} a_{ik}b_{kj}$

    **Example:**
    If $A = \begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix}$ and $B = \begin{pmatrix} 5 & 6 \\ 7 & 8 \end{pmatrix}$
    $A$ is $2 \times 2$, $B$ is $2 \times 2$, so $AB$ will be $2 \times 2$.
    $AB = \begin{pmatrix} (1)(5)+(2)(7) & (1)(6)+(2)(8) \\ (3)(5)+(4)(7) & (3)(6)+(4)(8) \end{pmatrix}$
    $AB = \begin{pmatrix} 5+14 & 6+16 \\ 15+28 & 18+32 \end{pmatrix} = \begin{pmatrix} 19 & 22 \\ 43 & 50 \end{pmatrix}$

    **Important Points about Matrix Multiplication:**
    * Matrix multiplication is generally **not commutative** ($AB \neq BA$).
    * Matrix multiplication is **associative** ($(AB)C = A(BC)$).
    * Matrix multiplication is **distributive** ($A(B+C) = AB + AC$).

### 2.2 Inverse of a Matrix

The **inverse of a square matrix $A$**, denoted as $A^{-1}$, is a matrix such that when multiplied by $A$, it yields the identity matrix $I$.
$AA^{-1} = A^{-1}A = I$

* **Existence of Inverse:** A square matrix $A$ has an inverse if and only if its determinant is non-zero (i.e., $|A| \neq 0$). Such a matrix is called **non-singular**. If $|A| = 0$, the matrix is **singular** and its inverse does not exist.

* **Formula for Inverse:**
    $A^{-1} = \frac{1}{|A|} \text{adj}(A)$
    where $\text{adj}(A)$ is the adjoint of matrix $A$.

* **Adjoint of a Matrix:**
    The adjoint of a matrix $A$ is the transpose of its cofactor matrix.
    If $C$ is the cofactor matrix of $A$, then $\text{adj}(A) = C^T$.

    * **Cofactor ($C_{ij}$):** The cofactor of an element $a_{ij}$ is $(-1)^{i+j}$ times the determinant of the submatrix obtained by deleting the $i$-th row and $j$-th column.
        $C_{ij} = (-1)^{i+j} M_{ij}$, where $M_{ij}$ is the minor of $a_{ij}$.

**Steps to find the Inverse of a $3 \times 3$ matrix:**
1.  **Calculate the determinant of $A$ ($|A|$).** If $|A|=0$, the inverse does not exist.
2.  **Find the matrix of minors ($M_{ij}$).** For each element $a_{ij}$, cover its row and column and calculate the determinant of the remaining $2 \times 2$ matrix.
3.  **Find the matrix of cofactors ($C_{ij}$).** Apply the sign pattern to the matrix of minors:
    $\begin{pmatrix} + & - & + \\ - & + & - \\ + & - & + \end{pmatrix}$
    So, $C_{ij} = (-1)^{i+j} M_{ij}$.
4.  **Find the adjoint of $A$ ($\text{adj}(A)$).** Transpose the cofactor matrix ($C^T$). This means swapping rows and columns.
5.  **Calculate $A^{-1}$** using the formula $A^{-1} = \frac{1}{|A|} \text{adj}(A)$.

**Example Problem (Inverse of a Matrix):**
Find the inverse of $A = \begin{pmatrix} 1 & 2 & -1 \\ 0 & 1 & 4 \\ 5 & 6 & 0 \end{pmatrix}$

**Step 1: Calculate $|A|$**
From the determinant example above, $|A| = 1$. (Since $|A| \neq 0$, the inverse exists.)

**Step 2: Find the Matrix of Minors ($M_{ij}$)**
$M_{11} = \begin{vmatrix} 1 & 4 \\ 6 & 0 \end{vmatrix} = 0 - 24 = -24$
$M_{12} = \begin{vmatrix} 0 & 4 \\ 5 & 0 \end{vmatrix} = 0 - 20 = -20$
$M_{13} = \begin{vmatrix} 0 & 1 \\ 5 & 6 \end{vmatrix} = 0 - 5 = -5$

$M_{21} = \begin{vmatrix} 2 & -1 \\ 6 & 0 \end{vmatrix} = 0 - (-6) = 6$
$M_{22} = \begin{vmatrix} 1 & -1 \\ 5 & 0 \end{vmatrix} = 0 - (-5) = 5$
$M_{23} = \begin{vmatrix} 1 & 2 \\ 5 & 6 \end{vmatrix} = 6 - 10 = -4$

$M_{31} = \begin{vmatrix} 2 & -1 \\ 1 & 4 \end{vmatrix} = 8 - (-1) = 9$
$M_{32} = \begin{vmatrix} 1 & -1 \\ 0 & 4 \end{vmatrix} = 4 - 0 = 4$
$M_{33} = \begin{vmatrix} 1 & 2 \\ 0 & 1 \end{vmatrix} = 1 - 0 = 1$

So, the matrix of minors $M = \begin{pmatrix} -24 & -20 & -5 \\ 6 & 5 & -4 \\ 9 & 4 & 1 \end{pmatrix}$

**Step 3: Find the Matrix of Cofactors ($C_{ij}$)**
Apply the sign pattern: $\begin{pmatrix} + & - & + \\ - & + & - \\ + & - & + \end{pmatrix}$
$C_{11} = -24$
$C_{12} = -(-20) = 20$
$C_{13} = -5$

$C_{21} = -(6) = -6$
$C_{22} = 5$
$C_{23} = -(-4) = 4$

$C_{31} = 9$
$C_{32} = -(4) = -4$
$C_{33} = 1$

So, the cofactor matrix $C = \begin{pmatrix} -24 & 20 & -5 \\ -6 & 5 & 4 \\ 9 & -4 & 1 \end{pmatrix}$

**Step 4: Find the Adjoint of $A$ ($\text{adj}(A)$)**
$\text{adj}(A) = C^T = \begin{pmatrix} -24 & -6 & 9 \\ 20 & 5 & -4 \\ -5 & 4 & 1 \end{pmatrix}$

**Step 5: Calculate $A^{-1}$**
$A^{-1} = \frac{1}{|A|} \text{adj}(A) = \frac{1}{1} \begin{pmatrix} -24 & -6 & 9 \\ 20 & 5 & -4 \\ -5 & 4 & 1 \end{pmatrix}$
$A^{-1} = \begin{pmatrix} -24 & -6 & 9 \\ 20 & 5 & -4 \\ -5 & 4 & 1 \end{pmatrix}$

### 2.3 Matrix Inverse Method to Solve a System of Linear Equations in 3 Variables

The matrix inverse method is another powerful way to solve systems of linear equations, especially when dealing with multiple systems that have the same coefficient matrix but different constant terms.

Consider a system of linear equations:
$a_1x + b_1y + c_1z = d_1$
$a_2x + b_2y + c_2z = d_2$
$a_3x + b_3y + c_3z = d_3$

This system can be written in matrix form as $AX = B$, where:
$A = \begin{pmatrix} a_1 & b_1 & c_1 \\ a_2 & b_2 & c_2 \\ a_3 & b_3 & c_3 \end{pmatrix}$ (Coefficient matrix)
$X = \begin{pmatrix} x \\ y \\ z \end{pmatrix}$ (Variable matrix)
$B = \begin{pmatrix} d_1 \\ d_2 \\ d_3 \end{pmatrix}$ (Constant matrix)

If $A$ is a non-singular matrix (i.e., $|A| \neq 0$), then $A^{-1}$ exists. We can multiply both sides of the equation $AX = B$ by $A^{-1}$ from the left:
$A^{-1}(AX) = A^{-1}B$
$(A^{-1}A)X = A^{-1}B$
$IX = A^{-1}B$
$X = A^{-1}B$

**Problem-Solving Steps using Matrix Inverse Method:**
1.  Write the system of equations in matrix form $AX = B$.
2.  Calculate the determinant of the coefficient matrix $A$ ($|A|$).
3.  If $|A| = 0$, the inverse does not exist, and this method cannot yield a unique solution (system is either inconsistent or has infinitely many solutions).
4.  If $|A| \neq 0$, find the inverse of matrix $A$ ($A^{-1}$) using the steps described above (determinant, minors, cofactors, adjoint, inverse formula).
5.  Multiply $A^{-1}$ by the constant matrix $B$ ($X = A^{-1}B$).
6.  The resulting column matrix $X$ will give the values of $x, y, z$.

**Example Problem (Matrix Inverse Method):**
Solve the system:
$x + 2y - z = 3$
$3x + y + 2z = 1$
$x - 3y - z = -2$

**Step 1: Write in matrix form $AX = B$**
$A = \begin{pmatrix} 1 & 2 & -1 \\ 3 & 1 & 2 \\ 1 & -3 & -1 \end{pmatrix}$, $X = \begin{pmatrix} x \\ y \\ z \end{pmatrix}$, $B = \begin{pmatrix} 3 \\ 1 \\ -2 \end{pmatrix}$

**Step 2: Calculate $|A|$**
From the Cramer's Rule example, $|A| = 25$. (Since $|A| \neq 0$, the inverse exists.)

**Step 3: Find $A^{-1}$**
Since we haven't calculated this exact inverse previously, let's find it.
* **Determinant:** $|A|=25$
* **Minors:**
    $M_{11} = \begin{vmatrix} 1 & 2 \\ -3 & -1 \end{vmatrix} = -1 - (-6) = 5$
    $M_{12} = \begin{vmatrix} 3 & 2 \\ 1 & -1 \end{vmatrix} = -3 - 2 = -5$
    $M_{13} = \begin{vmatrix} 3 & 1 \\ 1 & -3 \end{vmatrix} = -9 - 1 = -10$

    $M_{21} = \begin{vmatrix} 2 & -1 \\ -3 & -1 \end{vmatrix} = -2 - 3 = -5$
    $M_{22} = \begin{vmatrix} 1 & -1 \\ 1 & -1 \end{vmatrix} = -1 - (-1) = 0$
    $M_{23} = \begin{vmatrix} 1 & 2 \\ 1 & -3 \end{vmatrix} = -3 - 2 = -5$

    $M_{31} = \begin{vmatrix} 2 & -1 \\ 1 & 2 \end{vmatrix} = 4 - (-1) = 5$
    $M_{32} = \begin{vmatrix} 1 & -1 \\ 3 & 2 \end{vmatrix} = 2 - (-3) = 5$
    $M_{33} = \begin{vmatrix} 1 & 2 \\ 3 & 1 \end{vmatrix} = 1 - 6 = -5$

    Matrix of Minors $M = \begin{pmatrix} 5 & -5 & -10 \\ -5 & 0 & -5 \\ 5 & 5 & -5 \end{pmatrix}$

* **Cofactors:** Apply the sign pattern $\begin{pmatrix} + & - & + \\ - & + & - \\ + & - & + \end{pmatrix}$
    $C = \begin{pmatrix} 5 & -(-5) & -10 \\ -(-5) & 0 & -(-5) \\ 5 & -(5) & -5 \end{pmatrix} = \begin{pmatrix} 5 & 5 & -10 \\ 5 & 0 & 5 \\ 5 & -5 & -5 \end{pmatrix}$

* **Adjoint:** $\text{adj}(A) = C^T = \begin{pmatrix} 5 & 5 & 5 \\ 5 & 0 & -5 \\ -10 & 5 & -5 \end{pmatrix}$

* **Inverse:** $A^{-1} = \frac{1}{|A|} \text{adj}(A) = \frac{1}{25} \begin{pmatrix} 5 & 5 & 5 \\ 5 & 0 & -5 \\ -10 & 5 & -5 \end{pmatrix}$

**Step 4: Multiply $A^{-1}$ by $B$ ($X = A^{-1}B$)**
$X = \frac{1}{25} \begin{pmatrix} 5 & 5 & 5 \\ 5 & 0 & -5 \\ -10 & 5 & -5 \end{pmatrix} \begin{pmatrix} 3 \\ 1 \\ -2 \end{pmatrix}$

$X = \frac{1}{25} \begin{pmatrix} (5)(3) + (5)(1) + (5)(-2) \\ (5)(3) + (0)(1) + (-5)(-2) \\ (-10)(3) + (5)(1) + (-5)(-2) \end{pmatrix}$

$X = \frac{1}{25} \begin{pmatrix} 15 + 5 - 10 \\ 15 + 0 + 10 \\ -30 + 5 + 10 \end{pmatrix}$

$X = \frac{1}{25} \begin{pmatrix} 10 \\ 25 \\ -15 \end{pmatrix}$

**Step 5: Extract $x, y, z$**
$X = \begin{pmatrix} 10/25 \\ 25/25 \\ -15/25 \end{pmatrix} = \begin{pmatrix} 2/5 \\ 1 \\ -3/5 \end{pmatrix}$

So, $x = \frac{2}{5}$, $y = 1$, $z = -\frac{3}{5}$.

