# Secant Method Soup Cooling Simulation

This project demonstrates the implementation of the **Secant Method**, a numerical algorithm used to find roots of nonlinear equations.

The program models a real-world problem: estimating the time required for a hot soup to cool down to a desired temperature.

---

## Mathematical Model

The temperature of the soup is modeled using an exponential decay function:

T(t) = 20 + 70e^(-0.05t)

Where:

- 20°C represents room temperature
- 70°C is the initial temperature difference
- 0.05 is the cooling constant
- t is time in minutes

The goal is to determine when the soup reaches **40°C**.

This leads to solving the equation:

20 + 70e^(-0.05t) - 40 = 0

---

## Numerical Method

The program uses the **Secant Method**, an iterative technique for solving nonlinear equations.

Unlike methods that require derivatives (such as Newton's method), the Secant Method approximates the derivative using two previous points.

The iterative formula used is:

t₂ = t₁ − f(t₁)(t₁ − t₀) / (f(t₁) − f(t₀))

The algorithm continues iterating until the difference between successive approximations is smaller than the desired tolerance.

---

## Features

- implementation of the Secant Method in C#
- numerical root finding
- iterative approximation
- console output of iteration steps
- configurable tolerance and iteration limits

---

## Technology

- C#
- .NET Console Application
- Numerical Methods

---

## Example Output

The program prints the approximation at every iteration until it converges to the solution representing the cooling time.

---

## Educational Purpose

This project demonstrates how numerical algorithms can be applied to real-world problems such as thermal cooling processes.

It was developed as part of numerical methods practice and serves as a practical example of root-finding algorithms.
