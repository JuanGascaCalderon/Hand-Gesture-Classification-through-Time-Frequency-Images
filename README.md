# Hand-Gesture-Classification-through-Time-Frequency-Images using EMG signal from Amputees Patients.

## Overview

This repository presents a comprehensive solution for the classification of hand grip postures in amputees using Electromyography (EMG) signals. The methodology is centered around the Short-Time Fourier Transform (STFT) for feature extraction in the time-frequency domain, combined with Convolutional Neural Networks (CNNs) for effective classification throught 4 validations; One to One, All to One, Cross Validation and Transfer Learning . This approach enables the identification of distinct grip postures, which can be pivotal in rehabilitation and prosthetic control.

![image](https://github.com/user-attachments/assets/4be731dc-3cbb-41be-b495-b4220badeff6)


## Key Features

- **Short-Time Fourier Transform (STFT)**: 
  - Utilizes STFT for a detailed time-frequency analysis of EMG signals, allowing for the extraction of meaningful features that capture the dynamics of grip postures.4
    ![image](https://github.com/user-attachments/assets/03950ef4-d8f9-4ad7-806d-9cb3a6709a65)

- **Convolutional Neural Networks (CNNs)**: 
  - Employs advanced CNN architectures for image-based classification, leveraging the spatial hierarchies in the data for improved accuracy.
    ![CNN_3](https://github.com/user-attachments/assets/995f81d1-f6f8-45a2-b43b-2b7ce2a44b3a)

- **EMG Signal Analysis**: 
  - Extracts informative features from EMG signals to create a robust dataset for training and evaluation.
  ![image](https://github.com/user-attachments/assets/cc567ee3-def7-4291-995e-6059757207c0)
  ![image](https://github.com/user-attachments/assets/bf293d72-4e5d-48ff-9297-d280b3ee1729)

- **Experimental Validation**: 
  - Conducts three distinct experiments to validate the classification method, ensuring the reliability and effectiveness of the model.
  ![image](https://github.com/user-attachments/assets/f0a990bc-5cfb-4536-90a0-5c51657ad3e7)
  ![image](https://github.com/user-attachments/assets/3cdab35d-2731-4486-8934-4117fc3046d2)

- **Data Augmentation Techniques**: 
  - Implements advanced data augmentation strategies to enhance the dataset, promoting robust model training and reducing overfitting.

## Requirements

- Python 3.9 or later
- TensorFlow & Keras
- NumPy
- Matplotlib & Seaborn
- Pandas

## Installation

To install the necessary packages, you can use pip:

```bash
pip install -r requirements.txt
