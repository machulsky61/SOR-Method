![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)

# SOR Method - Linear Algebra Assignment

This repository contains the implementation of a program to analyze the convergence of the SOR (Successive Over-Relaxation) method for solving linear systems, considering different values of the parameter ω.

## Instructions

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
