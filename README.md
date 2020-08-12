# Memes-vs-Notes
Images in a student's phone can be categorized as Memes or Notes.

This Repository contains two types of implementation for a Neural Network that can be used to classify images as Notes or Memes.

* [Numpy Implementation](https://github.com/Atharva-K12/Memes-vs-Notes/blob/master/Numpy_Implementation.ipynb)
* [CNN Implementation](https://github.com/Atharva-K12/Memes-vs-Notes/blob/master/CNN_Implementation.ipynb)
---
## Numpy Implementation
The numpy implementation uses a (non-convolutional)neural network.
#### This Implementation is written from scratch by use of Numpy library.
Input Image size is (100x100x3).

DataSet Link: [DataSET_memes_vs_notes(100X100X3)](https://drive.google.com/drive/folders/1TDgDvdbbkGkp3n7IstgHat9TpygnqPoF?usp=sharing)

DataSet Split:

    Train Set = 1400 Images
    Dev Set = 100 Images
    Test Set = 100 Images

Architecture used:

    (FC-Fully Connected Dense Layer)

    FC(100x100x3,730)
    FC(730,250)
    FC(250,95)
    FC(95,33)
    FC(33,1)
Optimizer Used: ADAM

    Learning Rate(alpha)=0.0001
    Beta1=0.9
    Beta2=0.999
    Epsilon=1e-8
Regularisation: L2

    Lambda=0.1
Number of Epochs = 3

Mini Batch Size = 64

#### Train Set Accuracy = 86.57%

#### Dev Set Accuracy = 86%

#### Test Set Accuracy =86%

---
## CNN Implementation
The CNN implementation uses a convolutional neural network.

#### This Implementation uses Pytorch library.

Input Image size is (256x256x3).

DataSet Link: [DataSET_memes_vs_notes(256X256X3)](https://drive.google.com/drive/folders/1nVcnbBLrvy5ZV9_Yv_X3Nl0zmG2kFPcv?usp=sharing)

DataSet Split:

    Train Set = 1400 Images
    Dev Set = 100 Images
    Test Set = 100 Images
Architecture used:

    (FC-Fully Connected Dense Layer,F-Features,S-Strides,C-Channels)
    Conv Layer - F(9x9) S(5x5) C(3,50)
    Max Pool - F(5x5) S(1x1)
    Conv Layer - F(7x7) S(4x4) C(50,70)
    Max Pool - F(3x3) S(1x1)
    Conv Layer - F(3x3) S(1x1) C(70,90)
    Max Pool - F(3x3) S(1x1)
    FC(4*4*90,90)
    FC(90,2)
Optimizer Used: ADAM

    Learning Rate(alpha)=0.0009
Number of Epochs = 4

Mini Batch Size = 100

#### Train Set Accuracy = 99.93%

#### Dev Set Accuracy = 100% 

#### Test Set Accuracy = 100% 

---
### Programming Language :Python
### Notebook Environment Used :[Collaboratory](https://colab.research.google.com/notebooks/intro.ipynb#recent=true)
#### Libraries Installed
* [PIL](https://python-pillow.org/)
* [MATPLOTLIB](https://matplotlib.org/)
* [TORCH](https://pytorch.org/) (only in CNN)
# Contributors
[Atharva Kathale](https://github.com/Atharva-K12)
