# ECE444-F2020-Lab4&5
 Build by Dongfang. this repo is a clone of https://github.com/miguelgrinberg/flasky 

## Activity 1:(1pt) 
Perform all development in a branch "lab4_Microservice_Experiment" in your Lab3 task GitHub repository

## Activity 2: (6pt) 
Show how to build and start the system (including the location of the Docker files and a screenshot of your docker run command, Browser, and your docker image).

### How to build and start the system
Reference page: https://codefresh.io/docker-tutorial/hello-whale-getting-started-docker-flask/


To build: `docker build -t flask-sample:latest .`

To run:  `docker run -d -p 5000:5000 flask-sample`

To check the img: `docker ps -a`

### location of the docker files
The `Dockerfile`and the `requirements.txt` are under the same directory with other files in Lab4
<img src="https://github.com/kmomuphnie/ECE444-F2020-Lab3/blob/lab4_Microservice_Experiment/img/location.png" width="1200">

### Container log
<img src="https://github.com/kmomuphnie/ECE444-F2020-Lab3/blob/lab4_Microservice_Experiment/img/docker_container_log.png" width="1200">

### docker run command & image status

<img src="https://github.com/kmomuphnie/ECE444-F2020-Lab3/blob/lab4_Microservice_Experiment/img/docker_image_status.png" width="1200">

### localhost in browser
<img src="https://github.com/kmomuphnie/ECE444-F2020-Lab3/blob/lab4_Microservice_Experiment/img/localhost.png" width="1200">

## Activity 3 
(3pt) Briefly summarize the differences between Docker and Virtual Machine.


