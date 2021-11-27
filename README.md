# LeNet
Jupyter Notebook: Training a CNN for Letter Recognition using EMNIST/letters dataset and the LeNet network architecture with Tensorflow/Keras
In the following application you can draw some letters and do some predictions:
https://christopher-holzweber.com/leNet/
# About LeNet:
The model which is used for prediciton is based on LeNet which was first introduced in 1989 by Yann LeCun et al. It is a convolutional neural netowork structure which was used for applied to handwritten zip code recognition.
During the first lecture on CNNs in one of my courses 'Deep Learning and Neural Nets 1' at my university, I decided to implement the LeNet architecture by myself. In the following image, you can see the network architecture of the implemented CNN:
![leNet](https://user-images.githubusercontent.com/48522299/143719205-3b8da41c-4f5e-4f8f-92d1-4ce79ee23a22.png)
LeCun, Y.; Boser, B.; Denker, J. S.; Henderson, D.; Howard, R. E.; Hubbard, W.; Jackel, L. D. (December 1989). "Backpropagation Applied to Handwritten Zip Code Recognition". Neural Computation
# About the dataset:
EMNIST dataset: https://www.kaggle.com/crawford/emnist
The dataset needed some preprocessing steps (resizing, flipping, normalisation)
# Model Evaluation:
After playing around quite some time with tensorflow convention, struggles with TensorflowJS in an Angular project and some trianing time, I came up with following results:


![loss](https://user-images.githubusercontent.com/48522299/143719218-4fe6f976-6e51-4369-9128-82e186dc2c0d.png)


![acc](https://user-images.githubusercontent.com/48522299/143719219-d9cc646b-bf3e-4e15-8020-38a495bac204.png)


# Model Implementation:
As shown above, the model has the following structure:


![image](https://user-images.githubusercontent.com/48522299/143719379-201e9722-c26b-43e1-92cb-147188ff60c4.png)


The model was trained using Google Colab, where it was possible to upload the csv-files form Kaggle.
In order to run in a Angular application, the model and trained weights needed to be exported using TensorflowJS ( https://www.tensorflow.org/js )
