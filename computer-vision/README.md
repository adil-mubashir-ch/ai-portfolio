# 👁️ Computer Vision

This directory contains my **applied and research-oriented projects in Computer Vision**, covering the full pipeline from **classical image processing** to **deep learning–based visual perception systems**.

The emphasis is on:

* **Understanding visual representations**
* **Building efficient and scalable models**
* **Analyzing performance under real-world constraints**
* **Deploying vision models on edge and embedded devices**

---

## 🎯 Scope & Objectives

Projects in this folder aim to:

* Implement **core computer vision tasks** from scratch and with modern frameworks
* Explore **architectural and training trade-offs**
* Evaluate **accuracy vs latency vs memory**
* Bridge the gap between **research results** and **deployable systems**

---

## 📂 Folder Structure

```
computer-vision/
│
├── mnist_digit_classification
│
└── README.md
```

Each subdirectory is **self-contained** and includes:

* Problem definition
* Dataset details
* Model architecture
* Training & evaluation scripts
* Results and analysis

---

## 🔍 Key Topics Covered

### 📌 Image Classification

* CNN architectures (ResNet, Efficient models)
* Training stability and regularization
* Performance benchmarking across datasets

### 📌 Object Detection

* Bounding box regression and classification
* Detector architecture trade-offs
* mAP-based evaluation and error analysis

### 📌 Segmentation

* Semantic segmentation pipelines
* Lightweight models for constrained environments
* Accuracy vs resolution trade-offs

### 📌 Vision on Edge

* Quantized inference (low-bit precision)
* Knowledge distillation for compact vision models
* Deployment using TensorFlow Lite and optimized runtimes

---

## 🧪 Experimental Philosophy

All experiments follow a **structured methodology**:

* Establish a **strong baseline**
* Apply **one change at a time**
* Report **quantitative metrics**
* Analyze **failure modes**
* Consider **deployment constraints**

Where relevant, experiments include:

* Ablation studies
* Accuracy recovery analysis
* Memory and latency profiling

---

## 🧠 Research Orientation

Some projects replicate or extend ideas from:

* Recent computer vision literature
* Model compression and efficiency research
* Edge AI and TinyML studies

The goal is not just to reproduce results, but to **understand why they work** and **when they fail**.

---

## 🛠️ Tools & Frameworks

Commonly used tools across projects:

* PyTorch / TensorFlow
* OpenCV
* NumPy, Matplotlib
* TensorFlow Lite
* CUDA (where applicable)

---

## 🚀 Future Work

Planned extensions include:

* Multi-task vision models
* Vision transformers on constrained hardware
* Real-time perception pipelines for robotics
* Robustness and out-of-distribution testing

---

## ⭐ Why This Folder Matters

Computer Vision is foundational to **Robotics, Autonomous Systems, and Edge AI**.
This folder represents my approach to building **accurate, efficient, and deployable visual systems**, grounded in both **theory and practice**.