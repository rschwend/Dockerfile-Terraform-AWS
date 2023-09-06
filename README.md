# Dockerfile-Terraform-AWS
Docker Container with Terraform incl. AWS Provider (Dockerfile)

First, add your keys in the Dockerfile.yaml

ENV AWS_ACCESS_KEY=
ENV AWS_SECRET_KEY=

docker build - < Dockerfile.yaml --tag myubuntu-aws-terraform

docker run -it --rm --name MyUbuntu-dev-Container-aws-terraform -v ~/Documents/Docker/Terraform:/root/terraform/ myubuntu-aws-terraform
