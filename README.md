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


minikube start --driver=docker
minikube status
minikube kubectl -- get pods -A
minikube dashboard
minikube version
kubectl version --client

minikube start

kubectl create deployment mynginx --image=nginx
kubectl get deployments
kubectl get pods
kubectl describe pods

kubectl expose deployment mynginx --type=NodePort --port=80 --target-port=80

kubectl scale deployment mynginx --replicas=4
kubectl get service mynginx

kubectl port-forward svc/mynginx 8081:80

minikube tunnel
minikube service mynginx --url

kubectl delete deployment mynginx
kubectl delete service mynginx
minikube stop
minikube delete

ngios:
docker pull jasonrivers/nagios:latest
docker run --name nagiosdemo -p 8888:80 jasonrivers/nagios:latest
open in browser   http://localhost:8888
	Username: nagiosadmin
	Password: nagios

docker stop nagiosdemo
docker rm nagiosdemo
docker images
docker rmi jasonrivers/nagios:latest
