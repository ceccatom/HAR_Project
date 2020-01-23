# Human Activity Recognition Project
The project consists of an Activity Recognition System using a single _Inertial Measurement Unit (IMU)_ to acquire motion related data. The purpose of this project is to develop a flexible framework that can be integrated in portable devices. A [public dataset](https://www.dlr.de/kn/en/desktopdefault.aspx/tabid-8500/14564_read-36508/) was used to train three different deep learning frameworks that aim to achieve high-performing activity classifiers for seven predefined activities:
* Walking
* Running
* Jumping
* Standing
* Sitting
* Falling
* Lying



## Dataset
The dataset was created by _German Aerospace Center (DLR)_ using a single 9-axis IMU placed on the belt of the users. For more details about the dataset visit:
`https://www.dlr.de/kn/en/desktopdefault.aspx/tabid-8500/14564_read-36508/`

## Proposed schemes
Starting from raw data, three different activity recognition schemes are proposed:
1. ___FeaturesConvNet___, computes hand-crafted features and then uses convolutional layers to classify the activities
1. ___AutoConvNet___, converts the raw data into an image-like signal and then uses CNN for the classification
1. ___AutoEncoderNet___, performs an Automatic _Features Extraction (AFE)_ through Convolutional Stacked AutoEncoders and then uses a hybrid classifier composed of LSTM and DNN layers

More information regarding the proposed schemes and their preprocessing are available in the article:
`Automatic Features Extraction for Human Activity Recognition through Deep Learning.pdf`


## Live Classifier Demo
A demo software was built to test the classifiers using live data coming from smartphones. The application is written in Matlab and imports the pre-trained Keras models. [_Matlab Mobile App_](https://www.mathworks.com/products/matlab-mobile.html) is required to be installed in the smartphone.

__The code will be uploaded soon !__
