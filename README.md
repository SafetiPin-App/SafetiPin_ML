<img src="https://safetipin.com/wp-content/uploads/2020/01/SafetiPin-Logo-1.png" alt="SafetiPin Logo" width="250" height="100" align="top">  &nbsp; &nbsp;&nbsp;&nbsp; &nbsp; &nbsp;&nbsp;&nbsp; &nbsp; &nbsp;&nbsp;&nbsp;  <img src="https://www.un.org/ruleoflaw/wp-content/uploads/2015/04/uniceflogo.png" alt="Unicef Logo" width="200" height="200">

###  Introduction to Safetipin

Safetipin is a technology platform that works to make our communities and cities safer by collecting and disseminating safety-related information through map-based application by users and trained auditors. We collect and assess information on perceptions of safety in urban public spaces by assessing them on parameters of physical infrastructure and the social environment. Using the methodology of a safety audit, the following parameters are measured - Lighting, openness, visibility, security, walkpath, availability of public transport, presence of people and diversity of women or children in people. Based on the audit ratings, a Safety Score is generated for an area/ city.

While crowdsourced data is valuable, we realised that it needed to be supplemented by a large-scale dataset that covers a city in a uniform manner. To allow for large-scale data collection, we built Safetipin Nite App. This is used to capture images of the city through cars that drive around the city. Images once uploaded on the Safetipin server are then analysed on above listed parameters by a trained team at Safetipin. However, it is a time-consuming process as the analysts have to evaluate each picture and rate them on the audit parameters. 

**About this Project:**
As part of Global Innovation Fund, UNICEF supported a project where Safetipin has built a Machine Learning model that would automatically extract key feature points from a picture. These features could then be used to rate a location on safety audit parameters. The aim of this project is to use state of the art AI/ML technology to capture following keypoints /features from night-time pics. 
- Pedestrians
- Streetlights
- Roof Lights
- Pavement
- Vehicles
- Vehicle Front Glare
- Bike Drivers
- Banners

All the above features are important in our analysis and further evaluating its key Parameters.

###### About this Repository

This is an implementation of Faster RCNN on Python 3, Keras, and TensorFlow. The model generates bounding boxes around key features model for which it has been trained. With this repository we have released the final model which can be directly used.
The model has been trained using a pretrained base Vgg16 model. The Vgg16 model has been specifically designed using night-time dataset and can be downloaded from here. This could be useful for open-source community. The final model for features detection will be released soon on completion of project.

###### The repository includes:
- Source Code for Training Faster RCNN model using Keras and TensorFlow
- Parser for VOC dataset
- Jupyter Notebook for evaluating the results and analysing attention maps on Vgg model
- Source code for prediction
- Additional/Pre-processing Script

###### Requirement
- Python 3.7 or above
- TensorFlow 2.0 or above
- Keras 2.2.0 or above

###### How to use the Repository:

The training is done on a dataset prepared in voc format. For COCO dataset, there is a script which converts coco dataset format into voc dataset format.
Download the base vgg model from link here and put it into folder model.
The training can be initiated by running python train.py -p /path/to/vocdataset.
The configuration for Faster RCNN is saved in lib/config.py. The settings are as per our requirement and can be changed as per dataset.
For people interested in using our model, please download the file from the link here and save it in model folder.
The inference can be done either using jupyter notebook present in the repository or by running following files python train.py

Example Output:



![alt text](https://github.com/SafetiPin-App/SafetiPin_ML/blob/add-license-1/images/1227_1226.jpg?raw=true)

![alt text](https://github.com/Aavesh/SafetiPin_ML/blob/master/images/18.jpg?raw=true)
