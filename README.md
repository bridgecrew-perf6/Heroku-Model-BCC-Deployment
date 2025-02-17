#Deployed Model 

[MODEL](https://itsrawlinz-jeff.github.io/rawlinzbreastcancerclassificationweb/)

# Breast Cancer Prediction using Federated Learning with PyTorch


Check the Source Code [here](https://github.com/itsrawlinz-jeff/Heroku-Model-BCC-Deployment.git).


## Introduction

In this project we will develop a classifier to predict Breast Cancer from Histopathological images. We will use PyTorch and PySyft for Federated Learning.


### Federated Learning

We will make use of PySyft library. First, we will train a model based on Densenet121, using Federated learning approach. Specifically, we will create two (virtual) workers, `hospital_1` and `hospital_2`, where Histopathological images will be sent for training. Then the results from each worker is combined to build a privacy preserving classifier. Check the [notebook](https://github.com/avinassh/breast-cancer-prediction/blob/master/Detecting_Breast_Cancer_With_Federated_Learning.ipynb) for more details on training.


## Demo

Check the demo [here]( https://breastcancerfinaldeploymentjef.herokuapp.com/) You can use following histopathological images for testing

### Malignant Samples

![malignant_1](https://user-images.githubusercontent.com/640792/63314664-09142700-c326-11e9-90fc-ae358c59b045.jpg)

![malignant_2](https://user-images.githubusercontent.com/640792/63314665-09142700-c326-11e9-9075-607a5d900bd1.jpg)



### Benign Samples

![benign_1](https://user-images.githubusercontent.com/640792/63314649-01ed1900-c326-11e9-8db5-6f6ac8f01f8b.jpg)

![benign_2](https://user-images.githubusercontent.com/640792/63314650-01ed1900-c326-11e9-8a23-1139c38de5e6.jpg)



## Installation and Deployment


### System Requirements


Works with Python 3.5 and above


### Python Requirements
https://pytorch-cancer-prediction.herokuapp.com/
Install them from `requirements.txt`:

    pip install -r requirements.txt


### Local Deployment

Run the server:

    python app.py


Visit `localhost:5000`

