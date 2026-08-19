# Ultimate NumPy Visual Cheat Sheet & Guide

> An exhaustive, visual, and zero-fluff reference manual for NumPy fundamentals, operations, and linear algebra.

<p align="center">
  <a href="https://colab.research.google.com/github/AdhamAmgadElSharkawy/numpy-visual-guide/blob/main/learnnumpy.ipynb">
    <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab">
  </a>
  <img src="https://img.shields.io/badge/Python-3.10%2B-blue" alt="Python Version">
  <img src="https://img.shields.io/badge/NumPy-2.0%2B-green" alt="NumPy Version">
  <img src="https://img.shields.io/badge/License-MIT-yellow" alt="License">
</p>

---

## Visual Breakdowns (3D Animations)

NumPy arrays operate as multi-dimensional memory buffers. Here is how tensor manipulation, reduction axes, and broadcasting behave under the hood:

<table align="center">
  <tr>
    <td align="center" width="50%">
      <b>3D Tensor Slicing</b><br>
      <code>arr[0:2, 0:2, 1:3]</code>
    </td>
    <td align="center" width="50%">
      <b>Broadcasting Mechanics</b><br>
      <code>(3, 1) + (1, 3) ──> (3, 3)</code>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="assets/3d_slicing.gif" width="380" alt="3D Slicing Visual">
    </td>
    <td align="center">
      <img src="assets/3d_broadcasting.gif" width="380" alt="3D Broadcasting Visual">
    </td>
  </tr>
  <tr>
    <td colspan="2" align="center">
      <b>Understanding Axis Reductions</b><br>
      <code>axis=0</code> (down rows ⬇) vs. <code>axis=1</code> (across columns ➡)
    </td>
  </tr>
  <tr>
    <td colspan="2" align="center">
      <img src="assets/axis_concept.gif" width="450" alt="Axis Reduction Visual">
    </td>
  </tr>
</table>

---

## Table of Contents

The complete notebook is divided into **14 modular sections**, structured logically from zero to production linear algebra:

1. **[1. NumPy Basics & Array Creation](learnnumpy.ipynb)** — Vectors, matrices, shapes, and `.ndim`.
2. **[2. Built-in Initializers & Dtypes](learnnumpy.ipynb)** — `np.zeros`, `linspace` vs `arange`, type casting.
3. **[3. Indexing & Slicing](learnnumpy.ipynb)** — Sub-array extraction, striding, and stepping.
4. **[4. Memory: Views vs. Deep Copies](learnnumpy.ipynb)** — Shared memory buffers and mutation safety.
5. **[5. Reshaping, Transposing & Stacking](learnnumpy.ipynb)** — Inferred dimensions (`-1`), `vstack`, `hstack`.
6. **[6. Arithmetic & Vectorization](learnnumpy.ipynb)** — Scalar operations and high-performance universal functions.
7. **[7. Broadcasting Rules](learnnumpy.ipynb)** — Dimension expansion without copying data.
8. **[8. Aggregate & Statistical Functions](learnnumpy.ipynb)** — Axis-based reductions, `mean`, `std`, and `argmax`.
9. **[9. Handling Missing Data](learnnumpy.ipynb)** — NaN detection, finite filtering, and `nan`-safe metrics.
10. **[10. Filtering & Boolean Indexing](learnnumpy.ipynb)** — Masks, bitwise logic, and `np.where`.
11. **[11. Sorting & Unique Values](learnnumpy.ipynb)** — `np.sort`, argsort index mappings, and frequencies.
12. **[12. Random Numbers (np.random)](learnnumpy.ipynb)** — Modern `default_rng`, distributions, and sampling.
13. **[13. Linear Algebra (np.linalg)](learnnumpy.ipynb)** — Matrix products (`@`), determinants, and solvers.
14. **[14. Array File I/O](learnnumpy.ipynb)** — High-speed binary serialization (`.npy`) and plain CSVs.

---

## Quick Start

### 1. Run in Cloud (Zero Setup)
Click the badge below to run, edit, and experiment directly in your browser:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AdhamAmgadElSharkawy/numpy-visual-guide/blob/main/learnnumpy.ipynb)

### 2. Run Locally

```bash
# Clone the repository
git clone [https://github.com/AdhamAmgadElSharkawy/numpy-visual-guide.git](https://github.com/AdhamAmgadElSharkawy/numpy-visual-guide.git)
cd numpy-visual-guide

# Install required dependencies
pip install numpy matplotlib pillow

# Open the Jupyter notebook
jupyter notebook learnnumpy.ipynb
