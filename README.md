# Hand-Gesture-Classification-through-Time-Frequency-Images using EMG signal from Amputees Patients. 🧠

## Overview 🗺️

This repository presents a comprehensive solution for the classification of hand grip postures in amputees using Electromyography (EMG) signals. The methodology is centered around the Short-Time Fourier Transform (STFT) for feature extraction in the time-frequency domain, combined with Convolutional Neural Networks (CNNs) for effective classification through four validations: One to One, All to One, Cross Validation, and Transfer Learning. This approach enables the identification of distinct grip postures, which can be pivotal in rehabilitation and prosthetic control.

<div align="center">
    <img src="https://github.com/user-attachments/assets/4be731dc-3cbb-41be-b495-b4220badeff6" alt="Overview Image" style="max-width: 60%; height: auto;">
</div>

## Key Features 🗝️

- **Short-Time Fourier Transform (STFT)**: 🦾
  - The **Short-Time Fourier Transform** (STFT) is a technique that analyzes non-stationary signals in both time and frequency domains. It divides the signal into short segments, known as **windows**, and applies the Fourier Transform to each segment, generating frequency spectra over time.
  - In the analysis of EMG signals, STFT allows capturing temporal changes in the frequencies associated with different grip postures, providing valuable features for classification using neural networks.
  
  <div align="center">
      <img src="https://github.com/user-attachments/assets/03950ef4-d8f9-4ad7-806d-9cb3a6709a65" alt="STFT Image" style="max-width: 60%; height: auto;">
  </div>

- **Convolutional Neural Networks (CNNs)**: 🤯
- They are a class of deep learning models specifically designed for processing structured grid data, such as images. They consist of multiple layers, including convolutional layers, pooling layers, and fully connected layers, which work together to automatically extract and learn hierarchical features from the input data.
- In the context of EMG signal classification, CNNs can effectively analyze the time-frequency images generated by techniques like the Short-Time Fourier Transform (STFT). By leveraging their ability to capture spatial hierarchies, CNNs enhance the accuracy of classifying different hand grip postures.

  <div align="center">
      <img src="https://github.com/user-attachments/assets/995f81d1-f6f8-45a2-b43b-2b7ce2a44b3a" alt="CNN Architecture" style="max-width: 60%; height: auto;">
  </div>

- **EMG Signal Analysis**: 🫸
  - **Electromyography (EMG)** is a technique used to record and analyze the electrical activity of skeletal muscles. By placing electrodes on the skin surface or inserting them into the muscle, EMG captures the electrical signals generated during muscle contraction and relaxation.
  - EMG signals provide valuable insights into neuromuscular function and are essential for understanding muscle coordination and movement patterns. In the context of hand grip posture classification, analyzing EMG signals allows for the extraction of relevant features that can be used to identify distinct grip patterns, which is crucial for rehabilitation and prosthetic control..

  <div align="center">
      <img src="https://github.com/user-attachments/assets/cc567ee3-def7-4291-995e-6059757207c0" alt="EMG Signal Analysis 1" style="max-width: 60%; height: auto;">
      <img src="https://github.com/user-attachments/assets/bf293d72-4e5d-48ff-9297-d280b3ee1729" alt="EMG Signal Analysis 2" style="max-width: 60%; height: auto;">
  </div>

- ## Validation Methods 🏦
  
    - ### Cross-Validation
    Cross-validation is a statistical method used to estimate the skill of machine learning models. The primary goal is to assess how the results of a statistical analysis will generalize to an independent dataset. In k-fold cross-validation, the dataset is divided into     **k** subsets or folds. The model is trained on **k-1** folds and tested on the remaining fold. This process is repeated **k** times, with each fold used as the test set once. The final performance metric is typically the average of the metrics obtained from each        fold. This technique helps to mitigate overfitting and provides a more reliable estimate of model performance.
  
  <div align="center">
      <img src="https://github.com/user-attachments/assets/a6f5142a-a011-44ea-8d20-6a84221ac394" alt="Experimental Validation 1" style="max-width: 20%; height: auto;">
  </div>

    - ### Transfer Learning 🤺
    Transfer Learning is a machine learning technique where a pre-trained model on one task is reused as the starting point for a model on a second task. This is particularly useful when the second task has a smaller dataset, as the pre-trained model has already learned     useful features from the larger dataset. In the context of CNNs, transfer learning often involves fine-tuning the weights of the pre-trained model on the new dataset. This approach significantly reduces training time and can improve model performance, especially         when data availability is limited.

  <div align="center">
      <img src="https://github.com/user-attachments/assets/813752b2-a6bc-4a42-a033-f1660c08234b" alt="Experimental Validation 1" style="max-width: 20%; height: auto;">
  </div>

    - ### One-to-One Validation 👨‍🏫
    One-to-One validation is a simple evaluation method in which each instance of the dataset is compared to a corresponding instance in the testing dataset. This method is often used in scenarios where the aim is to directly match input and output pairs, such as in         classification tasks. For example, in hand gesture recognition, the model might be tested by comparing the predicted gestures against the actual gestures for each sample. While straightforward, this method may not account for the overall distribution of the dataset     and can be sensitive to outliers.

  <div align="center">
      <img src="https://github.com/user-attachments/assets/86bd5f5e-eb93-4808-a533-06fc7119a0f9" alt="Experimental Validation 1" style="max-width: 20%; height: auto;">
  </div>

- **Data Augmentation Techniques**: 👨‍💻
  - Implements advanced data augmentation strategies to enhance the dataset, promoting robust model training and reducing overfitting.

## Requirements 🕵️

- Python 3.9 or later
- TensorFlow & Keras
- NumPy
- Matplotlib & Seaborn
- Pandas

## Installation 😎

To install the necessary packages, you can use pip:

```bash
pip install -r requirements.txt

