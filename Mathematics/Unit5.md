

## UNIT - V: Differential Equations and MATLAB Introduction

This unit introduces the basics of differential equations, a powerful mathematical tool for modeling dynamic systems, and provides a foundational look at MATLAB, a versatile computational software.

### I. Differential Equations

#### A. Definition of a Differential Equation

* **Definition:** A differential equation is an equation that relates one or more functions and their derivatives.
* **Order of a Differential Equation:** The order of the highest derivative present in the equation.
    * Example: $\frac{d^2y}{dx^2} + 5\frac{dy}{dx} + 6y = \sin x$ (Order 2)
* **Degree of a Differential Equation:** The highest power of the highest order derivative after the equation has been made free from radicals and fractions, as far as derivatives are concerned.
    * Example: $\left(\frac{dy}{dx}\right)^3 + y = x$ (Degree 3)
    * Example: $\frac{d^2y}{dx^2} + \sqrt{\frac{dy}{dx}} = x \Rightarrow \frac{d^2y}{dx^2} = x - \left(\frac{dy}{dx}\right)^{1/2} \Rightarrow \left(\frac{d^2y}{dx^2}\right)^2 = \left(x - \sqrt{\frac{dy}{dx}}\right)^2$. Here, the highest derivative is $\frac{d^2y}{dx^2}$ and its power is 2. (Degree 2).
* **First Order and First Degree Differential Equation:** An equation involving only the first derivative, raised to the power of one.
    * General Form: $\frac{dy}{dx} = f(x, y)$ or $M(x,y) dx + N(x,y) dy = 0$.

#### B. Solution of First Order and First Degree Differential Equation by Variable Separation Method (Simple Problems)

* **Concept:** The variable separation method is a technique used to solve first-order differential equations where the terms involving the dependent variable ($y$) and its differential ($dy$) can be grouped on one side of the equation, and the terms involving the independent variable ($x$) and its differential ($dx$) can be grouped on the other side.
* **Method (Steps):**
    1.  **Rearrange the equation:** Given $\frac{dy}{dx} = f(x, y)$, try to rewrite it in the form:
        $$g(y) \, dy = h(x) \, dx$$
        where $g(y)$ is a function of $y$ only, and $h(x)$ is a function of $x$ only.
    2.  **Integrate both sides:** Integrate each side with respect to its respective variable.
        $$\int g(y) \, dy = \int h(x) \, dx$$
    3.  **Add the constant of integration:** After integrating, add a single constant of integration ($C$) to one side (conventionally, the right-hand side).
    4.  **Solve for y (if possible):** Express $y$ explicitly in terms of $x$, if the resulting equation allows for it. Otherwise, leave it in implicit form.

* **Formula (General Form):**
    If a differential equation can be written as $\frac{dy}{dx} = f(x) \cdot g(y)$, then separate variables as $\frac{dy}{g(y)} = f(x) \, dx$.
    Integrate to get: $\int \frac{1}{g(y)} \, dy = \int f(x) \, dx + C$.

* **Simple Examples:**

    1.  **Example 1:** Solve $\frac{dy}{dx} = \frac{x^2}{y^2}$
        * **Step 1 (Separate variables):**
            $y^2 \, dy = x^2 \, dx$
        * **Step 2 (Integrate both sides):**
            $\int y^2 \, dy = \int x^2 \, dx$
            $\frac{y^3}{3} = \frac{x^3}{3} + C'$
        * **Step 3 (Rearrange for solution):**
            $y^3 = x^3 + 3C'$
            Let $3C' = C$ (another arbitrary constant)
            $y^3 = x^3 + C$
            $y = \sqrt[3]{x^3 + C}$

    2.  **Example 2:** Solve $\frac{dy}{dx} = \frac{1+y^2}{1+x^2}$
        * **Step 1 (Separate variables):**
            $\frac{dy}{1+y^2} = \frac{dx}{1+x^2}$
        * **Step 2 (Integrate both sides):**
            $\int \frac{1}{1+y^2} \, dy = \int \frac{1}{1+x^2} \, dx$
            $\tan^{-1}(y) = \tan^{-1}(x) + C$
        * **Step 3 (Solve for y):**
            $y = \tan(\tan^{-1}(x) + C)$

    3.  **Example 3:** Solve $\frac{dy}{dx} = e^{x+y}$
        * **Step 1 (Separate variables):**
            Recognize $e^{x+y} = e^x \cdot e^y$.
            $\frac{dy}{e^y} = e^x \, dx$
            $e^{-y} \, dy = e^x \, dx$
        * **Step 2 (Integrate both sides):**
            $\int e^{-y} \, dy = \int e^x \, dx$
            $-e^{-y} = e^x + C$
        * **Step 3 (Solve for y):**
            $e^{-y} = -e^x - C$
            $-y = \ln(-e^x - C)$
            $y = -\ln(-e^x - C)$

### II. MATLAB – Simple Introduction

MATLAB (Matrix Laboratory) is a proprietary multi-paradigm programming language and numerical computing environment. It's widely used in engineering, science, and economics for tasks like numerical analysis, data visualization, algorithm development, and matrix manipulation.

#### A. Key Characteristics of MATLAB

* **High-Level Language:** Designed for mathematical and engineering tasks.
* **Interactive Environment:** Provides a command-line interface for quick calculations and a graphical user interface (GUI) for more complex tasks.
* **Matrix-Based:** Data is primarily handled as arrays or matrices, making matrix operations very intuitive and efficient.
* **Extensible:** Users can write their own functions and scripts (M-files).
* **Toolboxes:** Offers specialized toolboxes for various applications (e.g., Signal Processing, Control Systems, Statistics, Machine Learning, Symbolic Math).
* **Visualization:** Excellent capabilities for plotting 2D and 3D graphs.

#### B. MATLAB Environment Components (Simple Introduction)

When you open MATLAB, you typically see several windows:

1.  **Command Window:**
    * This is where you type commands directly and see the immediate results.
    * Example:
        ```matlab
        >> 2 + 3
        ans = 5
        >> a = 10
        a = 10
        >> b = [1 2; 3 4] % Define a 2x2 matrix
        b =
             1     2
             3     4
        >> b*2
        ans =
             2     4
             6     8
        ```
2.  **Command History:**
    * Shows a list of commands you've typed in the Command Window. Useful for re-running commands.
3.  **Workspace:**
    * Lists all variables currently in memory, along with their values and data types.
    * You can inspect variables by double-clicking them.
4.  **Current Folder (or Current Directory):**
    * Displays the files in the current working directory. MATLAB looks for scripts and functions in this directory.
    * It's important to set this to the folder where your script files (.m files) are located.
5.  **Editor (or Live Editor):**
    * Used to write, edit, and save MATLAB scripts (sequences of commands) and functions.
    * Scripts are saved with a `.m` extension (e.g., `myscript.m`).

#### C. Simple MATLAB Commands and Operations

* **Basic Arithmetic:** `+`, `-`, `*`, `/`, `^` (power)
    * `>> 5 * (4 + 2) / 3`
* **Variable Assignment:** `=`
    * `>> x = 5;` (semicolon suppresses output)
    * `>> greeting = 'Hello, world!';`
* **Creating Vectors/Matrices:**
    * **Row Vector:** `>> v_row = [1 2 3 4]`
    * **Column Vector:** `>> v_col = [1; 2; 3; 4]`
    * **Matrix:** `>> M = [1 2 3; 4 5 6; 7 8 9]`
    * `zeros(m, n)`: Creates an $m \times n$ matrix of zeros.
    * `ones(m, n)`: Creates an $m \times n$ matrix of ones.
    * `eye(n)`: Creates an $n \times n$ identity matrix.
    * `rand(m, n)`: Creates an $m \times n$ matrix of random numbers.
* **Matrix Operations:**
    * `A * B`: Matrix multiplication.
    * `A .* B`: Element-wise multiplication.
    * `A + B`, `A - B`: Matrix addition/subtraction.
    * `A'` or `transpose(A)`: Transpose of matrix A.
    * `inv(A)`: Inverse of matrix A.
    * `det(A)`: Determinant of matrix A.
* **Built-in Functions:** MATLAB has a vast library of functions.
    * `sin(x)`, `cos(x)`, `tan(x)`
    * `sqrt(x)`: Square root.
    * `exp(x)`: Exponential function $e^x$.
    * `log(x)`: Natural logarithm (base $e$). `log10(x)` for base 10.
    * `abs(x)`: Absolute value.
    * `sum(V)`: Sum of elements in vector V.
    * `mean(V)`: Mean of elements in vector V.
    * `max(V)`, `min(V)`: Maximum/minimum element.
* **Plotting (Simple):**
    * `plot(x, y)`: Plots 2D data.
    * `xlabel('X-axis')`, `ylabel('Y-axis')`, `title('My Plot')`
    * `grid on`: Adds a grid.
    * Example script (`plot_example.m`):
        ```matlab
        x = 0:0.1:2*pi; % Create a vector from 0 to 2*pi with step 0.1
        y = sin(x);
        plot(x, y);
        xlabel('Angle (radians)');
        ylabel('sin(Angle)');
        title('Sine Wave');
        grid on;
        ```
* **Comments:** Use `%` for single-line comments.

#### D. Solving Simple Differential Equations in MATLAB (Conceptual / Basic `dsolve` or Numerical)

While the focus of the differential equations part is on manual variable separation, MATLAB can solve them symbolically or numerically.

* **Symbolic Solutions (using `dsolve` from Symbolic Math Toolbox):**
    * First, define symbolic variables using `syms`.
    * `dsolve` can find analytical solutions for many differential equations.
    * Example: Solve $\frac{dy}{dx} = \frac{x^2}{y^2}$
        ```matlab
        syms y(x) % Define y as a function of x
        eqn = diff(y, x) == x^2/y^2;
        sol = dsolve(eqn);
        disp(sol);
        % The output will show the solution, often implicitly.
        % ans = (x^3 + 3*C1)^(1/3)
        ```
* **Numerical Solutions (using `ode45` for Initial Value Problems):**
    * For more complex differential equations that don't have simple analytical solutions, MATLAB's ODE solvers (like `ode45`) can find numerical approximations. This is beyond "simple introduction" but good to know it exists.
