# Implement-CNNs-with-CIFAR-10
Implement CNNs with CIFAR 10. Training and Evaluating on CIFAR 10. Tuning hyper-parameters: batch size, optimizer, learning rate, ...
## Project Overview
This project implements a Convolutional Neural Network (CNN) to classify images from the CIFAR-10 dataset. The project includes hyperparameter tuning to find the best combination of batch size, learning rate, and optimizer for optimal performance.

## Dataset
Dataset: CIFAR-10 (60,000 images in 10 classes).
Training Set: 50,000 images.
Test Set: 10,000 images.

## Model Training Details
Loss Function: CrossEntropyLoss.
Optimizers: Adam, SGD.
Batch Sizes: 32, 64.
Learning Rates: 0.001, 0.0005.
Epochs per Run: 5 (for tuning).
### Hyperparameter Tuning Results

| **Batch Size** | **Learning Rate** | **Optimizer** | **Epoch 1 Loss** | **Epoch 5 Loss** | **Test Accuracy** |  
|----------------|-------------------|---------------|------------------|------------------|-------------------|  
| 32             | 0.001             | Adam          | 1.2567           | 0.3660           | 72.64%            |  
| 32             | 0.001             | SGD           | 1.9240           | 1.0561           | 62.32%            |  
| 32             | 0.0005            | Adam          | 1.3081           | 0.4568           | 72.95%            |  
| 32             | 0.0005            | SGD           | 2.0279           | 1.2572           | 55.60%            |  
| 64             | 0.001             | Adam          | 1.2627           | 0.3640           | 74.28%            |  
| 64             | 0.001             | SGD           | 2.0638           | 1.2478           | 55.75%            |  
| 64             | 0.0005            | Adam          | 1.3787           | 0.6034           | 72.30%            |  
| 64             | 0.0005            | SGD           | 2.1957           | 1.4631           | 48.88%            |  

---

### Best Hyperparameters:
- **Batch Size**: 64
- **Learning Rate**: 0.001
- **Optimizer**: Adam
- **Test Accuracy**: 74.28%

### Images with Predictions
![test image](https://github.com/user-attachments/assets/8097d45e-def7-4633-bf97-7a4f7ca50987)
