# Dockerfile-Terraform-AWS
Docker Container with Terraform incl. AWS Provider (Dockerfile)

docker build - < Dockerfile.yaml --tag myubuntu-aws-terraform

docker run -it --rm --name MyUbuntu-dev-Container-aws-terraform -v ~/Documents/Docker/Terraform:/root/terraform/ myubuntu-aws-terraform
