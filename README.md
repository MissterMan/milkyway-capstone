
![logo](https://github.com/MissterMan/milkyway-capstone/blob/main/assets/logo.png)

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
#### Machine Learning
Generating dummy data, building a recommendation system with content-based filtering using the TensorFlow library and Flask as the framework, and then performing preprocessing with feature scaling

#### Mobile Development
Deployment a mobile application with kotlin and android studio IDE that uses a RESTful API to get and post data and firebase auth to login and register. The application UI created in Figma. The application integrated into a cloud-based system and created a seamless and intuitive user experience, it will be implemented based on user flows.

#### Cloud Computing
Provisioning IT Infrastructure in Google Cloud Platform using Compute Engine, doing RESTful API research, developing RESTful API service,  and doing the testing. Deploying the service as a container in the Compute Engine using docker.

## Features
In this project there is one main contributors who are also students from the learning path mobile development.
- Login & Registration User
- Breast Milk Request Using Match Making
- Breast Milk Donation
- Baby Care Information

## How to use our project

#### Clone this repo
```https://github.com/MissterMan/milkyway-capstone.git```

#### Mobile Development

* Clone this repo.

  ```
  git clone https://github.com/bahrulajisantoso/MilkyWay.git
  ```
* Open in Android Studio
* Connect your device into Android Studio.

  ```
  https://developer.android.com/codelabs/basic-android-kotlin-compose-connect-device?hl=id#0
  ```
* Run in your Android Studio.

  ```
  https://developer.android.com/training/basics/firstapp/running-app?hl=id
  ```

#### Machine Learning Model
``` bash
# cloning main repo
$ git clone https://github.com/MissterMan/milkyway-capstone.git

# change directory
$ cd milkyway-model

#build docker image
$ docker build -t milkyway-model .

# run container
$ docker container run -p {host port}:5000 -d --name milkyway-model
```

#### Backend API CC
``` bash
# creating docker network
$ docker network create -d milkyway-network

# creating mariadb container
$ docker run --name mariadb -e MYSQL_ROOT_PASSWORD=mypass -p 3306:3306 -d docker.io/library/mariadb:10.3

# setup database
# copy database
$ docker cp db_donor.sql container_id:/donor.sql

# create database
$ docker exec -ti mariadb bash
$ mysql -u root -p
$ CREATE DATABASE db_donor;
$ exit
# import database
$ mysql -u root -p db_donor < db_donor.sql

# connect MariaDB container to the network
docker network connect milkyway-network mariadb

# cloning main repo
$ git clone https://github.com/MissterMan/milkyway-capstone.git

# change directory
$ cd milkyway-api

#build docker image
$ docker build -t milkyway-model .

# run container
$ docker container run -p {host port}:5000 -d --name milkyway-model

# connect milkyway-api-service container to the network
docker network connect milkyway-network milkyway-api-service
```

### API Documentation
https://app.swaggerhub.com/apis-docs/PUTRAYOGI4545/milkyway-api/1.0#/default/get_api_donors

### Datasets Link
https://drive.google.com/drive/folders/13bh8brNmRumwPvgVHOTbJnTJCtxU6waZ?usp=sharing
