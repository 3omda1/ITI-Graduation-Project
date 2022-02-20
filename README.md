# ITI-Graduation-Project
## Our graduation project for ITI journey at devops track :relaxed:

# DevOps and cloud provider used:
## 1. Docker Platform
## 2. Kubernetes
## 3. Terraform 
## 4. Ansible
## 5. Jenkins
## 6. Google CLoud Platform (GCP)

## What we have done 
1. Built a simple web page 
2. Dockorized it 
3. Created our infrastructure using Terraform
4. Deployed Jenkins  deployment and services  using Ansible
5. Created jenkins pipeline to do:
   - Build our Dockerfile and push it to dockerhub repository
   - Deploy our image with kubernetes YAML file to the cluster

## Infrastructure with Terraform
1. VPC with public and private subnets with their configurations
2. Firewall rule with IAP for security purposes
3. Private VM (with pre-configured installations) to access our private cluster
4. Private GKE cluster 
-To use our infrastructure: Navigate to terraform folder and then run the following commands:
```
terraform init
terraform plan
terraform apply
```
## Kubernetes objects
1. Deployment object to deploy our custom image
2. External service object (LoadBalancer) to access our deployment
-To use our objects: Navigate to kubernets folder and then run the following command:
```
kubectl apply -f docker-deployment-with-service.yaml
```


## Configurations with Ansible
1. Create K8S namespace for our objects
2. Create our jenkins deployments and services using definition module
-To use our ansible configurations: Navigate to ansible folder and then run the following command:
```
ansible-playbook provision-k8s.yaml
```
## CI/CD with Jenkins
1. Configure our jenkins agent as jenkins node and install Docker Pipeline plugin to be able to build and push
2. Added my dockerhub credentials
3. Pipeline to do the following:
   - CI stages to build our image and pushes it to dockerhub
   - CD stages to deploy our deployment and external service YAML file

## Finaly
At the end of this great journey
We would like to thank each and every one of skilled and experienced instructors who helped us greatly and supported us whether by lectures or with valuable advices  :blue_heart: :blue_heart:

## Contributors:
![Image](pics/ahmed.jpg)|![Image](pics/dalia.jpg)|
|:-----------:|:-----------:|
|[Ahmed Emad](https://www.linkedin.com/in/ahmed-emad1/)|[Dalia Badr](https://www.linkedin.com/in/DaliaBadr-db7/)|



