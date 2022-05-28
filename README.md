

# FACEATTEND

Attendance system using Face Recognition developed using Django framework and libraries like Dlib, Opencv and face_recognition.
The aim of this project is to build a attendance system which is based on face recognition. Face 
recognition system can be used for attendance marking in 
schools, colleges, offices, etc. This system aims to build a 
attendance system which uses the concept of face recognition as 
existing manual attendance system is time consuming and 
cumbersome to maintain. Here face of 
an individual will be considered for marking attendance. 
It detects the faces of users and attendance will be marked if the detected 
face is found in the database. 



## Introduction

All the user first have to get register along with username and password. Users have to capture photos and it will get stored in dataset. The dataset get trained and the 
faces detected will be compared with images present in the dataset. If match found, attendance will be marked for the respective user. 

* **Create Dataset**  : Images of users are captured using a web cam. Multiple images of single user will be acquired with various gestures and angles.
* **Face Detection** : Dlib's HOG facial detector. Facial Landmark Detection using Dlib's 68 point shape predictor. Classification of Unknown Embedding using a Linear SVM (scikit-learn).
* **Face Recognition** : face_recognition by Adam Geitgey.
* **Attendance Updation** : After face recognition process, the recognized faces will be marked as present and the rest will be marked as absent.

## Installation

* After cloning repository, make a [python virtual environment](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/) using [requirements.txt](https://requirements-txt.readthedocs.io/en/latest/)
* Download [file](https://drive.google.com/uc?export=download&id=1HzO-rnEqgkZ6tLt48yWhYgHk1_zOIYhf) and save in below directory
```
FaceAttend/Face Attendance/face_recognition_data
```
## Documentation

Documentation is available on this [link](https://drive.google.com/drive/folders/1VUP90cYxWo_D2EGDxciO5Dg4uS7H_WFe?usp=sharing)
## About

This project works with 2 types
* Admin 
* User

Admin can perform following functionalities : 
* Login
* Register new user
* Add user photos to the training dataset
* Train the model 
* View attendance of all user


User can perform following functionalities :
* Login
* Mark attendance-in and attendance-out  
* View attendance of itself

