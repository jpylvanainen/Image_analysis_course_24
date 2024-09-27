# Day 2: Key Topics

- What is Deep Learning?
- What is ZerocostDL4Mic?
- How can you use ZerocostDL4Mic?
- Example of deep learning in microscopy: Analyzing cancer cell behavior in microfluidics.
- Quality control in deep learning: From dataset validation to model performance monitoring.
- Tools available in ZerocostDL4Mic for segmentation, denoising, and super-resolution.
- By the end of the lecture, you’ll have a comprehensive understanding of how ZerocostDL4Mic can help streamline and democratize deep learning for microscopy, and how to start your own deep learning projects in this domain.

**Instructors** 

Joanna Pylvänäinen, Åbo Akademi University, joanna.pylvanainen@abo.fi <br /> Sujan Ghimire, Åbo Akademi University, sujan.ghimire@abo.fi

## Session 1: Lecture: ZerocostDL4Mic: Leveraging Deep Learning for Microscopy Image Analysis

In this lecture, we will explore ZerocostDL4Mic, a powerful and accessible toolbox designed to help researchers and students train deep learning models for microscopy image analysis. We will start with an introduction to deep learning and its applications in microscopy, followed by a detailed discussion of how ZerocostDL4Mic simplifies the process of building and applying neural networks, even for those with limited computational resources.

**You'll learn about:**

- The common deep learning tasks in microscopy, particularly Convolutional Neural Networks (CNN).
- The steps involved in training models from scratch versus using transfer learning.
- How data augmentation can improve model performance.
- The importance of quality control in deep learning models, with a focus on validation and model testing.
- The lecture will feature a practical demonstration, showing how to set up and train a neural network using ZerocostDL4Mic through Google Colab's free GPU resources. We will also showcase an example experiment analyzing pancreatic cancer cell adhesion and migration.

## Session 2: Hands-on: How to prepare a dataset for StarDist

In this hands-on session, you will learn how to prepare data for deep learning and train a deep learning model using ZeroCostDL4Mic. This practical training will guide you through the process of annotating images, setting up a training dataset, and utilizing the StarDist model to segment cells in microscopy images. You will use Google Colab and ZeroCostDL4Mic to simplify the model training process, leveraging free GPU resources.

> **[Download image for annotation](https://drive.google.com/file/d/1FU4nRPN_vD2uP5bvoc05KnmA4ZPmgagy/view?usp=drive_link)**
> **[Download T cell dataset](https://drive.google.com/drive/folders/16_z9sDaI7mlteWcOZJcTWPT0lx-GldMK?usp=drive_link)**
> **[Download Breast cancer dataset](https://drive.google.com/drive/folders/1N5l_wKl4gD6SPQUJE7bb1sC7I8VQAX4Q?usp=drive_link)**

**You'll learn about:**

- Preparing and annotating data for deep learning in microscopy
- The importance of high-quality training datasets
- Step-by-step guide on how to create a training dataset for the StarDist model using Fiji
- Folder structure organization for training data in StarDist
- Using ZeroCostDL4Mic on Google Colab to train a StarDist model for cell segmentation

By the end of this session, you'll have hands-on experience in training your own deep learning model and applying it to microscopy data.

## Session 3: Hands-on: How to evaluate the quality of your model

In this hands-on session, , we will focus on Quality Control (QC) for deep learning (DL) models, particularly in the context of DL-based segmentation in microscopy. Ensuring that models perform accurately and generalize well beyond the training data is crucial. This session will walk you through the importance of quality control in deep learning, the steps to evaluate model performance, and how to inspect model outputs through various QC methods.

**You'll learn about:**

- Why Quality Control is Essential: Understanding the role of QC in reducing errors, detecting biases, and ensuring model robustness.
- Steps in Quality Control: How to monitor training and validation loss, prevent overfitting, and determine when further training is no longer necessary.
- Visual Inspection and Error Mapping: Learn to visually inspect the loss function, map errors, and use quality metrics like IoU (Jaccard Index), F1 score (Dice Coefficient), and mean matched score.
- Model Evaluation: Comparing different models trained with various numbers of epochs to assess their performance and track accuracy using TrackMate.

By the end of this session, you will be equipped to conduct thorough quality control checks on your own models, ensuring that they perform well on unseen data and are reliable for real-world applications.

## Session 4: Hands-on: Applying StarDist to unseen dataset

In Part 3 of this hands-on session, we will focus on applying a trained deep learning model to unseen data. You will learn how to choose a model based on its training history and apply it to a new dataset for cell segmentation and tracking. 

**You'll learn about:**

- Model Selection for Unseen Data: How to select the most appropriate model from a list of options (trained with different epochs) to apply to new data.
- Batch Processing: Applying the chosen model to a whole folder of images for efficient data analysis.

By the end of this session, you'll be able to confidently apply your trained models to new datasets, perform tracking, and complete your image analysis workflow.


