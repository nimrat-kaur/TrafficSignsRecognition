# Traffic Signs Recognition using CNN & Keras with GUI

## Project
We will build a deep neural network model that can classify traffic signs present in the image into different categories. With this model, we are able to read and understand traffic signs which are a very important task for all autonomous vehicles.

##### What is Traffic Signs Recognition?
There are several different types of traffic signs like speed limits, no entry, traffic signals, turn left or right, children crossing, no passing of heavy vehicles, etc. Traffic signs classification is the process of identifying which class a traffic sign belongs to.

### Dataset
The dataset contains more than 50,000 images of different traffic signs. It is further classified into 43 different classes. The dataset is quite varying, some of the classes have many images while some classes have few images.

Link: https://www.kaggle.com/meowmeowmeowmeowmeow/gtsrb-german-traffic-sign

### GUI
A graphical user interface is built for traffic signs classifier with Tkinter. Tkinter is a GUI toolkit in the standard python library. 

In this file, we have first loaded the trained model using Keras. And then we build the GUI for uploading the image and a button is used to classify which calls the classify() function. The classify() function is converting the image into the dimension of shape (1, 30, 30, 3). This is because to predict the traffic sign we have to provide the same dimension we have used when building the model. Then we predict the class, the "pred" returns us a number between (0-42) which represents the class it belongs to. We use the dictionary to get the information about the class.

## Summary
In this project, we have successfully classified the traffic signs classifier with 94% accuracy and also visualized how our accuracy and loss changes with time, which is pretty good from a simple CNN model.
