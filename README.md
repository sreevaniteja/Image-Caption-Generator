# Image-Caption-Generator
Building Captions for Images using deep learning technique of Convolutional Neural Networks and a type of Recurrent Neural Network LSTM using Python
For Image caption generator model, CNN-RNN model is used.

CNN is used for extracting features from the image. The pre-trained model Xception is used, LSTM will use the information from CNN to help generate a description of the image.
Defining the CNN-RNN model

To define the structure of the model, we will be using the Keras Model from Functional API. It will consist of three major parts:

Feature Extractor – The feature extracted from the image has a size of 2048, with a dense layer, we will reduce the dimensions to 256 nodes.
Sequence Processor – An embedding layer will handle the textual input, followed by the LSTM layer.
Decoder – By merging the output from the above two layers, we will process by the dense layer to make the final prediction. The final layer will contain the number of nodes equal to our vocabulary size.
![image](https://user-images.githubusercontent.com/36618714/137600634-c44c7e51-738d-43a3-b083-482762cf8598.png)

