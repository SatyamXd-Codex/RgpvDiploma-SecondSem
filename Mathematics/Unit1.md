

## UNIT - I: Determinants and Matrices

This unit focuses on two fundamental concepts in mathematics: Determinants and Matrices. Both play a crucial role in solving systems of linear equations, understanding transformations in geometry, and are vital in various engineering and scientific applications.

### I. Determinants

**Definition:** A determinant is a scalar value that can be computed from the elements of a square matrix. It is only defined for square matrices (i.e., matrices with an equal number of rows and columns).

**Purpose/Significance:**
1.  To determine the **consistency** of a system of linear equations.
2.  To find the **inverse of a matrix**.
3.  To calculate the **area of a triangle** or the **area of a parallelogram**.

#### A. Elementary Properties of Determinants up to 3rd Order

These properties are crucial for simplifying and evaluating determinants, especially for larger orders, but are illustrated here for up to 3rd order.

1.  **Interchange of Rows and Columns (Transpose):**
    * **Property:** The value of a determinant remains unchanged if its rows and columns are interchanged (i.e., the determinant of a matrix is equal to the determinant of its transpose).
    * **Formula/Example:** $det(A) = det(A^T)$
        For a 2x2 matrix:
        $$\begin{vmatrix} a & b \\ c & d \end{vmatrix} = ad - bc$$
        $$\text{And } \begin{vmatrix} a & c \\ b & d \end{vmatrix} = ad - bc$$

2.  **Interchange of Two Rows or Two Columns:**
    * **Property:** If any two rows or any two columns of a determinant are interchanged, the sign of the determinant changes, but its numerical value remains the same.
    * **Formula/Example:** If $R_i \leftrightarrow R_j$ or $C_i \leftrightarrow C_j$, then $det(A_{new}) = -det(A_{old})$.
        $$\begin{vmatrix} a & b \\ c & d \end{vmatrix} = ad - bc$$
        Interchanging rows $R_1 \leftrightarrow R_2$:
        $$\begin{vmatrix} c & d \\ a & b \end{vmatrix} = cb - da = -(ad - bc)$$

3.  **Identical Rows or Columns:**
    * **Property:** If any two rows or any two columns of a determinant are identical (all corresponding elements are the same), then the value of the determinant is zero.
    * **Formula/Example:** If $R_i = R_j$ or $C_i = C_j$, then $det(A) = 0$.
        $$\begin{vmatrix} 1 & 2 & 3 \\ 1 & 2 & 3 \\ 4 & 5 & 6 \end{vmatrix} = 0$$

4.  **Scalar Multiplication of a Row or Column:**
    * **Property:** If all the elements of any one row or any one column of a determinant are multiplied by a scalar $k$, then the value of the determinant is also multiplied by $k$.
    * **Formula/Example:**
        $$\begin{vmatrix} ka & kb \\ c & d \end{vmatrix} = k \begin{vmatrix} a & b \\ c & d \end{vmatrix} = k(ad - bc)$$
        *Note:* For a matrix $A$ of order $n \times n$, $det(kA) = k^n det(A)$.

5.  **Proportional Rows or Columns:**
    * **Property:** If the elements of any two rows or any two columns of a determinant are proportional, then the value of the determinant is zero. (This is a generalization of property 3).
    * **Formula/Example:** If $R_i = kR_j$ or $C_i = kC_j$, then $det(A) = 0$.
        $$\begin{vmatrix} 1 & 2 & 3 \\ 2 & 4 & 6 \\ 7 & 8 & 9 \end{vmatrix} = 0 \quad (\text{since } R_2 = 2R_1)$$

6.  **Sum of Elements in a Row/Column:**
    * **Property:** If some or all elements of a row or column of a determinant are expressed as a sum of two (or more) terms, then the determinant can be expressed as a sum of two (or more) determinants.
    * **Formula/Example:**
        $$\begin{vmatrix} a+x & b \\ c+y & d \end{vmatrix} = \begin{vmatrix} a & b \\ c & d \end{vmatrix} + \begin{vmatrix} x & b \\ y & d \end{vmatrix}$$

7.  **Row/Column Operations (Most Important for Simplification):**
    * **Property:** If to the elements of any row or column, the scalar multiples of corresponding elements of any other row or column are added (or subtracted), then the value of the determinant remains unchanged.
    * **Formula/Example:** $R_i \rightarrow R_i + kR_j$ or $C_i \rightarrow C_i + kC_j$.
        $$\begin{vmatrix} a & b \\ c & d \end{vmatrix}$$
        Perform $R_1 \rightarrow R_1 + kR_2$:
        $$\begin{vmatrix} a+kc & b+kd \\ c & d \end{vmatrix} = (a+kc)d - (b+kd)c = ad + kcd - bc - kcd = ad - bc$$
        The value remains the same. This property is extensively used to create zeros in a determinant, making evaluation easier.

#### B. Evaluating Determinants (up to 3rd Order)

* **For 2x2 Matrix:**
    If $A = \begin{bmatrix} a & b \\ c & d \end{bmatrix}$, then $det(A) = ad - bc$.

* **For 3x3 Matrix (Sarrus' Rule / Cofactor Expansion):**
    If $A = \begin{bmatrix} a_{11} & a_{12} & a_{13} \\ a_{21} & a_{22} & a_{23} \\ a_{31} & a_{32} & a_{33} \end{bmatrix}$, then
    $$det(A) = a_{11}(a_{22}a_{33} - a_{23}a_{32}) - a_{12}(a_{21}a_{33} - a_{23}a_{31}) + a_{13}(a_{21}a_{32} - a_{22}a_{31})$$
    This is called expansion along the first row. You can expand along any row or column using the cofactor method.
    * **Cofactor ($C_{ij}$):** $C_{ij} = (-1)^{i+j} M_{ij}$, where $M_{ij}$ is the minor (determinant of the submatrix obtained by deleting the $i$-th row and $j$-th column).
    * **Determinant:** $det(A) = \sum_{j=1}^{n} a_{ij} C_{ij}$ (expansion along row $i$) or $det(A) = \sum_{i=1}^{n} a_{ij} C_{ij}$ (expansion along column $j$).

### II. Consistency of Equations

For a system of linear equations, "consistency" refers to whether the system has a solution or not.

Consider a system of $n$ linear equations in $n$ variables (e.g., 3 variables for 3 equations):
$a_1x + b_1y + c_1z = d_1$
$a_2x + b_2y + c_2z = d_2$
$a_3x + b_3y + c_3z = d_3$

This can be written in matrix form as $AX = B$, where:
$A = \begin{bmatrix} a_1 & b_1 & c_1 \\ a_2 & b_2 & c_2 \\ a_3 & b_3 & c_3 \end{bmatrix}$ (coefficient matrix)
$X = \begin{bmatrix} x \\ y \\ z \end{bmatrix}$ (variable matrix)
$B = \begin{bmatrix} d_1 \\ d_2 \\ d_3 \end{bmatrix}$ (constant matrix)

**Consistency Conditions:**

1.  **Case 1: If $det(A) \neq 0$**
    * **Meaning:** The system is **consistent** and has a **unique solution**.
    * **Explanation:** This means the matrix A is invertible, and a single solution $X = A^{-1}B$ exists. Geometrically, for 3 variables, the three planes intersect at a single point.

2.  **Case 2: If $det(A) = 0$**
    * **Meaning:** The system may be either **consistent (with infinitely many solutions)** or **inconsistent (with no solution)**.
    * **Explanation:** In this case, we need to examine the adjoint of A multiplied by B ($adj(A)B$).
        * **If $det(A) = 0$ AND $adj(A)B = \begin{bmatrix} 0 \\ 0 \\ 0 \end{bmatrix}$ (a zero matrix):** The system is **consistent** and has **infinitely many solutions**. Geometrically, the planes either coincide or intersect along a common line.
        * **If $det(A) = 0$ AND $adj(A)B \neq \begin{bmatrix} 0 \\ 0 \\ 0 \end{bmatrix}$ (a non-zero matrix):** The system is **inconsistent** and has **no solution**. Geometrically, the planes are parallel or intersect in such a way that there is no common point of intersection (e.g., forming a triangular prism).

### III. Cramer’s Rule

Cramer's Rule is a formulaic method for solving a system of linear equations using determinants. It is particularly useful for systems with a unique solution (i.e., when $det(A) \neq 0$).

For a system of 3 linear equations in 3 variables:
$a_1x + b_1y + c_1z = d_1$
$a_2x + b_2y + c_2z = d_2$
$a_3x + b_3y + c_3z = d_3$

1.  **Calculate the determinant of the coefficient matrix, D ($det(A)$):**
    $$D = \begin{vmatrix} a_1 & b_1 & c_1 \\ a_2 & b_2 & c_2 \\ a_3 & b_3 & c_3 \end{vmatrix}$$

2.  **Calculate $D_x$:** Replace the first column (coefficients of $x$) in D with the constant terms ($d_1, d_2, d_3$).
    $$D_x = \begin{vmatrix} d_1 & b_1 & c_1 \\ d_2 & b_2 & c_2 \\ d_3 & b_3 & c_3 \end{vmatrix}$$

3.  **Calculate $D_y$:** Replace the second column (coefficients of $y$) in D with the constant terms.
    $$D_y = \begin{vmatrix} a_1 & d_1 & c_1 \\ a_2 & d_2 & c_2 \\ a_3 & d_3 & c_3 \end{vmatrix}$$

4.  **Calculate $D_z$:** Replace the third column (coefficients of $z$) in D with the constant terms.
    $$D_z = \begin{vmatrix} a_1 & b_1 & d_1 \\ a_2 & b_2 & d_2 \\ a_3 & b_3 & d_3 \end{vmatrix}$$

5.  **Find the solutions:**
    * $x = \frac{D_x}{D}$
    * $y = \frac{D_y}{D}$
    * $z = \frac{D_z}{D}$

**Condition:** Cramer's Rule is applicable **only if $D \neq 0$**. If $D=0$, the system either has no solution or infinitely many solutions, and Cramer's Rule cannot be directly used to find specific values.

### IV. Algebra of Matrices

**Definition:** A matrix is a rectangular array of numbers or functions, arranged in rows and columns.
* An $m \times n$ matrix has $m$ rows and $n$ columns.

#### A. Types of Matrices (Important for operations)

* **Row Matrix:** A matrix with only one row (e.g., $\begin{bmatrix} 1 & 2 & 3 \end{bmatrix}$).
* **Column Matrix:** A matrix with only one column (e.g., $\begin{bmatrix} 1 \\ 2 \end{bmatrix}$).
* **Square Matrix:** Number of rows equals number of columns (e.g., 2x2, 3x3).
* **Diagonal Matrix:** A square matrix where all non-diagonal elements are zero.
* **Scalar Matrix:** A diagonal matrix where all diagonal elements are equal.
* **Identity Matrix ($I$):** A square matrix where all diagonal elements are 1 and all non-diagonal elements are 0. (e.g., $I_3 = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix}$).
* **Zero Matrix (Null Matrix):** A matrix where all elements are zero.
* **Symmetric Matrix:** $A^T = A$ (elements symmetric about the main diagonal).
* **Skew-Symmetric Matrix:** $A^T = -A$ (diagonal elements are zero).

#### B. Operations on Matrices

1.  **Equality of Matrices:**
    * Two matrices $A$ and $B$ are equal if and only if they have the same order AND their corresponding elements are equal ($a_{ij} = b_{ij}$ for all $i, j$).

2.  **Addition and Subtraction of Matrices:**
    * **Condition:** Matrices must have the **same order**.
    * **Rule:** Add/subtract corresponding elements.
    * **Formula:** If $A = [a_{ij}]$ and $B = [b_{ij}]$, then $A \pm B = [a_{ij} \pm b_{ij}]$.
    * **Properties:**
        * Commutative: $A+B = B+A$
        * Associative: $(A+B)+C = A+(B+C)$
        * Additive Identity: $A+O = A$ (where O is the zero matrix of the same order).
        * Additive Inverse: $A+(-A) = O$.

3.  **Scalar Multiplication of a Matrix:**
    * **Rule:** Multiply every element of the matrix by the scalar.
    * **Formula:** If $A = [a_{ij}]$ and $k$ is a scalar, then $kA = [ka_{ij}]$.

4.  **Matrix Multiplication:**
    * **Condition:** For $AB$, the number of columns in $A$ must be equal to the number of rows in $B$.
        * If $A$ is an $m \times n$ matrix and $B$ is an $n \times p$ matrix, then the product $AB$ will be an $m \times p$ matrix.
    * **Rule:** The element in the $i$-th row and $j$-th column of $AB$ is the sum of the products of corresponding elements from the $i$-th row of $A$ and the $j$-th column of $B$.
    * **Formula:** If $AB = C$, then $c_{ij} = \sum_{k=1}^{n} a_{ik} b_{kj}$.
    * **Properties:**
        * Not Commutative: Generally, $AB \neq BA$.
        * Associative: $(AB)C = A(BC)$.
        * Distributive: $A(B+C) = AB + AC$ and $(A+B)C = AC + BC$.
        * Multiplicative Identity: $AI = IA = A$ (where $I$ is the identity matrix).
        * The product of two non-zero matrices can be a zero matrix.

5.  **Transpose of a Matrix ($A^T$ or $A'$):**
    * **Rule:** Rows become columns, and columns become rows.
    * **Formula:** If $A = [a_{ij}]$, then $A^T = [a_{ji}]$.
    * **Properties:**
        * $(A^T)^T = A$
        * $(A+B)^T = A^T + B^T$
        * $(kA)^T = kA^T$
        * $(AB)^T = B^T A^T$ (important property)

### V. Inverse of a Matrix

**Definition:** For a square matrix $A$, its inverse, denoted as $A^{-1}$, is a matrix such that when multiplied by $A$, it yields the identity matrix ($I$).
* **Formula:** $AA^{-1} = A^{-1}A = I$
* **Condition for Inverse:** A square matrix $A$ has an inverse if and only if its determinant is non-zero ($det(A) \neq 0$). Such a matrix is called a **non-singular matrix**. If $det(A) = 0$, the matrix is **singular** and its inverse does not exist.

#### A. Formula for Inverse of a Matrix (using Adjoint)

The formula for the inverse of a matrix A is:
$$A^{-1} = \frac{1}{det(A)} adj(A)$$
where:
* $det(A)$ is the determinant of matrix A.
* $adj(A)$ is the **adjoint** of matrix A.

**Steps to find $adj(A)$:**

1.  **Find the Matrix of Minors ($M$):** For each element $a_{ij}$, find its minor $M_{ij}$ (the determinant of the submatrix obtained by deleting the $i$-th row and $j$-th column).
2.  **Find the Matrix of Cofactors ($C$):** For each minor $M_{ij}$, calculate the cofactor $C_{ij} = (-1)^{i+j} M_{ij}$.
3.  **Find the Adjoint Matrix ($adj(A)$):** The adjoint of A is the transpose of the cofactor matrix ($adj(A) = C^T$).

**Example for 3x3 Matrix:**
If $A = \begin{bmatrix} a_{11} & a_{12} & a_{13} \\ a_{21} & a_{22} & a_{23} \\ a_{31} & a_{32} & a_{33} \end{bmatrix}$

**Step 1: Calculate $det(A)$** (as explained in Section I.B).

**Step 2: Calculate Cofactors:**
$C_{11} = (a_{22}a_{33} - a_{23}a_{32})$
$C_{12} = -(a_{21}a_{33} - a_{23}a_{31})$
$C_{13} = (a_{21}a_{32} - a_{22}a_{31})$
... and so on for all 9 elements.

**Step 3: Form the Cofactor Matrix ($C$):**
$C = \begin{bmatrix} C_{11} & C_{12} & C_{13} \\ C_{21} & C_{22} & C_{23} \\ C_{31} & C_{32} & C_{33} \end{bmatrix}$

**Step 4: Find the Adjoint Matrix ($adj(A)$):**
$adj(A) = C^T = \begin{bmatrix} C_{11} & C_{21} & C_{31} \\ C_{12} & C_{22} & C_{32} \\ C_{13} & C_{23} & C_{33} \end{bmatrix}$

**Step 5: Calculate the Inverse:**
$A^{-1} = \frac{1}{det(A)} \begin{bmatrix} C_{11} & C_{21} & C_{31} \\ C_{12} & C_{22} & C_{32} \\ C_{13} & C_{23} & C_{33} \end{bmatrix}$

### VI. Matrix Inverse Method to Solve a System of Linear Equations in 3 Variables

This method is used to solve systems of linear equations when the coefficient matrix is non-singular (i.e., its determinant is non-zero, and thus its inverse exists).

Consider the system of 3 linear equations in 3 variables:
$a_1x + b_1y + c_1z = d_1$
$a_2x + b_2y + c_2z = d_2$
$a_3x + b_3y + c_3z = d_3$

**Step 1: Write the system in Matrix Form:**
$AX = B$
where:
$A = \begin{bmatrix} a_1 & b_1 & c_1 \\ a_2 & b_2 & c_2 \\ a_3 & b_3 & c_3 \end{bmatrix}$ (coefficient matrix)
$X = \begin{bmatrix} x \\ y \\ z \end{bmatrix}$ (variable matrix)
$B = \begin{bmatrix} d_1 \\ d_2 \\ d_3 \end{bmatrix}$ (constant matrix)

**Step 2: Check for Consistency (Find $det(A)$):**
* Calculate $det(A)$.
* If $det(A) = 0$, the inverse does not exist, and the system cannot be solved by this method (it either has no solution or infinitely many solutions). Refer back to consistency conditions.
* If $det(A) \neq 0$, proceed to the next step.

**Step 3: Find the Inverse of Matrix A ($A^{-1}$):**
* Follow the steps outlined in Section V.A to calculate $A^{-1}$.

**Step 4: Solve for X:**
Multiply both sides of the matrix equation $AX = B$ by $A^{-1}$ from the left:
$A^{-1}(AX) = A^{-1}B$
$(A^{-1}A)X = A^{-1}B$
$IX = A^{-1}B$
$X = A^{-1}B$

**Step 5: Perform the Matrix Multiplication:**
Multiply the inverse matrix $A^{-1}$ by the constant matrix $B$ to get the solution matrix $X$.
$$\begin{bmatrix} x \\ y \\ z \end{bmatrix} = \left( \frac{1}{det(A)} adj(A) \right) \begin{bmatrix} d_1 \\ d_2 \\ d_3 \end{bmatrix}$$
The resulting matrix $X$ will give you the values of $x, y,$ and $z$.
