
![logo](https://raw.githubusercontent.com/Bangkit-Capstone-C22-PS085/kalpataru-waste-classification/master/assets/logo.png)
<h2>An application to waste classification to capstone project Bangkit 2023</h2>
<h1></h1>
<p>Hi. this is our repository for our project in capstone project Bangkit 2023. Our team consist of 6 people from Machine Learning Path, Mobile Development Path and Cloud Computing Path.

All of the project management we take a place with Github repository, to distinguish each path we create a different repository.</p>

## Our Capstone Member
|            Nama             |  Bangkit ID    |       Path         |
|:---------------------------:|:--------------:|:------------------:|
|Bahrul Aji Santoso           |  A063DSX2983   | Mobile Development |
|Hafizul Damar Laya           |  M040DSX0279   | Machine Learning   |
|Ernst Fajar Millennio        |  M181DKX4351   | Machine Learning   |
|Muhamad Wahyudin Nuramanu    |  M004DKX4709   | Machine Learning   |
|Pratama Putra Prayogi        |  C251DSX2189   | Cloud Computing    |


## Simple Description About Our Project
### Machine Learning
In this project we created a machine learning that is used to detect a waste and classify the waste into several classifications including 
- cardboard
- metal
- glass
- plastic
- paper 
Then we also give some decisions for the results by showing the accuracy of the predictions.

### Mobile Development 
In this project, mobile development using Kotlin to develop all in the application. In this project there are one main contributors who are also students from the learning path mobile development. below is a main features of our application:
- Login & Registration User
- Edit Member Address and Integrate With Google Maps SDK
- Image classification trash with camera
- Transaction & History Transaction

### Cloud Computing
Cloud Computing in here as backend services to connect from machine learning model and mobile development with android platform, below is the infrastructure of cloud computing:
- Google Cloud Platform
- ExpressJS
- App Engine
- Cloud Run
- Cloud Storage
- Cloud SQL


## Tech stack
![Machine Learning Infrastructure](https://raw.githubusercontent.com/Bangkit-Capstone-C22-PS085/kalpataru-waste-classification/master/assets/infrastructure.png)
![Mobile Development Infrastructure](https://raw.githubusercontent.com/Bangkit-Capstone-C22-PS085/.github/main/MD.png)
![Cloud Computing Infrastructure](https://raw.githubusercontent.com/Bangkit-Capstone-C22-PS085/.github/main/CC.png)


## Our Import Library on Project
For development you must install several import in your local computer (on Jupyter Notebook) or you can run on Google Colaboratory:
```text
flask==2.1.2
matplotlib==3.4.3
tensorflow==2.8.0
numpy==1.22.3
Pillow==9.0.1
protobuf<=3.20.0
gunicorn==20.1.0
```
For development in Android Studio you need environment in this below:
```
Android
Kotlin Prgramming Language
Android Maps SDK
MVVM Architecture
```

For development in Backend and prepare API consume you need environment in this below:
```
Google Cloud Platform
ExpressJS
App Engine
Cloud Run
Cloud Storage
Cloud SQL
```

For using our project you must clone clone, this below the link:
<br>

```bash
# cloning project Machine Learning
$ git clone https://github.com/Bangkit-Capstone-C22-PS085/kalpataru-waste-classification.git
# cloning project Mobile Development
$ git clone https://github.com/Bangkit-Capstone-C22-PS085/Kalpataru-Mobile.git
# cloning project Cloud Computing
$ git clone https://github.com/Bangkit-Capstone-C22-PS085/backend-cc.git

# build docker image
$ cd kalpataru-waste-classification
$ cd api-services-model
$ docker build -t waste-predict-api .

# run container
$ docker container run  -p {port host}:5000 --name api-model-trashnet
```

after you clone you can use our machine learning project. Then you can use our main machine learning file
`waste_classification.ipynb` our has a several model, you can choose model dependent on your need, you can check on `/api-services-model/model_ml/` `trash-classification.h5` and `trash_exception.h5`.

## Dataset and Additional Dataset
Dataset : [https://github.com/garythung/trashnet](https://github.com/garythung/trashnet)
<br>
Additional dataset Google Drive : [https://drive.google.com/drive/folders/1d0CX9xGEwKoTrGSHxyTOcei2dbr3w3NL?usp=sharing](https://drive.google.com/drive/folders/1d0CX9xGEwKoTrGSHxyTOcei2dbr3w3NL?usp=sharing)