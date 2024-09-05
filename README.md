# Prostate MRI Image Segmentation using Deep Learning

This project aims to perform image segmentation on Prostate MRI images using deep learning techniques.

## Models Used

In this project, we assess the effectiveness of three different backbone architectures incorporated into the UNet framework. These architectures are utilized specifically for feature extraction within the encoder section of the UNet model, aiming to enhance prostate MRI segmentation.

### VGG19

VGG19 is a variant of the VGG model which in originality was constituted by 16 convolutional layers. VGG19 has 19 layers that include 16 convolutional layers, 3 Fully connected layers, 5 MaxPool layers, and 1 SoftMax layer. It has a total of 140 million parameters.

### ResNet50:

ResNet50, short for "residual network, is a deep convolutional neural network architecture featuring 50 layers. It incorporates residual connections to enable the learning of deeper architectures without the vanishing gradient problem. The architecture includes convolutional layers for feature extraction, identity blocks for learning residual functions, and convolutional blocks for transformation. Max pooling layers reduce spatial dimensions, and fully connected layers produce final classifications.

### EfficientNetB0

EfficientNet is a convolutional neural network architecture that introduces a systematic method for scaling network dimensions, uniformly adjusting the network's depth, width, and resolution using a compound coefficient.

## Installation

This project requires Python and the following Python libraries installed:

- NumPy
- Matplotlib
- TensorFlow
- Keras
- segmentation_models

If you do not have Python installed yet, you should install the Anaconda distribution of Python, which already includes the above packages and more.

The main code for this project is provided in the Python notebook `S5156692_Prostate_CV_Project_Final.ipynb`. To open and run this notebook, use Jupyter Notebook or use Google Colab.
The other notebook `Prostate_Segmentation_CV_Project_FV.ipynb` is a work in progress for making the code modular and streamlining the hyperparameter tuning process using hyperband.

## Data

The dataset used in this project was obtained from the Multi-site Dataset for Prostate MRI Segmentation, accessible from the link (https://liuquande.github.io/SAML/). This organized dataset comprises T2-weighted Prostate MRI data collected from six diverse data sources, representing different institutions and imaging protocols. To ensure consistency, preprocessing steps were uniformly applied to the data from all six sites, including converting the data to the '.nii' format and resizing all samples to a standardized size of 384x384 in the axial plane.
Site A and Site B
This project focuses on data from two sites, referred to as Site A and Site B. Each site contained data from 30 patients and exhibited distinct characteristics:

## Results

The model's performance is evaluated using metrics such as IoU and F1 Score, and for loss, Total Loss is calculated using Dice Loss and Binary Focal Loss. Among the three models tested, the EfficientNetB0 model outperformed the others on both Site A and Site B. For Site A, the EfficientNetB0 model achieved the highest mean IoU score (0.84557) and mean F1 score (0.91272). Similarly, for Site B, it recorded the highest mean IoU score (0.77517) and mean F1 score (0.85335).

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License. See the LICENSE.md file for details.
