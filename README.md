# Diagnose and Defend: Lightweight Behavior-Aware Attention Gating for Robust Vision Transformers

> **CS231n Final Project – Stanford University (Winter 2025)** 

## Overview

Vision Transformers (ViTs) achieve strong performance on clean images but are notably vulnerable to adversarial perturbations. In this project, we propose a **modular, lightweight defense pipeline** that detects, diagnoses, and mitigates adversarial attacks using behavior-aware attention gating—without modifying the base ViT model or requiring adversarial training.

Our method:
- Detects adversarial inputs using CLS token embeddings
- Diagnoses the type of attention disruption via unsupervised clustering
- Applies gated attention correction in ViT Blocks 7–12 for targeted robustness
