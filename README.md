[![CircleCI](https://dl.circleci.com/status-badge/img/gh/MillicentMal/DevOps_Microservices/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/MillicentMal/DevOps_Microservices/tree/master)

## Project Overview
This project shows the ability to incorporate DevOps Engineering with Machine Learning.This can be seen as a dataOps project. 

Given a pre-trained, `sklearn` model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. You can read more about the data, which was initially taken from Kaggle, on [the data source site](https://www.kaggle.com/c/boston-housing). This project tests your ability to operationalize a Python flask app—in a provided file, `app.py`—that serves out predictions (inference) about housing prices through API calls. This project could be extended to any pre-trained machine learning model, such as those for image recognition and data labeling.


## Setup the Environment

* Create a virtualenv with Python 3.7 and activate it. Refer to this link for help on specifying the Python version in the virtualenv. 
```bash
python3 -m pip install --user virtualenv
# You should have Python 3.7 available in your host. 
# Check the Python path using `which python3`
# Use a command similar to this one:
python3 -m virtualenv --python=<path-to-Python3.7> .devops
source .devops/bin/activate
```
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
* 
## Files
1. "app.py" - Contains the main application written in python which can be run as a standalone using "python app.py"
2. "run_docker.sh" - builds the docker image,and runs the app in docker
3. "run_kubernetes.sh" - runs the app in kubernetes
4. "upload_docker.sh" - contains instructions to upload the docker image to a repository on docker
5. "requirements.txt" - contains all the required dependencies for app.py to run

