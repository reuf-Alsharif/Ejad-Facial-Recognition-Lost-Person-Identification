# Ejad: Facial Recognition for Lost People Identification

**An AI-Based Approach to Identifying Lost Pilgrims During Hajj**

## Project Overview

Ejad is an AI-based project that explores the use of facial recognition to help identify lost pilgrims during the Hajj season. The proposed system combines Convolutional Neural Networks (CNNs) with a structured database of simulated pilgrim information to support identity matching and the retrieval of relevant details.

The project addresses challenges associated with crowded holy sites, language barriers, and the difficulties of assisting vulnerable groups, including children and elderly pilgrims.

## Project Objectives

- Explore facial image classification using deep learning.
- Compare three CNN architectures and evaluate their performance.
- Combine facial images with synthetic metadata representing pilgrim information.
- Demonstrate how facial predictions can be associated with campaign and supervisor details.
- Explore the potential of AI to support lost-person identification during Hajj and Umrah.

## Dataset

The study uses a facial image dataset obtained from Kaggle.

| Attribute | Description |
|---|---|
| Total images | 4,000 |
| Male images | 2,000 |
| Female images | 2,000 |
| Image resolution | 128 × 128 pixels |
| Data source | Kaggle |
| Metadata | Synthetically generated |

Synthetic metadata was generated to simulate pilgrim profiles, including names, countries, campaign names, supervisor names, and supervisor phone numbers.

**Dataset source:** [Face Dataset of People That Don't Exist – Kaggle](https://www.kaggle.com/datasets/bwandowando/all-these-people-dont-exist)

## Methodology

### 1. Image Preprocessing

Facial images were resized to 128 × 128 pixels and normalized to prepare them for model training.

### 2. Synthetic Metadata Generation

Fictitious profile information was generated to represent potential pilgrim records. Categorical metadata was encoded into numerical representations for integration into the experimental dataset.

### 3. CNN Model Development

Three CNN architectures with different network depths were developed and evaluated using TensorFlow and Keras.

The models were trained using:
- Adam optimizer
- Categorical cross-entropy loss
- Batch size of 32
- An 80:20 training/testing split

The report describes training runs of 20, 10, and 5 epochs for the three models, respectively.

### 4. Model Evaluation

The models were assessed using training and validation accuracy, loss, and confusion matrix analysis to compare performance and examine misclassifications.

## Results

The report presents the following model performance:

| Model | Training Accuracy | Validation Accuracy | Reported Loss |
|---|---:|---:|---:|
| Model 1 | 57% | 66% | 1.92% |
| Model 2 | 73% | 74% | 1.9% |
| Model 3 | 88% | 80% | 1.6% |

Model 3 achieved the highest training and validation accuracy, while Model 2 showed a more balanced performance according to the report's discussion. Model 3 also showed signs of overfitting.

## System Demonstration

The paper presents examples of predicted identities alongside associated synthetic metadata, including country, campaign, and supervisor information.

The proposed workflow illustrates how a facial image prediction could be connected to a corresponding profile to assist field teams in identifying and reuniting lost pilgrims with their groups.

## Technology Stack

- **Programming:** Python
- **Deep Learning:** Convolutional Neural Networks (CNNs)
- **Frameworks:** TensorFlow, Keras
- **Data Preparation:** Image normalization and categorical encoding
- **Evaluation:** Accuracy, loss, confusion matrix
- **Dataset:** Kaggle facial image dataset

## Limitations and Future Work

This project is an experimental prototype based on facial images and synthetic metadata. The results do not establish readiness for real-world identification or deployment during Hajj.

Potential future improvements include:
- Expanding the dataset with more diverse facial variations.
- Improving performance under different lighting and environmental conditions.
- Applying regularization and early stopping to reduce overfitting.
- Optimizing inference for real-time processing and edge devices.
- Evaluating the system using representative, independently collected data.
- Addressing privacy, security, and responsible use of facial recognition.

## Academic Context

**Project:** Ejad – Facial Recognition for Lost People Identification

**Focus:** Artificial Intelligence, Deep Learning, Computer Vision, and Hajj Crowd Management

