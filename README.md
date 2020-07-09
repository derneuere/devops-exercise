# Devops ExerciseTitle

Getting Started:
- Install MicroK8s with the "Kubernetes Commands" File

Concept:
- three docker container: Gitlab, Application with Node.js and NPM, MongoDB
- version control: Gitlab
- pipeline: Gitlab Ci
- container: Docker
- container orchestrator: MicroK8s
- local everything, except VCS and CI/CD via gitlab.com
- complete infrastructure start script/option

Criteria:

- resource allocation is automated
- resource allocation is reproducible
- component bootstrapping is automated -> Microk8s.yml
- component bootstrapping is reproducible -> Microk8s.yml
- every component exists and is operational
- every component can be reached via HTTPS
- FQDNs are configured for all components, resolve to each of them and serve them properly
- application runs with a replication factor of 2 -> Application runs as ReplicationSet with replicas set to two
- in each environment the applications uses a different instances of its backing service (database)
- CI/CD pipeline functions properly -> finishes without error
- CI/CD pipeline is triggered through VCS commit, or manually, in case of production environment -> triggers everytime a commmit is done
- CI/CD pipeline consists of at least 3 stages -> build, test, deploy stages
- overall setup implements all environments
- concept matches implementation
- implementation meets all formal requirements
- at least one component - aside from the application - was bootstrapped by yourself -> Kubernetes via MicroK8s
- submitted a Pull Request, that adds another meaningful test to the application
- [3] quality and impression, e.g.:
    reasonable documentation
    readable commit messages
    engagement

Tech:
- Linux with Manjaro KDE
- Terminal with Fish
- Git with Gitlab 
- Gitlab CI/CD
- Docker
- Kubernetes with MicroK8s
- Nginx

Ressources:

https://www.danclarke.com/nginx-to-avoid-localhost-port

https://www.youtube.com/playlist?list=PLu-nSsOS6FRIg52MWrd7C_qSnQp3ZoHwW

https://www.udemy.com/course/docker-mastery/

https://www.youtube.com/c/LukeSmithxyz/videos
