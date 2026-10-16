# IoT Network Intrusion Detection

A machine learning project that detects cyberattacks in IoT network traffic and compares how different models perform on the task.

## Problem

Smart home and IoT devices are common targets for cyberattacks such as botnets and denial-of-service attacks. Manually monitoring their network traffic is not practical, so automated systems are needed to tell normal traffic apart from malicious traffic.

## Objective

- Detect whether a network flow is **normal or an attack** (binary classification).
- Identify the **type of attack**: DoS, MITM ARP Spoofing, Mirai, Scan, or Normal (multiclass classification).
- Compare a **Decision Tree**, **Gaussian Naive Bayes**, and a **Neural Network** to see which approach suits this problem best.

## Dataset

**IoTID20**: network traffic captured from smart home IoT devices, with about 625,000 flows described by features such as packet counts, packet lengths, flow duration and inter-arrival times.

The dataset is not included in this repository. Download it from [Kaggle](https://www.kaggle.com/search?q=IoTID20).

## Approach

1. **Data preprocessing:** handled missing and infinite values and encoded categorical columns and labels.
2. **Outlier removal:** filtered extreme values using the IQR method.
3. **Model training:** trained all three models on an 80/20 train-test split for both tasks.
4. **Evaluation:** compared models using accuracy, precision, recall, F1-score and confusion matrices.

## Tech Stack

Python · pandas · NumPy · scikit-learn · TensorFlow/Keras · Matplotlib · Seaborn

## Author

**Muniba Manaal**: [GitHub](https://github.com/Muniba-Manaal) · [LinkedIn](https://www.linkedin.com/in/muneebamanaal/)
