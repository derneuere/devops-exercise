//install docker <br>
sudo apt-get update <br>
sudo -y apt-get install apt-transport-https ca-certificates curl software-properties-common <br>
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add - <br>
sudo add-apt-repository \ <br>
   "deb [arch=amd64] https://download.docker.com/linux/ubuntu \ <br>
   $(lsb_release -cs) \ <br>
   stable" <br>
sudo -y apt-get install docker-ce docker-ce-cli containerd.io <br>
<br>
//run application locally <br>
git clone https://github.com/zainlol/lecture-devops-app.git <br>
cd lecture-devops-app <br>
sudo apt install make <br>
make install-stack <br>
make install-deps <br>
make build <br>
make run-db <br>
make run-local <br>
<br>
// run Gitlab Docker Image <br>
export GITLAB_HOME=/srv <br>
sudo docker run --detach \ <br>
  --hostname gitlab.example.com \ <br>
  --publish 443:443 --publish 80:80 --publish 22:22 \ <br>
  --name gitlab \ <br>
  --restart always \ <br>
  --volume $GITLAB_HOME/gitlab/config:/etc/gitlab \ <br>
  --volume $GITLAB_HOME/gitlab/logs:/var/log/gitlab \ <br>
  --volume $GITLAB_HOME/gitlab/data:/var/opt/gitlab \ <br>
  gitlab/gitlab-ce:latest <br>