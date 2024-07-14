# Scene-recognition

Overview
Scene recognition is an evolving field in computer vision that has not achieved the same level of success as image recognition due to the vast variability of features in different environments. This project aims to evaluate problem statements using recent literature surveys and propose solutions for these challenges.

We employ ResNet (ResNet18, ResNet50, ResNet152) and VGG (VGG16, VGG19, VGG19 with batch normalization) variants to tackle the proposed problem statement. The entire scene recognition procedure is discussed in this report, with the main goal of laying a foundation for developing a new algorithm. Before the advent of deep learning, scene recognition models relied on low-dimensional representations of scenes. The use of deep learning, especially Convolutional Neural Networks (CNNs), has garnered significant attention in the computer vision community for scene recognition tasks.


Model Architectures
ResNet (Residual Networks)
ResNet, or Residual Networks, introduced by He et al., addresses the vanishing gradient problem by utilizing skip connections, also known as residual connections. These connections allow the model to learn residual functions with reference to the input layer. ResNet variants such as ResNet18, ResNet50, and ResNet152 differ in the number of layers, with deeper networks providing better accuracy but at the cost of increased computational complexity.

VGG (Visual Geometry Group)
VGG networks, developed by the Visual Geometry Group at the University of Oxford, are known for their simplicity and depth. The key characteristic of VGG architectures, such as VGG16 and VGG19, is the use of small 3x3 filters throughout the entire network, which allows for deep networks with up to 19 weight layers. VGG19 with batch normalization further improves performance by normalizing the output of each layer, reducing overfitting, and accelerating the training process.

Dataset
To download intel-image-classification kaggle dataset

1. we need to create an API key in Kaggle for that go to kaggle.com/ and open your user settings page.
2. Then scroll down to the API access section and click generate to download an API key. This will download a file called kaggle.json to your computer. You'll use this file in Colab to access Kaggle datasets and competitions.
3. Navigate to https://colab.research.google.com/. Upload your kaggle.json file using the following snippet in a code cell: ![3](https://github.com/user-attachments/assets/8cb60cb9-d999-4789-b10b-5869aabaa894)

Install the kaggle API using *!pip install -q kaggle
Move the kaggle.json file into ~/.kaggle, which is where the API client expects your token to be located: image
MIT indoor scene dataset:"http://groups.csail.mit.edu/vision/LabelMe/NewImages/indoorCVPR_09.tar"
