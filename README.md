# Devops Exercise

## Getting Started:

### Gitlab Setup
To setup your github repository install a local github or use gitlab.com \
Push the code from https://github.com/lucendio/lecture-devops-app to your new repository at gitlab 

- Add Dockerfile and gitlab-ci.yaml to the repository
- Replace dev.env otherwise the MongoDB will not connect
- Configure then the test.yaml and production.yaml configs to pull the correct images.
### Kubernetes Setup
- Install MicroK8s and it's pods with the [Kubernetes Commands](https://github.com/zainlol/devops-exercise/tree/master/Kubernetes%20Setup)
### Local Setup
Add the following entries to your /etc/hosts:\
\
127.0.0.1  todoapp.com\
127.0.0.1  test.todoapp.com\
127.0.0.1  dashboard.todoapp.com

## Application repository: 
https://gitlab.com/devops-exercise/lecture-devops-app 

## Diagram:

![Devops](https://user-images.githubusercontent.com/6658807/87355290-6d546080-c560-11ea-9dc7-ebea0c0d3509.jpg "Diagram for concept")

## Concept:
- three docker container: Gitlab, Application with Node.js and NPM, MongoDB
- version control: Gitlab
- pipeline: Gitlab Ci
- container: Docker
- container orchestrator: MicroK8s
- environments: test, production
- monitoring: Kubernetes Dashboard
- local everything, except VCS and CI/CD via gitlab.com
- complete infrastructure start script/option

## Tech:
- Linux with Manjaro KDE
- Terminal with Fish
- Git with Gitlab 
- Gitlab CI/CD
- Gitlab Registry
- Docker as Image
- Kubernetes with MicroK8s
- Nginx with Ingress

## Ressources:

https://www.danclarke.com/nginx-to-avoid-localhost-port

https://www.youtube.com/playlist?list=PLu-nSsOS6FRIg52MWrd7C_qSnQp3ZoHwW

https://www.udemy.com/course/docker-mastery/

https://www.youtube.com/c/LukeSmithxyz/videos
