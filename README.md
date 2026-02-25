# 📧 Spam Email Classification using Perceptron

## 🔹 Overview
This project demonstrates how a **single-layer Perceptron** can be used to classify emails as **Spam** or **Not Spam** based on two binary features:
- Presence of suspicious keywords
- Whether the sender is unknown

The project also visualizes the **decision boundary** learned by the perceptron.

---

## 📚 Problem Description
Each email is represented using two features:

| Feature | Description |
|--------|-------------|
| x₁ | Suspicious keywords present (1 = Yes, 0 = No) |
| x₂ | Unknown sender (1 = Yes, 0 = No) |

Target label:
- `1` → Spam  
- `0` → Not Spam  

Dataset follows the **OR logic**, which is linearly separable.

---

## 🧠 Perceptron Model
The perceptron learns a linear function:

\[
w \cdot x + b = 0
\]

### ✅ Final Trained Parameters
- **Weights:** `[0.1, 0.1]`
- **Bias:** `-0.1`

### ✏️ Final Decision Boundary
\[
0.1x_1 + 0.1x_2 - 0.1 = 0
\]

Simplified:
\[
x_1 + x_2 = 1
\]

---

## 📈 Visualization
- **X (cross)** → Spam emails  
- **O (circle)** → Not spam emails  
- **Straight line** → Decision boundary  

The plot clearly shows how the perceptron separates spam and non-spam emails using a linear boundary.

---

## 💻 Code Highlights
- Implements perceptron learning rule
- Plots training data points
- Draws the learned decision boundary
- Labels spam and non-spam classes clearly using legends

---

## ⚠️ Limitation
If the dataset becomes **non-linearly separable** (e.g., XOR pattern), the perceptron:
- Will **not converge**
- Cannot correctly classify the data

This highlights a key limitation of **single-layer perceptrons**.

---
