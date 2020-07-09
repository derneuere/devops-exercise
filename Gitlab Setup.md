Gitlab Setup

Dependencies:
Install a local github or use gitlab.com

Push code from https://github.com/lucendio/lecture-devops-app to your new repository at gitlab
//add repository of application to gitlab
cd lecture-devops-app
git init
git add .
git config --global credential.helper store
git push --set-upstream https://gitlab.example.com/namespace/nonexistent-project.git master

Add Dockerfile and gitlab-ci.yaml to the repository
Configure then the test.yaml and production.yaml configs to pull the correct images.
