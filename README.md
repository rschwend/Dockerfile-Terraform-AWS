# Dockerfile-Terraform-AWS

Let's start with Terraform Learning IaC (Infrastructure as Code). This Dockerfile is deploying a Docker Instance (local) with all dependencies for starting immediately with Terraform Deployments.

Docker Container with Terraform incl. AWS Provider (AWS-CLI)

First, add your keys in the Dockerfile.yaml

ENV AWS_ACCESS_KEY=replace-with-access-key

ENV AWS_SECRET_KEY=replace-with-secret-key

ENV AWS_REGION=replace-with-region

docker build - < Dockerfile.yaml --tag myubuntu-aws-terraform

docker run -it --rm --name MyUbuntu-dev-Container-aws-terraform -v ~/Documents/Docker/Terraform:/root/terraform/ myubuntu-aws-terraform
