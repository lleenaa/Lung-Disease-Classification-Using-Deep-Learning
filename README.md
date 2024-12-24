# Lung Disease Detection Using X-Ray Images

This project involves the classification of lung X-ray images into multiple disease categories using deep learning models. The objective is to provide an accurate and efficient method for identifying various lung diseases from X-ray images.

## Project Overview

Lung diseases are critical health issues, and accurate early diagnosis is essential for effective treatment. This project explores state-of-the-art deep learning techniques to classify X-ray images into the following categories:

- Normal
- Inflammatory Pneumonia
- High Density
- Low Density
- Obstructive Diseases
- Infectious Diseases
- Encapsulated Lesions
- Mediastinal Changes
- Thoracic Changes

## Dataset

The dataset consists of X-ray images categorized into nine classes. The data was preprocessed, augmented, and split into training, validation, and test subsets while maintaining class proportions using a stratified splitting approach. 

### Class Distribution
| Class                  | Number of Images |
|------------------------|------------------|
| Normal                | 1340            |
| Inflammatory Pneumonia| 1060            |
| High Density          | 678             |
| Low Density           | 629             |
| Obstructive Diseases  | 644             |
| Infectious Diseases   | 594             |
| Encapsulated Lesions  | 658             |
| Mediastinal Changes   | 596             |
| Thoracic Changes      | 544             |
| **Total**             | **6723**        |

## Models

The project employs three deep learning models:

1. **Basic CNN**: A simple convolutional neural network architecture built from scratch.
2. **Xception**: A pretrained model fine-tuned on the dataset for better performance.
3. **ConvNeXt**: A modern, high-performance model fine-tuned for lung disease classification.

### ConvNeXt on Hugging Face Spaces
Explore the ConvNeXt model using this interactive demo: [ConvNeXt-Image-Classifier](https://huggingface.co/spaces/leenaalsalhi/ConvNeXt-Image-Classifier)

## Results

The models were evaluated on the test set. Here are the key metrics:

| Model       | Test Accuracy | Test Loss |
|-------------|---------------|-----------|
| Basic CNN   | 87.20%        | 0.3792    | 
| Xception    | 88.84%        | 0.4069    | 
| ConvNeXt    | 99.11%        | 0.0294    | 

## Preprocessing

- **Training Data**:
  - Resize: Images resized to 224×224.
  - Augmentation: Random horizontal flip and random rotation (10 degrees).
  - Normalization: Standard ImageNet normalization.
- **Test and Validation Data**:
  - Resize: Images resized to 224×224.
  - Normalization: Standard ImageNet normalization.

## Future Work

- Investigate the use of ensemble methods for better predictions.
- Perform hyperparameter tuning for further optimization.
- Collect and analyze additional datasets to enhance model generalization.



