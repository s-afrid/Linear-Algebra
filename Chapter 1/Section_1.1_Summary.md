# Section 1.1 — Systems of Linear Equations

**Textbook:** *Linear Algebra and Its Applications, 5th Edition* — David C. Lay, Steven R. Lay, and Judi J. McDonald.

## 1. What is a linear equation?

A linear equation in variables \(x_1, x_2, \ldots, x_n\) has the general form

\[
a_1x_1 + a_2x_2 + \cdots + a_nx_n = b.
\]

For example,

\[
2x_1 + 3x_2 = 10.
\]

A **system of linear equations** is a collection of two or more linear equations involving the same variables. The objective is to find values of the variables that satisfy every equation simultaneously.

Example:

\[
\begin{cases}
x_1 + x_2 = 5,\\
2x_1 - x_2 = 4.
\end{cases}
\]

## 2. Geometric interpretation

- With two variables, equations represent lines.
- With three variables, equations represent planes.
- With more variables, equations represent higher-dimensional objects.

A solution is a point that satisfies all the equations. For example, when two lines intersect, their intersection point is the solution of the corresponding system.

## 3. Elementary row operations

The section introduces three operations for simplifying linear systems.

### 1. Row replacement

Replace one row by the sum of itself and a multiple of another row.

\[
R_2 \longrightarrow R_2 - 3R_1.
\]

### 2. Row interchange

Exchange two rows.

\[
R_1 \longleftrightarrow R_2.
\]

### 3. Row scaling

Multiply every entry in a row by a nonzero constant.

\[
R_1 \longrightarrow \frac{1}{2}R_1.
\]

These operations simplify equations without changing their solution set.

## 4. Augmented matrices

An augmented matrix is a compact representation of a linear system.

For example,

\[
\begin{cases}
x_1 + 2x_2 = 5,\\
3x_1 + 4x_2 = 11
\end{cases}
\]

can be represented as

\[
\left[
\begin{array}{cc|c}
1 & 2 & 5\\
3 & 4 & 11
\end{array}
\right].
\]

Instead of manipulating entire equations, we can perform elementary row operations directly on the matrix.

## 5. Row-equivalent matrices

Two matrices are called **row equivalent** if a sequence of elementary row operations transforms one matrix into the other.

**Important result:** If the augmented matrices of two linear systems are row equivalent, then the two systems have the same solution set.

Why? Elementary row operations are reversible and preserve the solutions.

## 6. Consistency and uniqueness

The section introduces two fundamental questions:

1. Is the system consistent? Does at least one solution exist?
2. If a solution exists, is it unique?

There are three possible outcomes.

### No solution — inconsistent

For example,

\[
0x_1 + 0x_2 = 5
\]

is impossible, so the system has no solution.

### One solution — consistent

The system determines exactly one combination of variable values.

### Infinitely many solutions — consistent

Multiple combinations of variable values satisfy all equations.

## 7. Numerical note

Computers solve linear systems using numerical algorithms and floating-point arithmetic. Because computers store numbers with finite precision, rounding and truncation can introduce small errors called **roundoff errors**.

This matters when solving large systems in engineering and scientific applications.

---

## Quick revision sheet

| Concept | What to remember |
|---|---|
| Linear equation | Equation involving variables with power 1 |
| Linear system | Collection of linear equations |
| Augmented matrix | Matrix representation of a linear system |
| Row replacement | Add a multiple of one row to another |
| Row interchange | Exchange two rows |
| Row scaling | Multiply a row by a nonzero constant |
| Row equivalent | Matrices connected by elementary row operations |
| Consistent | At least one solution exists |
| Inconsistent | No solution exists |
| Unique solution | Exactly one solution |

## Key takeaway

**Elementary row operations help simplify a system while preserving its solution set.**

## Exercises completed

Selected exercises from Section 1.1:

- 1–8
- 15–16

These covered solving systems, geometric interpretation, elementary row operations, solution sets, and consistency.
