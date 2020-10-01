# SafetiPin_ML
This is Machine Learning work done by SafetiPin for features extraction from night time images

The Project is with regards to work done by SafetiPin for a project involving Artificial Intelligence/MachineLearning in coordination  with UNICEF. The aim of this project is to use state of the art AI/ML technology to capture following keypoints/features from night time pics.The main features to be extracted  are
* Pedestrian.
* Street Lights
* Roof Lights
* Pavements
* Vehicles
* Vehicle Front Glare
* Bike Driver
* Banners

All above features are very important in SafetiPin Analysis for further evaluating its key Parameters.

## What is SafetiPin:

Safetipin is a social organisation working with a wide range of urban stakeholders including governments to make public spaces safer and more inclusive for women. We collect data using our 3 mobile phone applications (My Safetipin, which is available on the app store and play store; Safetipin Nite and Safetipin Site) and present this to relevant stakeholders with recommendations. We also generate a safety score based on the data we collect and provide it in the My Safetipin app for users to make safe and informed decisions about their mobility.

## About this Repository :

This is an implementation of Faster RCNN on Python 3, Keras, and TensorFlow. The model generates bounding boxes around key features model has been trained for. With this repository we have released the final model which can directly be used.

The model has been trained using a pretrained base VGG16 model. The VGG16 model has been specifically designed using night time dataset and can be downloaded from here.

### The repository includes:
* Source Code for Training Faster RCNN model using Keras & TensorFlow
* Parser for VOC dataset
* Jupyter Notebook for evaluating the results
* Source code for prediction
* Additional/Preprocessing Script

 ## Requirement
* Python 3.7 or above
* TensorFlow 2.0 or above
* Keras 2.2.0 or above
 
 ## How to use the Repository:
* The training is done on a dataset prepared in voc format. For COCO dataset ,there  is a script which converts coco dataset format into voc dataset format.
* Download the base vgg model from link here and put it into folder model
* The training can be initiated by running python  train.py -p /path/to/vocdataset
* The configuration for Faster RCNN  are saved in lib/config.py. The settings are as per our requirement and  can be changed as per dataset.
* For people interested in using our model , please download the file from the link here and save it in model folder.
* The inference can be done either using jupyter notebook present in the repository or by running following files python train.py 

### Example Output

![alt text](https://github.com/Aavesh/SafetiPin_ML/blob/master/images/1227_1226.jpg?raw=true)

![alt text](https://github.com/Aavesh/SafetiPin_ML/blob/master/images/47.jpg?raw=true)

![alt text](https://github.com/Aavesh/SafetiPin_ML/blob/master/images/18.jpg?raw=true)
