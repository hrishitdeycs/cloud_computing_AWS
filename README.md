# Cloud and cloud computing
<img width=500px src="https://th.bing.com/th/id/R.bcaed2483788a001e1b8b032ea906f27?rik=vGmsHFueWU7b5w&riu=http%3a%2f%2f4.bp.blogspot.com%2f-VUh4P9IAaIs%2fUzmr30k4AhI%2fAAAAAAAABRo%2f3d-hslTNsIU%2fs1600%2fcloud.jpg&ehk=zbbTp9WSQHp1T%2b%2fUligZZR5IWrLNz72PzN%2b3lZlZU1Y%3d&risl=&pid=ImgRaw&r=0">

### The cloud is a global network of servers, each with a unique function, that are hooked together and meant to operate as a single ecosystem
### Cloud Computing means storing and accessing the data and programs on remote servers that are hosted on the internet instead of the computer’s hard drive or local server. Cloud computing is also referred to as Internet-based computing, it is a technology where the resource is provided as a service through the Internet to the user. The data that is stored can be files, images, documents, or any other storable document.
# Cloud participants
### Cloud computing involves various participants, each playing a crucial role in the ecosystem. Here are the key participants:

## 1. Cloud Service Providers (CSPs):
### Companies that offer cloud computing services.
### Examples: Amazon Web Services (AWS), Microsoft Azure, Google Cloud Platform.

## 2. Cloud Consumers:
### Organizations or individuals who use cloud services.
### Examples: Businesses, educational institutions, government agencies, and individuals.

## 3. End user:
### Use the application deployed in the cloud.
### Do not have any knowledge about the application backend.

# How cloud works
### The back-end is provided by the Cloud Provider - offers services such as storage, compute, database, traffic control mechanisms, and security postures.
### The front-end consists of the client systems which can access the cloud resources from anywhere globally.

# On-premise vs cloud
### Scalability –
### When it comes to scalability we pay more for on-premises set up and get lesser option too and once you scale up it is difficult to scale down and turn into heavy loss like infrastructure and maintenance cost while on the other hand Cloud allows you to pay only how much you use with much easier and faster for scaling upper and down.
### Server Storage –
### On-premises need a lot of space, power, and maintenance to store while on the other hand cloud solution are offered by the provider and maintain the server which saves your money and space.
### Data Security –
### On-premises offers less security and for security, we need physical and traditional IT security measures whereas the cloud offers much better security, and I avoiding all other physical and other security options.
### Data Loss or Recovery –
### If data loss occurs recovery in on-premises is very least while cloud offers you the backup for easier and faster data recovery.
### Maintenance –
### On-premises require an extra team for maintenance which increases the cost while the cloud is maintained by the provider.
# Aws_ec2
## Getiing started with aws
### 1.Create an account on aws
### 2.Sign in to your account 
### 3.Go to your dashboard
### 4.Click on launch instance
### 5.Enter your server name and select ubuntu 
### 6.Click on create new key pair
### 7.Enter your key pair name then select .ppk and click on create new key pair
### 8.In the network settings click on allow http traffic from the internet
### 9.Click on launch instance
### 10.Copy the public ipv4 address from your instance and download putty. 
### 11.Paste the ip address in host name   
### 12.Click on SSH then auth then credentials
### 13.Click browse and open the key pair you downloaded
### 14.Click accept then type ubuntu and then press enter 
### 15.Use the commands
```bash
sudo apt update
```
```bash
sudo apt install apache2 -y
```
### 16.Use the commands 
```bash
cd /var/www/html
```
```bash
sudo rm index.html
```
```bash
sudo vi index.html
```
### 17.Edit the file and press Ctrl+C then type :wq
### 18.On the instance dashboard click on terminate running instance  
# docker_nginx
### 1.Create an account on aws
### 2.Sign in to your account 
### 3.Go to your dashboard
### 4.Click on launch instance
### 5.Enter your server name and select ubuntu 
### 6.Click on create new key pair
### 7.Enter your key pair name then select .ppk and click on create new key pair
### 8.In the network settings click on allow http traffic from the internet
### 9.Click on launch instance
### 10.Copy the public ipv4 address from your instance and download putty. 
### 11.Paste the ip address in host name   
### 12.Click on SSH then auth then credentials
### 13.Click browse and open the key pair you downloaded
### 14.Click accept then type ubuntu and then press enter 
### 15.Install docker using the command
```bash
curl -sL https://github.com/ShubhamTatvamasi/docker-install/raw/master/docker-install.sh | bash
``` 
### 16.Now use the following docker commands
```bash
newgrp docker
```
```bash
docker ps
```
```bash
docker --version
```
### 17.Use the following commands to use ngnix
```bash
docker pull nginx
```
```bash
docker run --name docker-nginx -p 80:80 nginx
```
### 18.Use the following commands 
```bash
ctrl + c
```
```bash
docker ps -a
```
```bash
docker run --name docker-nginx -p 80:80 -d nginx
```
```bash
docker ps
```
```bash
docker stop docker-nginx
```
```bash
docker rm docker-nginx
```
### 19.Use the following html commands
```bash
mkdir -p ~/docker-nginx/html
```
```bash
cd ~/docker-nginx/html
```
```bash
vi index.html
```
```bash
docker run --name docker-nginx -p 80:80 -d -v ~/docker-nginx/html:/usr/share/nginx/html nginx
```
### 20.Visit the website
### 21.On the instance dashboard click on terminate running instance  
# openstack
### 1.Create an account on aws
### 2.Sign in to your account 
### 3.Go to your dashboard
### 4.Click on launch instance
### 5.Enter your server name and select ubuntu(22.04)
### 6.Click on create new key pair
### 7.Enter your key pair name then select .ppk and click on create new key pair
### 8.In the network settings click on allow all traffic from the internet
### 9.Increase storage to 50gb then Click on launch instance
### 10.Copy the public ipv4 address from your instance and download putty. 
### 11.Paste the ip address in host name   
### 12.Click on SSH then auth then credentials
### 13.Click browse and open the key pair you downloaded
### 14.Click accept then type ubuntu and then press enter 
### 15.Use the following command to install openstack
```bash
sudo snap install openstack --channel 2024.1/beta
```
### 16.Use the following commands to create and launch vm on openstack
```bash
sunbeam prepare-node-script
```
```bash
sunbeam prepare-node-script | bash -x && newgrp snap_daemon
```
### 17.This will take around 30 mins
```bash
sunbeam cluster bootstrap --accept-defaults
```
```bash
sunbeam configure --accept-defaults --openrc demo-openrc
```
```bash
sunbeam launch ubuntu --name test
```
![Screenshot (4)](https://github.com/user-attachments/assets/4dd6560c-5cb2-4afc-99ed-0a082801988d)


### 18.On the instance dashboard click on terminate running instance  
# minikube_kubectl
### 1.Create an account on aws
### 2.Sign in to your account 
### 3.Go to your dashboard
### 4.Click on launch instance
### 5.Enter your server name and select ubuntu(22.04) and t3.xlarge
### 6.Click on create new key pair
### 7.Enter your key pair name then select .ppk and click on create new key pair
### 8.In the network settings click on allow all traffic from the internet
### 9.Increase storage to 30gb and click on launch instance
### 10.Copy the public ipv4 address from your instance and download putty. 
### 11.Paste the ip address in host name   
### 12.Click on SSH then auth then credentials
### 13.Click browse and open the key pair you downloaded
### 14.Click accept then type ubuntu and then press enter
### 15.Use the following docker commands
```bash
curl -sL https://github.com/ShubhamTatvamasi/docker-install/raw/master/docker-install.sh | bash
```
```bash
sudo usermod -aG docker $USER
```
```bash
newgrp docker
```
### 16.Use the folowing commands to install kubectl

```bash
sudo snap install kubectl --classic
```
```bash
kubectl version --client
```
### 17.Use the following commands to install minikube
```bash
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
```
```bash
sudo install minikube-linux-amd64 /usr/local/bin/minikube
```
```bash
minikube version
```
### 18.Use the following minikube and kubectl commands
```bash
minikube start --driver=docker
```
```bash
minikube status
```
```bash
kubectl cluster-info
```
```bash
kubectl config view
```
```bash
kubectl get nodes
```
```bash
kubectl get pods
```
```bash
minikube dashboard
```
### 20.Use the following commands to deploy a nginx web server
```bash
kubectl create deployment nginx-web --image=nginx
```
```bash
kubectl expose deployment nginx-web --type NodePort --port=80
```
```bash
kubectl get deployment,pod,svc
```
### 21.Use the following commands to manage minikube addons
```bash
minikube addons list
```
```bash
minikube addons enable dashboard
```
```bash
minikube addons enable ingress
```
```bash
minikube dashboard --url
```
```bash
kubectl proxy --address='0.0.0.0' --disable-filter=true &
```
### 22.Replace server_ip with your public ip
```bash
http://server_ip:8001/api/v1/namespaces/kubernetes-dashboard/services/http:kubernetes-dashboard:/proxy/
```
![Screenshot (2)](https://github.com/user-attachments/assets/e90f73f3-5dac-4231-84cd-258fbe1c2332)

### 23.On the instance dashboard click on terminate running instance  
# virtual_networking
## VPC
### AWS Console -> Services -> Networking & Content Delivery -> VPC -> Your VPCs
### VPC Name: MyVPC
### IPv4 CIDR Block: 10.0.0.0/16
### Click Create
![Screenshot (6)](https://github.com/user-attachments/assets/dc1ec107-f43b-4f8c-8689-269dffd602a8)

### Create subnets :-
### S1-Private Us-east-2a 10.0.1.0/24 Private
### S2-Private Us-east-2b 10.0.2.0/24 Private
### S3-Public Us-east-2a 10.0.3.0/24 Public
### S4-Public Us-east-2b 10.0.4.0/24 Public
![Screenshot (7)](https://github.com/user-attachments/assets/ed2d850f-42f7-4074-afe5-f1ad0714cd52)

### Create Internet gateway 
### Now attach Internet Gateway to VPC
### Create Virtual Private Gateway 
###  Now attach Virtual Private Gateway  to VPC
### Create route tables and attach to subnets
![Screenshot (8)](https://github.com/user-attachments/assets/793c6d62-971c-405e-9283-26f1071dd9db)

## ELB
###  Launch two EC2 instances in different AZs
![Screenshot (9)](https://github.com/user-attachments/assets/3d985a1a-f79f-47d3-a087-28febb549da9)

### Select Application Elastic Load Balancer
### Create 2 instances of same type with select VPC which you created and using putty download apache-2 on both 
### Create Target group  and attach both ec2 instances we created and edit health check-ups 
### Now select this target group and create load balancer 
### Now copy your load balancers dns name and paste it in another tab and refersh twice to see it working
### On any one instance write following commands in putty
```bash
seq 999999999999999999999 > /dev/null &
```
```bash
htop
```
![Screenshot (5)](https://github.com/user-attachments/assets/ee6678f9-b7f4-4606-893b-a338e4717f83)


