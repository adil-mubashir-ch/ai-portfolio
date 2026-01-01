# 🧮 MNIST Digit Classification — Multi-Framework Baseline

This project implements **handwritten digit classification on the MNIST dataset** using three major deep learning frameworks:

* **TensorFlow**
* **PyTorch**
* **Keras**

The goal is to establish a **clear, minimal, and comparable baseline** for image classification that can serve as:

* A learning reference
* A framework comparison
* A reusable template for future vision projects

---

## 📊 About the Dataset

**MNIST** is a benchmark dataset consisting of:

* **70,000 grayscale images** of handwritten digits (0–9)
* Image size: **28 × 28**
* **60,000 training samples**
* **10,000 test samples**

MNIST is often considered the *“Hello World”* of computer vision and is widely used to validate training pipelines, preprocessing strategies, and model correctness.

---

## 🎯 Objectives of This Notebook

* Implement the **same neural architecture** across multiple frameworks
* Compare **training pipelines**, not just results
* Demonstrate **standard vision preprocessing practices**
* Provide a **clean baseline** for extending into CNNs, quantization, or edge deployment

---

## 🧠 Model Architecture

All three implementations use an identical **Multi-Layer Perceptron (MLP)** architecture:

```
Input (784)
 → Dense(512) + ReLU
 → Dense(256) + ReLU
 → Dense(10)  + Softmax
```

Why MLP instead of CNN?

* Keeps the focus on **framework mechanics**
* Makes performance differences easier to reason about
* Serves as a baseline before introducing convolutional layers

---

## 🛠️ Implementations

### 🔹 TensorFlow

* Uses `tf.keras.Sequential`
* Dataset loaded via `tf.keras.datasets.mnist`
* Loss: `SparseCategoricalCrossentropy`
* Optimizer: `Adam`

### 🔹 PyTorch

* Custom `nn.Module` implementation
* Manual training loop
* Dataset handled via `torchvision.datasets.MNIST`
* Loss: `CrossEntropyLoss`
* Optimizer: `Adam`

### 🔹 Keras

* High-level API with minimal boilerplate
* One-hot encoded labels
* Backend-agnostic model definition
* Optimizer: `Adam`

---

## 📈 Results

All three frameworks achieve **~97–98% test accuracy** after 10 epochs, demonstrating:

* Correct preprocessing
* Stable training
* Comparable performance across frameworks

Minor differences arise due to:

* Weight initialization
* Batch size choices
* Training loop implementation details

---

## 🧪 Key Takeaways

* Framework choice affects **developer experience**, not core model capability
* PyTorch offers **maximum control** via explicit training loops
* TensorFlow/Keras provide **faster prototyping**
* A consistent baseline simplifies future experimentation

---

## 🚀 Extensions & Future Work

This notebook is intentionally simple and serves as a foundation for:

* CNN-based MNIST models
* Quantization-aware training
* Knowledge distillation experiments
* Edge deployment (TensorFlow Lite)
* Latency and memory profiling

---

## 📌 Why This Project Exists

Rather than optimizing for state-of-the-art accuracy, this notebook focuses on:

* **Clarity**
* **Reproducibility**
* **Framework comparison**
* **Portfolio readability**

It sets a standard structure reused across other vision projects in this repository.

