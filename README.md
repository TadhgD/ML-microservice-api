# CircleCI Status
[![TadhgD](https://circleci.com/gh/TadhgD/ML-microservice-api.svg?style=svg)](https://app.circleci.com/pipelines/github/TadhgD/ML-microservice-api)

## Project Summary
In this project, a pre-trained sklearn model baked into an application, `app.py`, was deployed to a docker container and then ran as a kubernetes deployment.

While setting up the docker container and kubernetes deployment, supporting infrastructure for the project was built out to support CICD practices. For example, the creation of a Makefile, scripts to build the image and the kubernetes deployment, and CircleCI integration.

## Run instructions

See `Running app.py` below

## Summary of files in repo

This project repo contains a Makefile, a requirements file, a Python flask application, bash scripts to facilitate the building of docker images, uploading them to docker, and the deployment of images to kubernetes, and also a CircleCI config file.

## Project Overview

In this project, you will apply the skills you have acquired in this course to operationalize a Machine Learning Microservice API. 

You are given a pre-trained, `sklearn` model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. You can read more about the data, which was initially taken from Kaggle, on [the data source site](https://www.kaggle.com/c/boston-housing). This project tests your ability to operationalize a Python flask app—in a provided file, `app.py`—that serves out predictions (inference) about housing prices through API calls. This project could be extended to any pre-trained machine learning model, such as those for image recognition and data labeling.

### Project Tasks

Your project goal is to operationalize this working, machine learning microservice using [kubernetes](https://kubernetes.io/), which is an open-source system for automating the management of containerized applications. In this project you will:
* Test your project code using linting
* Complete a Dockerfile to containerize this application
* Deploy your containerized application using Docker and make a prediction
* Improve the log statements in the source code for this application
* Configure Kubernetes and create a Kubernetes cluster
* Deploy a container using Kubernetes and make a prediction
* Upload a complete Github repo with CircleCI to indicate that your code has been tested

You can find a detailed [project rubric, here](https://review.udacity.com/#!/rubrics/2576/view).

**The final implementation of the project will showcase your abilities to operationalize production microservices.**

---

## Setup the Environment

* Create a virtualenv and activate it
* Run `make install` to install the necessary dependencies

### Running `app.py`

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`
3. Run in Kubernetes:  `./run_kubernetes.sh`

### Kubernetes Steps

* Setup and Configure Docker locally
* Setup and Configure Kubernetes locally
* Create Flask app in Container
* Run via kubectl
