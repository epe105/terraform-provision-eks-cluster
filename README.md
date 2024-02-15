# Learn Terraform - Provision an EKS Cluster

This repo is a companion repo to the [Provision an EKS Cluster tutorial](https://developer.hashicorp.com/terraform/tutorials/kubernetes/eks), containing
Terraform configuration files to provision an EKS cluster on AWS.

terraform apply

aws eks --region us-east-1 update-kubeconfig --name=manny-eks-<unique>

# Apply role and role bindings for Service Account

kubectl apply -f role.yaml

kubectl apply -f role-binding.yaml

# Setup Service connection to Azure DevOps

kubectl cluster-info

kubectl get serviceaccounts default -o yaml

kubectl get secret default-token-<unique> -o yaml

# Get External IP of cluster

kubectl get svc

