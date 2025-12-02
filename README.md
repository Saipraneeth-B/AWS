sudo apt update
sudo apt-get install docker.io
sudo apt install git
Sudo apt install nano
git clone https://github.com/Saipraneeth-B/AWS.git
nano Dockerfile
sudo docker build –t mywebapp .
sudo docker run –d –p 80:80 mywebapp
sudo docker ps
sudo docker stop container id
