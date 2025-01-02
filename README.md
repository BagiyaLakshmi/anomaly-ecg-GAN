# Anomaly Detection on ECG Using GAN

This project focuses on using Generative Adversarial Networks (GANs) for anomaly detection in ECG data. The primary goal is to address dataset imbalance by synthesizing ECG images and using the generated data alongside domain data to train a Convolutional Neural Network (CNN) for anomaly detection.

## Project Overview

- **Dataset Balancing:** The GAN is employed to generate synthetic ECG data, particularly for underrepresented classes, ensuring a balanced dataset for training.
- **Anomaly Detection Model:** A CNN model is built using both the generated synthetic data and the domain-specific ECG data to classify anomalies effectively.

## Key Components

### 1. GAN for Data Synthesis
The generator component of the GAN is trained to create realistic synthetic ECG data. Feedback from the discriminator guides the generator to improve its outputs until the discriminator cannot reliably distinguish between real and generated data.

- **Generator:** Learns to produce synthetic ECG data.
- **Discriminator:** Distinguishes between real and generated ECG data.

### 2. CNN for Anomaly Detection
A CNN is trained using the augmented dataset (real + synthetic ECG data) to detect anomalies in ECG signals with high accuracy.

## Project Workflow
1. **Data Preprocessing:**
   - Clean and preprocess the ECG dataset.
   - Identify and quantify imbalances in the dataset.

2. **GAN Model Implementation:**
   - Design and train the GAN to generate synthetic ECG images for underrepresented classes.

3. **Data Augmentation:**
   - Combine the synthetic ECG data with the real dataset to achieve a balanced distribution.

4. **CNN Model Implementation:**
   - Build and train a CNN using the augmented dataset.
   - Evaluate the model’s performance on anomaly detection tasks.

## Results
- **Data Synthesis:** Generated realistic ECG images, improving class distribution.
- **Anomaly Detection:** Achieved high accuracy and reliability in detecting anomalies using the CNN model.

