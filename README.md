
## Provision EKS cluster with Node group.
* Create cloudformation stack for EKS and Its Node group.
* Create VPC using AWS cloudformation: vpc-2public-2private-subnets.yaml  
* Create an EKS cluster using EKSCTL using this file cluster.YAML 
* Run this setup script  ekssetup.sh after EKS cluster is created.
      
## Build deployment file in yaml for all Docker/ECR Images.
* myweb-deployment.yaml
* myjava-deployment.yaml
   
## Use kubectl to create deployment or apply deployment to run changes.
* kubectl create -f myweb-deployment.yaml
* kubectl create -f myjava-deployment.yaml
* kubectl apply  -f myweb-deployment.yaml ( updates)
* kubectl apply  -f myjava-deployment.yaml ( updates)

## Finally Run K8S Applications.
  
# Git Repo:
* https://github.com/febatech/docker-images-for-k8s-eks-deployments
* https://eksctl.io/usage/creating-and-managing-clusters/
