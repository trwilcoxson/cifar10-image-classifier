# CIFAR-10 Image Classifier

A convolutional neural network that classifies CIFAR-10 images, built with PyTorch.
The model uses six convolutional layers with batch normalization, dropout, and data
augmentation (random horizontal flips and random crops), and clears a 45% accuracy
baseline while staying compact enough to train on modest hardware.

## Contents

| File | Description |
|------|-------------|
| `cifar10_image_classifier.ipynb` | Data loading, model definition, training loop, and evaluation |
| `cifar10_model.pth` | Trained model weights |

## Running

```bash
pip install torch torchvision numpy matplotlib
jupyter notebook cifar10_image_classifier.ipynb
```

The notebook downloads CIFAR-10 via `torchvision.datasets`, trains the network, and
reports test accuracy. Load `cifar10_model.pth` to skip training and run inference
directly.
