# Diagnose and Defend: Lightweight Behavior-Aware Attention Gating for Robust Vision Transformers

> **CS231n Final Project – Stanford University (Spring 2025)** 

## Authors

- **Yanny Gao** – [rgao1218@stanford.edu](mailto:rgao1218@stanford.edu)  
- **Sara Kothari** – [sarako@stanford.edu](mailto:sarako@stanford.edu)  
- **Natalie Kuo** – [nskuo@stanford.edu](mailto:nskuo@stanford.edu)

## Overview

Vision Transformers (ViTs) achieve strong performance on clean images but are notably vulnerable to adversarial perturbations. In this project, we propose a **modular, lightweight defense pipeline** that detects, diagnoses, and mitigates adversarial attacks using behavior-aware attention gating—without modifying the base ViT model or requiring adversarial training.

## Key Components

- **Universal Adversarial Patch:** Suppresses object detection on DETR via patch optimization.
- **CLS-Token Detector:** MLP-based binary classifier using Block 6 CLS token to detect adversarial inputs.
- **Attention Diagnoser:** PCA + K-Means clustering identifies behavioral disruption types (e.g. shifting, attenuation).
- **Adaptive Gating:** Cluster-guided attention correction applied in ViT Blocks.


