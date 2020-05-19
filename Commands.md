//install docker
$ sudo apt-get update
$ sudo -y apt-get install apt-transport-https ca-certificates curl software-properties-common
$ curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
$ sudo add-apt-repository \
   "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
   $(lsb_release -cs) \
   stable"
$ sudo -y apt-get install docker-ce docker-ce-cli containerd.io

//run application locally
git clone https://github.com/zainlol/lecture-devops-app.git
cd lecture-devops-app
sudo apt install make
make install-stack
make install-deps
make build
make run-db
make run-local
