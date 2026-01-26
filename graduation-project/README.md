## 🧠 Robust and Privacy-Aware EEG Signal Classification for BCI

This project presents a robust and privacy-preserving EEG classification framework for Brain–Computer Interfaces (BCIs), focusing on motor imagery (MI) decoding under adversarial and privacy threats.

EEG-based BCIs are highly sensitive to noise, subject variability, and adversarial perturbations, while also containing private mental information that must be protected. This project addresses both challenges in a unified pipeline.

## 🔍 Problem Addressed

EEG signals are non-stationary and vary significantly across subjects and sessions

Deep learning models for BCIs are vulnerable to adversarial attacks

Brain signals can leak sensitive mental information if not protected properly

## 💡 Proposed Solution

An end-to-end EEG classification pipeline that integrates:

Euclidean Alignment (EA) to reduce inter-subject/session variability

Alignment-Based Adversarial Training (ABAT) using FGSM and PGD attacks to improve robustness

Differential Privacy (DP-SGD) to protect sensitive EEG data during training

EEGNet as a lightweight and efficient deep learning classifier

The model classifies EEG signals into four motor imagery classes:
Left Hand, Right Hand, Feet, and Tongue.

## 🧪 Dataset

BCI Competition IV-2a

9 subjects, 22 EEG channels

4 motor imagery classes

Standard preprocessing, epoching, and filtering applied

=> http://bnci-horizon-2020.eu/database/data-sets


## 🏗️ System Pipeline

The proposed system consists of two main phases: training and classification.

### 🔹 Training Phase

<img src="diagrams/Training Phase.png" width="800">

**Figure:** Training phase illustrating EEG preprocessing, Euclidean Alignment,
adversarial training (EABAT), and differential privacy enforcement.

### 🔹 Classification Phase

<img src="diagrams/Classification Phase.png" width="800">


**Figure:** Classification phase showing robust inference on aligned EEG data
without privacy noise injection.


### 👤 Use Case Diagram


<img src="diagrams/Use case.png" width="700">


**Figure:** Use case diagram illustrating interactions between users and the
EEG classification system.
.

### 🔁 Sequence Diagrams

### 👤 Admin Training Sequence

<img src="diagrams/Admin Training Sequence.png" width="800">

**Figure:** Sequence of operations during the training phase managed by the administrator.



#### User – Classification Sequence

<<img src="diagrams/user_classification_sequence.png" width="800">

**Figure:** Sequence of operations during real-time EEG classification.

## 🎯 Key Contributions

Improves classification robustness against adversarial attacks

Preserves mental privacy using formal differential privacy guarantees

Combines alignment + adversarial training, avoiding accuracy degradation

Designed as a secure BCI-ready ML pipeline

## ⚠️ Limitations

Supports four MI classes only

Increased training cost due to adversarial learning

Relies on public EEG datasets

## 🛠️ Technologies & Tools

Python, PyTorch

EEGNet

FGSM & PGD adversarial attacks

Differential Privacy (DP-SGD)
