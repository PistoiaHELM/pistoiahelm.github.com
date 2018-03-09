## Objective - 'helm' Image
Leveraging the docker container technology, it is intended to create a docker image 'helm' that anyone can use to evaluate HELM Web Editor.In addition to the HELM Web Editor, HELM2 Web Service and HELM Monomer/Rule Service are bundled in the image, so are Tomcat 8 and Java 8. This provides a one-stop-shopping for all HELM web components.

## Pre-requisite to use the Dockerfile to build and run the image
- Linux or Mac OS X
- Docker run time installed on the OS

## How to Build Docker Image
After cloning the project to your machine, navigate to the folder 'docker' which contains this file, then run the following command:

    docker build -t helm .

This will generate a docker image with the name 'helm' and tag 'latest' in your local docker image repository.  
Use the following command to verify:

    docker image ls

## How to Run the Docker Image
Execute the following command to run the docker image 'helm' locally:

    docker run -d -p 8080:8080 helm

Use the following command to verify a docker container is running based on this image:

    docker container ls

## How to Use HELM Web Editor

Open the following URL in your favorite web browser:

  http://localhost:8080/hwe/examples/App.htm

## Explore HELM Monomer Service Swagger Page

Open the following URL in your favorite web browser:

  http://localhost:8080/HELM2MonomerService/
  
## Explore HELM Web Service Swagger Page

Open the following URL in your favorite web browser:

  http://localhost:8080/WebService/HowToUse.html
