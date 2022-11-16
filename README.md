## Create ECR and ECS and deploy image from ECR to ECS using Terraform 

Using this template, you can create an AWS ECR and ECS and deploy a dockerized image (centos image for example) in it. Firstly, you need to pull the centos image from Docker Hub, and then you can push it to AWS ECR, Elastic Container Registry. Afterward using Terraform you can launch the Docker image in an AWS ECS cluster with AWS Fargate.

### Prerequisites:

- AWS account
- IDE of your choice
- AWS configured
- Terraform installed
- Docker installed

### Steps to follow

- cd into ecr folder
- run `terraform init` this will create a lock file
- run `terraform fmt`
- run `terraform plan`
- run `terraform apply`
This will pull the centos image from docker hub and will create an ECR. You can open our AWS console and navigate to Elastic Container Registry.
You can push that image on your ECR

Now go back to main directory and `cd to ecs` replace access-key and secret-key with your own keys , you can create .tfvars file for better sercurity and then run following command.

- run `terraform fmt`
- run `terraform validate`
- run `terraform plan`
- run `terraform apply`










