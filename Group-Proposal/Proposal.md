# Project Proposal: Conditional GAN for On-Demand Shoe Generation

**Date:** November 7, 2025

**Status:** Draft

---

##  Team Members

* Tejas Nisar
* Jasreen Kaur Mehta
* Mohammed Ismail Sarfaraz Shaik

---

##  Project Overview

This project aims to implement, train, and deploy a **Conditional Generative Adversarial Network (cGAN)**. The model will be trained on the **UT Zappos 50k shoe dataset**.

The final objective is to create an interactive web application where a user can provide a simple prompt (e.g., "men's boot," "women's high-heel") and the model will generate a novel, corresponding shoe image.

---

##  Key Objectives

1.  **Implement:** Successfully build a functional and stable cGAN architecture (Generator and Discriminator).
2.  **Train:** Train the model on the Zappos 50k dataset, conditioning the generation process on shoe attributes (like category or style).
3.  **Generate:** Achieve plausible, high-quality image generation that matches the given conditional prompt.
4.  **Demo:** Develop an accessible and intuitive user interface using Streamlit to demonstrate the model's capabilities.

---

##  Project Phases

Our workflow is divided into three main phases:

### Phase 1: Building & Data Preparation
* **Data:** Acquire and preprocess the UT Zappos 50k dataset. This includes resizing images, normalization, and extracting/formatting the conditional labels (e.g., shoe categories).
* **Model:** Design and implement the cGAN architecture in Python using a deep learning framework (like PyTorch or TensorFlow).

### Phase 2: Training & Evaluation
* **Training:** Train the model, carefully monitoring for stability, discriminator/generator loss, and avoiding common issues like mode collapse.
* **Evaluation:** Qualitatively and (if time permits) quantitatively evaluate the generated images for realism, diversity, and adherence to the conditional prompt.

### Phase 3: Demo Deployment
* **Interface:** Build a simple web application using **Streamlit**.
* **Integration:** Load the pre-trained generator model into the Streamlit app.
* **Final Demo:** Create the final user-facing demo that allows users to select a shoe category (the prompt) and receive a generated image.

---

##  Dataset

* **Primary Dataset:** UT Zappos 50k (Zappos50k)
* **Description:** A large-scale shoe dataset with over 50,000 catalog images. Crucially, it includes rich metadata (e.g., categories, materials, styles) which will serve as the "conditions" for our cGAN.
* **Source:** [https://vision.cs.utexas.edu/projects/finegrained/utzap50k/](https://vision.cs.utexas.edu/projects/finegrained/utzap50k/)
* **Citations:** 
    * A. Yu and K. Grauman. "Fine-Grained Visual Comparisons with Local Learning". In CVPR, 2014.
    * A. Yu and K. Grauman. "Semantic Jitter: Dense Supervision for Visual Comparisons via Synthetic Images". In ICCV, 2017.

---
