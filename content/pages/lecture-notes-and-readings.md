---
content_type: page
description: This page includes lecture notes and readings for each lecture.
draft: false
title: Lecture Notes and Readings
uid: d37b3aa2-ff0c-4286-b7ce-b7e4f3fbb2ea
---
## Lecture 1

### Lecture Notes

- Part 1: Introduction (PDF)
- Part 2: Derivatives as Linear Operators \[notes not available\]

### Further Readings:

- [matrixcalculus.org](http://www.matrixcalculus.org/) is a fun site to play with derivatives of matrix and vector functions. 
- [The Matrix Cookbook (PDF)](https://www.math.uwaterloo.ca/~hwolkowi/matrixcookbook.pdf) has a lot of formulas for these derivatives, but no derivations.
- [Vector and Matrix Differentiation (PDF)](https://cdn-uploads.piazza.com/paste/j779e63owl53k6/04b2cb8c2f300212d723bea822a6b856085b28e28ca9debc75a05761a436499c/6.S087_Lecture_2.pdf)
- **Fancier math**: The perspective of derivatives as linear operators is sometimes called a [Fréchet derivative](https://en.wikipedia.org/wiki/Fr%C3%A9chet_derivative) and you can find lots of very abstract (what I'm calling "fancy") presentations of this online, chock full of weird terminology whose purpose is basically to generalize the concept to weird types of vector spaces. The "little-o notation" o(δx) we're using here for "infinitesimal asymptotics" is closely related to the [asymptotic notation](https://en.wikipedia.org/wiki/Big_O_notation) used in computer science, but in computer science people are typically taking the limit as the argument (often called "n") becomes very *large* instead of very small. A fancy name for a row vector is a "covector" or [linear form](https://en.wikipedia.org/wiki/Linear_form), and the fancy version of the relationship between row and column vectors is the [Riesz representation theorem](https://en.wikipedia.org/wiki/Riesz_representation_theorem), but until you get to non-Euclidean geometry you may be happier thinking of a row vector as the transpose of a column vector.

## Lecture 2

### Lecture Notes

- Part 1: Derivatives as Linear Operators (cont.) \[notes not available\]
- Part 2: [Two by Two Matrix Jacobians](https://rawcdn.githack.com/mitmath/matrixcalc/7340d2a7d40e6548a5ca0945ecae96cbac659929/2x2Jacobians.jl.html)

### Further Readings:

- The terms "forward-mode" and "reverse-mode" differentiation are most prevalent in [automatic differentiation (AD)](https://en.wikipedia.org/wiki/Automatic_differentiation), which will will cover later in this course. You can find many, many articles online about [backpropagation](https://en.wikipedia.org/wiki/Backpropagation) in neural networks. There are many other versions of this, e.g. in differential geometry the derivative linear operator (multiplying Jacobians and perturbations dx right-to-left) is called a [pushforward](https://en.wikipedia.org/wiki/Pushforward_(differential)), whereas multiplying a gradient row vector (covector) by a Jacobian left-to-right is called a [pullback](https://en.wikipedia.org/wiki/Pullback_(differential_geometry)). This [video on "Understanding Automatic Differentiation"](https://www.youtube.com/watch?v=UqymrMG-Qi4) by [Dr. Mohamed Tarek](https://github.com/mohamed82008) also starts with a similar left-to-right (reverse) vs right-to-left (forward) viewpoint and goes into how it translates to Julia code, and how you define custom chain-rule steps for Julia AD.

## Lecture 3

### Lecture Notes

- Part 1: The Gradient of a Scalar Function of a Vector: Column Vector or Row Vector? (PDF)
- Part 2: [Finite-Difference](https://nbviewer.org/github/mitmath/matrixcalc/blob/main/Finite%20difference%20checks.ipynb)

### Further Readings:

- Wikipedia has a useful list of [properties of the matrix trace](https://en.wikipedia.org/wiki/Trace_(linear_algebra)#Properties). The "matrix dot product" introduced today is also called the [Frobenius inner product](https://en.wikipedia.org/wiki/Frobenius_inner_product), and the corresponding norm ("length" of the matrix viewed as a vector) is the [Frobenius norm](https://mathworld.wolfram.com/FrobeniusNorm.html). When you "flatten" a matrix A by stacking its columns into a single vector, the result is called [vec(A)](https://en.wikipedia.org/wiki/Vectorization_(mathematics)), and many important linear operations on matrices can be expressed as [Kronecker products](https://en.wikipedia.org/wiki/Kronecker_product). The [Matrix Cookbook](https://www.math.uwaterloo.ca/~hwolkowi/matrixcookbook.pdf) has lots of formulas for derivatives of matrix functions. There is a lot of information online on [finite difference approximations](https://en.wikipedia.org/wiki/Finite_difference), [notes on finite differences (PDF)](https://github.com/mitmath/18303/blob/fall16/difference-approx.pdf), or [Section 5.7 of *Numerical Recipes*](http://www.it.uom.gr/teaching/linearalgebra/NumericalRecipiesInC/c5-7.pdf). The Julia [FiniteDifferences.jl package](https://github.com/JuliaDiff/FiniteDifferences.jl) provides lots of algorithms to compute finite-difference approximations; a particularly robust and powerful way to obtain high accuracy is to employ [Richardson extrapolation](https://github.com/JuliaDiff/FiniteDifferences.jl#richardson-extrapolation) to smaller and smaller δx. If you make δx too small, the finite precision (#digits) of [floating-point arithmetic](https://en.wikipedia.org/wiki/Floating-point_arithmetic) leads to [catastrophic cancellation errors](https://en.wikipedia.org/wiki/Catastrophic_cancellation).

## Lecture 4

### Lecture Notes

- Part 1: Derivative of Matrix Determinant and Inverse
- Part 2: Nonlinear Root-Finding, Optimization, and Adjoint-Method Differentiation

### Further Readings:

- read

## Lecture 5

### Lecture Notes

- Automatic Differentiation

### Further Readings:

- read

## Lecture 6

### Lecture Notes

- Part 1: Derivatives of Eigenproblems
- Part 2: Second Derivatives, Bilinear Forms, and Hessian Matrices

### Further Readings:

- read

## Lecture 7

### Lecture Notes

- Part 1: Hessian Matrices (cont.)
- Part 2: Derivatives and Backpropagation on Graphs and Linear Operators

### Further Readings:

- read

## Lecture 8

### Lecture Notes

- Part 1: Hessian Matrices (cont.)
- Part 2: Differentiable Programming and Neural Differential Equations

### Further Readings:

- read