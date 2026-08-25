# AI-Defect-Detection-System
🔍 AI-powered manufacturing quality inspection system using Deep Learning, EfficientNet, FastAPI, Streamlit, MLflow, and ONNX for real-time defect detection.
# 🔍 AI Defect Detection System

> **An AI-powered automated quality inspection system that detects defective products from images using Deep Learning and Computer Vision.**

![Python](https://img.shields.io/badge/Python-3.10+-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-Deep%20Learning-red)
![FastAPI](https://img.shields.io/badge/FastAPI-REST%20API-green)
![Streamlit](https://img.shields.io/badge/Streamlit-Dashboard-orange)
![Computer Vision](https://img.shields.io/badge/Computer%20Vision-AI-purple)

---

## 📌 Overview

Manual quality inspection in manufacturing environments can be time-consuming, inconsistent, and difficult to scale.

The **AI Defect Detection System** leverages **Deep Learning and Computer Vision** to automatically analyze product images and classify them as:

- ✅ **Good**
- ⚠️ **Defective**

The system provides an end-to-end machine learning pipeline, including data preprocessing, augmentation, model training, inference, experiment tracking, REST API deployment, and an interactive analytics dashboard.

---

## 🎯 Problem Statement

Traditional quality inspection often relies on manual human inspection.

This can lead to:

- Human errors
- Inconsistent quality assessment
- Slow inspection processes
- Difficulty scaling production
- Increased operational costs

This project addresses these challenges by developing an AI-powered automated inspection system capable of analyzing product images and identifying potential defects.

---

## 💡 Solution

The system processes an input image using a trained Deep Learning model and predicts whether the product is **Good** or **Defective**.

### System Workflow

```text
                ┌─────────────────┐
                │  Product Image  │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │ Image Processing│
                │ & Augmentation  │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │ Deep Learning   │
                │ EfficientNet-B3 │
                └────────┬────────┘
                         │
                         ▼
              ┌──────────┴──────────┐
              │                     │
              ▼                     ▼
        ┌──────────┐          ┌──────────┐
        │   GOOD   │          │DEFECTIVE │
        └──────────┘          └──────────┘
              │                     │
              └──────────┬──────────┘
                         ▼
                ┌─────────────────┐
                │ Dashboard / API │
                └─────────────────┘
