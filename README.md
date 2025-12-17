# Implementation of a Secure Presentation Attack Detection (PAD) System with Post-Quantum Cryptography (PQC) Integration

## Title of the Project
Implementation of a Secure Presentation Attack Detection (PAD) System with Post-Quantum Cryptography (PQC) Integration

## Small Description
This project integrates a machine learning–based Presentation Attack Detection (PAD) system with modern cryptography, including simulated Post-Quantum Cryptography (PQC), to secure biometric data during the liveness detection inference process and safeguard against future quantum threats.



## About
The **Secure PAD + PQC System** creates a robust and secure pipeline for face liveness detection using a lightweight CNN model.  
AES-GCM is used for encrypting input images, and a simulated Kyber PQC key exchange secures the symmetric AES key.

This ensures end-to-end protection of biometric data during encrypted inference.



## Features
- **Custom PAD Dataset Simulation**  
  Converts CIFAR-10 into a binary Real/Spoof dataset with a 50% spoof ratio.

- **Lightweight CNN (SimplePADCNN)**  
  Efficient structure for real-time PAD inference.

- **PQC-Ready Cryptographic Pipeline**  
  Integrates **AES-256 GCM** for encryption/decryption.

- **Simulated Kyber Key Exchange**  
  Demonstrates PQC-style key exchange protecting the AES key.

- **High Secure Accuracy**  
  Achieves **97.64% accuracy** after secure encrypted pipeline.

- **Low Latency**  
  Maintains **1.80 ms** per image during encrypted inference.



## Requirements
- **OS:** Linux / Windows / macOS / Google Colab  
- **Python:** >= 3.x  
- **Deep Learning:** PyTorch  
- **Crypto Library:** PyCryptodome  
- **Dataset Handling:** torchvision, torch.utils.data  
- **Evaluation:** sklearn  
- **Plotting:** matplotlib  
- **Hardware:** CPU or CUDA-supported GPU



## System Architecture
<img width="450" height="450" alt="image" src="https://github.com/user-attachments/assets/d02e67f1-3cdb-49dc-9067-65d1da757095" />


### Secure Flow
1. AES key is secured with simulated Kyber key exchange.  
2. Image is encrypted using AES-GCM.  
3. Decrypted image is fed to CNN for PAD inference.



## Output

### Output 1 – Secure Pipeline Metrics

| Metric | Result |
|--------|--------|
| Accuracy | **97.64%** |
| Precision | **95.48%** |
| Recall | **99.98%** |
| F1 Score | **97.68%** |
| Average Latency | **1.80 ms** |



## Expected Results and Impact

- **Enhanced Data Privacy**  
  AES-GCM ensures secure encryption of biometric images, preventing data interception.

- **Future-Proof Security**  
  Simulated Kyber integration demonstrates quantum-resistant cryptographic capability.

- **Real-Time Performance**  
  Achieves secure inference with **minimal latency (1.80 ms)** suitable for edge deployment.



## References
1. N. S. Gupta et al., “Enhancing Heart Disease Prediction Accuracy Through Hybrid ML Methods”, EAI Endorsed Trans IoT, 2024.  
2. A. A. Bin Zainuddin, “Enhancing IoT Security…”, Data Science Insights, 2024.  
3. PyTorch Documentation  
4. PyCryptodome Documentation  
5. Kyber PQC Standard Documentation  

