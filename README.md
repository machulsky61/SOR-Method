![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)

# Successive over-relaxation

This repository contains the implementation of a program to analyze the convergence of the **SOR** (_Successive Over-Relaxation_) method for solving linear systems, considering different values of the parameter ω. This is a [Computational Linear Algebra](https://github.com/machulsky61/linear-algebra) assignment.

## Table of Contents
- [Introduction](#introduction)
- [Usage](#usage)
- [Assingment instructions](#assingment-instructions)
- [Classmates](#classmates)
- [License](#license)

## Introduction

The _Successive Over-Relaxation_ (SOR) method is an iterative technique used to solve linear systems of equations, particularly those arising in numerical analysis and computational science. It's an extension of the Gauss-Seidel method, introducing a relaxation parameter $ω$ to accelerate convergence.

This method aims to find the solution to a system of linear equations by iteratively updating the solution vector until convergence is achieved. By adjusting the relaxation parameter $ω$, the method can converge faster than traditional iterative methods.

## Usage
   - **Numerical Analysis:** SOR is extensively used in numerical analysis for solving systems of linear equations arising from various mathematical models.
   - **Computational Science:** It finds applications in computational science, including fluid dynamics, structural analysis, and electromagnetics.
   - **Optimization:** commonly employed in optimization problems where solving linear systems is a crucial step.
   - **Engineering:** the method is also used for solving complex systems of equations in various engineering disciplines, such as mechanical, civil, and electrical engineering.

This method offers a balance between computational efficiency and convergence rate, making it a valuable tool in scientific computing and engineering applications.

## Assingment instructions

1. **Implementation of Jacobi Method:**
   - Write a program that implements the Jacobi method to solve a system $Ax = b$.
   - The program should receive the matrix $A$, vector $b$, an initial vector $x^{(0)}$, and the maximum number of iterations $s$.
   - It should terminate when the relative error is small: $\frac{||Ax^{(k)} = b||}{||b||} < 10^{-8}$ or when the maximum number of iterations is reached.
   - Return a list with the obtained solution and the number of iterations performed.

2. **Solving the System with Jacobi Method:**
   - Use the implemented program to solve a specific system.
   - Determine if convergence is achieved and in how many steps.

3. **Implementation of SOR Method:**
   - Modify the previous program to implement the SOR method for solving a system $Ax = b$.
   - Receive an additional parameter, the value $ω$.
   - SOR iteration: $x^{k+1} = (D+ωL)^{-1}(ωb - [ωU + (ω-1)D]x^{(k)})$

4. **Solving the System with SOR Method:**
   - Use the implemented program to solve the previous system with different values of $ω$.
   - Determine in which cases convergence is achieved and in how many steps.

5. **Verification of Jacobi Method Convergence:**
   - Build a random matrix and vectors.
   - Verify if the implemented Jacobi method converges for this matrix with a maximum number of iterations.

6. **Analysis of SOR Method for the Constructed Matrix:**
   - Run the SOR method for various values of $ω$ and record the number of steps for each.
   - Plot the number of steps as a function of $ω$.
   - Identify the interval of $ω$ values where convergence is obtained without exceeding the maximum number of iterations.
   - Determine the value of ω for which the fastest convergence is achieved.

7. **Calculation of Spectral Radius:**
   - Implement a program that returns the spectral radius of the SOR method matrix for a given matrix $A$ and value $ω$.

8. **Analysis of Spectral Radius:**
   - Calculate the spectral radius of the SOR method matrix for various values of $ω$ and plot its variation.
   - Identify the values of $ω$ where the spectral radius is less than $1$ and the value of $ω$ with the smallest spectral radius.

9. **Calculation of Determinant of SOR Method Matrix:**
   - Calculate the determinant of the SOR method matrix for various values of $ω$ and plot its variation.
   - Identify the values of $ω$ where the determinant is less than $1$ and the value of $ω$ with the smallest determinant.

## Classmates
- Agustín Hernández [@agushernandezz](https://github.com/agushernandezz)

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
