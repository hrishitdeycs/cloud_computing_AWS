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


