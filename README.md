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

The Docker and VM are foundamentally different. 

VM creates guest OS above the host OS on host server, then run application inside of it. Every VM runs in it own virtual OS.

But the Docker creates Docker engine on host server, uses the snapshot of the OS as images, uses the instances of images as containers, then deploys applications inside the containers on top of the Docker engine. But all application process within the containers share the OS of the host.

The VM takes much larger memory(in GB) while the docker images take much much smaller memory(in MB).

The VM takes longer time to initialize(few mins) while the docker images only take from few milliseconds to few seconds.

The docker has much higher resource efficiency. A host server can support thousands of Docker containers while it can only support dozens of VMs.

Th VM has its own OS and does not share OS, with strong isolation(hardware-level) in the host kernel. While the docker containers have shared the host kernel, the VM is much more secure than a docker container. 


