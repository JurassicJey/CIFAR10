# Fashion MNIST Classification (98.5% accuracy)

This notebook demonstrates building, training, and evaluating a Convolutional Neural Network (CNN) to classify images from the CIFAR10 dataset—a collection of 32x2 grayscale images across 10 object categories (e.g., Cars, birds, trucks).

## Architecture

The CNN model consists of multiple convolutional and fully connected layers as outlined below:

### Convolutional Layers
1. **Conv1**: 3 input channels, 32 output channels, kernel size of 3, padding of 1
   - **ReLU Activation**
2. **Conv2**: 32 input channels, 32 output channels, kernel size of 3, padding of 1
   - **ReLU Activation**
3. **MaxPooling Layer**: kernel size of 2, stride of 2

4. **Conv3**: 32 input channels, 64 output channels, kernel size of 3, padding of 1
   - **ReLU Activation**
5. **Conv4**: 64 input channels, 64 output channels, kernel size of 3, padding of 1
   - **ReLU Activation**
6. **MaxPooling Layer**: kernel size of 2, stride of 2

7. **Conv5**: 64 input channels, 128 output channels, kernel size of 3, padding of 1
   - **ReLU Activation**
8. **Conv6**: 128 input channels, 128 output channels, kernel size of 3, padding of 1
   - **ReLU Activation**
9. **MaxPooling Layer**: kernel size of 2, stride of 2

### Fully Connected Layers
1. **Linear Layer**: 2048 input features, 256 output features
   - **ReLU Activation**
2. **Linear Layer**: 256 input features, 128 output features
   - **ReLU Activation**
3. **Output Layer**: 128 input features, 10 output features (corresponding to the 10 CIFAR-10 classes)

## Usage

1. **Data Preparation**: The notebook loads the CIFAR10 dataset and splits it into training and testing sets.
2. **Model Training**: Defines, compiles, and trains the CNN model on the training data.
3. **Evaluation**: Evaluates model performance on the test set, reporting accuracy and loss.

## Requirements

To run this notebook, ensure you have:
- Python 3.x
- TensorFlow or PyTorch (based on your setup)
- Common libraries like NumPy and Matplotlib

## Customization

This notebook allows for customization:
- Adjust the CNN architecture (e.g., layers, filters, kernel sizes).
- Modify hyperparameters, such as learning rate, batch size, and epochs.
- Experiment with data augmentation techniques to enhance generalization.

---
