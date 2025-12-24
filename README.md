# Image Deconvolution with Tikhonov Regularization

This project studies **image deconvolution as an inverse problem**, using
**Tikhonov regularization techniques**, with a focus on **L2** and **H1** regularizations.

The goal is to recover a clean image starting from a **blurred and noisy observation**.

---

## 📌 Problem Description

Given an observed image:

\[
g = Kf + \eta
\]

where:
- \( f \) is the original image,
- \( K \) is a blur operator,
- \( \eta \) is additive noise,

the task is to **reconstruct the original image** \( f \).

This is an **ill-posed inverse problem**, which requires regularization.

---

## 🧠 Methodology

The project follows these steps:

1. Apply different **blur operators** to an image
2. Add **noise** to simulate real degradation
3. Recover the image using **Tikhonov regularization**
4. Compare:
   - **L2 regularization**
   - **H1 regularization**

The Tikhonov functional is defined as:

\[
\min_f \|Kf - g\|^2 + \lambda \|Lf\|^2
\]

where:
- \( L = I \) for L2 regularization
- \( L = \nabla \) for H1 regularization

---

## 🖼 Blur Models

The following blur types are considered:
- Gaussian blur
- Motion blur
- Uniform blur

---

## 🧪 Experiments

Experiments are conducted by:
- varying the blur type
- changing noise levels
- tuning the regularization parameter \( \lambda \)

The results are visually and quantitatively compared.

---
