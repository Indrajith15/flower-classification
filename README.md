# Flower Classification Using MobileNetV2

## Overview

An image classification project that identifies five flower categories using TensorFlow, Keras, and transfer learning with MobileNetV2.

## Flower Categories

- Daisy
- Dandelion
- Roses
- Sunflowers
- Tulips

## Model Architecture

- **Base model:** MobileNetV2 pretrained on ImageNet
- **Transfer learning approach:** Feature extraction with the pretrained base frozen
- **Input size:** 224 × 224 RGB images
- **Pooling:** GlobalAveragePooling2D
- **Output layer:** Dense layer with five units and softmax activation
- **Optimizer:** Adam
- **Loss function:** Sparse categorical cross-entropy
- **Training:** 5 epochs

## Dataset

The project uses TensorFlow's flower photos dataset, containing approximately 3,670 images across five classes.

The data was split into training, validation, and test sets using a stratified split of approximately 70%, 15%, and 15%.

## Results

- **Test accuracy:** 89%
- **Macro F1-score:** 0.88
- **Weighted F1-score:** 0.89

The model was also saved, reloaded, and tested on a new flower image.

## Technologies

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Scikit-learn
- Google Colab

## How to Run

1. Open `flower_classification.ipynb` in Google Colab.
2. Run the notebook cells in order.
3. Allow the dataset and pretrained model weights to download.
4. Train and evaluate the model.
5. Upload a flower image to test a prediction.

## Future Improvements

- Fine-tune selected MobileNetV2 layers.
- Analyze misclassified images.
- Build a simple web interface for image predictions.

## Author

Indrajith Nair
