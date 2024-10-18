
# Tom and Jerry Image Classification

This project classifies images into **Tom**, **Jerry**, **Both**, or **Neither** using a DenseNet121-based CNN model.

## Dataset

- **Classes**: Jerry (0), Tom (1), None (2), Both (3)
- **Split**: 80% training, 20% validation.

## Model

- **Base**: DenseNet121 (pre-trained on ImageNet)
- **Custom Layers**: MaxPooling2D, Dropout (0.5), Flatten, Dense (4 units, softmax)
- **Loss**: Sparse Categorical Crossentropy
- **Optimizer**: Adam (learning rate = 1e-4)
- **Early Stopping**: Monitors validation loss with patience = 3 epochs.

## Results

- Plots for accuracy and loss during training are displayed at the end of training.
- Model evaluates on both training and validation sets.
