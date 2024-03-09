# Prostate MRI Image Segmentation using Deep Learning

This project aims to perform image segmentation on Prostate MRI images using deep learning techniques. The goal is to segment the prostate structure in the MRI images.

## Models Used

### VGG19

VGG19 is a variant of VGG model which in originality was constituted by 16 convolutional layers. VGG19 has 19 layers that includes 16 convolutional layers, 3 Fully connected layer, 5 MaxPool layers and 1 SoftMax layer. It has a total of 140 million parameters.

In this project, we use a U-Net architecture with a VGG19 backbone for the segmentation task. The U-Net model is a type of convolutional neural network that is widely used for biomedical image segmentation. The U-Net architecture is symmetric, with a contracting path to capture context and an expansive path that allows precise localization.

## Installation

This project requires Python and the following Python libraries installed:

- NumPy
- Matplotlib
- TensorFlow
- Keras
- segmentation_models

You will also need to have software installed to run and execute a Jupyter Notebook.

If you do not have Python installed yet, it is highly recommended that you install the Anaconda distribution of Python, which already has the above packages and more included.

## Usage

The main code for this project is provided in the notebook `S5156692_Prostate_CV_Project_Final.ipynb`. To open and run this notebook, you will need Jupyter Notebook installed with a Python kernel.

## Data

The data used in this project consists of Prostate MRI images. Each image is accompanied by a corresponding segmentation mask, which indicates the location of the prostate in the image.

## Results

The performance of the model is evaluated using various metrics, including Dice Coefficient, Jaccard Index, Sensitivity, Specificity, and Accuracy.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License. See the LICENSE.md file for details.