# CIFAR-10 Image Classification

This project uses a Convolutional Neural Network (CNN) model implemented in PyTorch to classify images from the CIFAR-10 dataset. The model achieves an accuracy of **98.512%** on the test set.

## Model Architecture

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

## Training

The model is trained using the Adam optimizer and CrossEntropyLoss. The data is loaded in batches, and training is done on a GPU for performance.

## Results

The model achieves an accuracy of **98.512%** on the test set, demonstrating high performance in image classification for the CIFAR-10 dataset.
