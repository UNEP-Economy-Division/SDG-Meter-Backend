# SDG Meter project - Backend

## Introduction

[The Sustainable Development Goals (SDGs)](http://62.160.8.100/#sdgs) are the guiding line to
achieve a better and more sustainable future for all. They tackle the global challenges we face, including poverty, inequality, climate change, environmental
degradation, peace and justice. The OnePlanet network - an open partnership
for sustainable development - provides a platform where all countries, including
all relevant stakeholders and organizations, are invited to join and actively engage. Thus, the latter submit daily a large number of descriptions of innovative
projects that may be linked to one or more SDGs. For experts, the task of linking all the texts submitted to the SDGs they deal with is very time consuming,
which is why the need to automate this process is very important. In this context,
we propose to solve this problem with a multi-lablel classification of texts using BERT (Bidirectional Encoder Representations from Transformers). We first
present the key steps for building our database, then the multi-label classification
phase using BERT and finally we will present and discuss the obtained results.

## Setup

**You must have python 3.8** for this project not above due to some conflict errors.

In order to develop on the project, you need first to install python dependencies.  
It's recommended to use a python virtual environment, for more details look at [the official documentation](https://docs.python.org/3/tutorial/venv.html).  

You need the binary of the model `app/models/finetuned_models/pytorch_model.bin` which is to heavy to be in this repository.  
Ask someone to get it

To install python dependencies:  
> pip install -r requirements.txt

## Development

To run the project:  
> python app/app.py


## Docker 
You need [Docker](https://www.docker.com/) installed on your machine.

1. Build the image: 
>  docker build --tag sdg-backend .


2. Run the image:
> docker run -p 5000:5000 sdg-backend

The project will be accessible on the port 5000 of your machine: **localhost:5000**

