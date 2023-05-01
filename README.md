# Counter-Service Web Applicatiton

## Description 
This repository contain all the necessary resources in order to deploy an application on kuberenetes

## Repo Content 
* A CI/CD GitHub Action pipeline to build and push the application to AWS ECR 
- AWS Secret key and Access key is masked with github variables for obvious security purposes.

* Python web application (counter-service.py) including the requirements.txt

* Dockerfile to build the application and create an image out of it

* Kubernetes manifests
 - both manifests are deployed under tomer-candidate namespace 
 - deployment.yaml  which labels the application and the containers.image to my ECR 
 - service.yaml to create a service of type loadbalancer and expose the application to the world