# Setup EKS Cluster

## Prequsite
1. AWS CLI
2. AWS Access key and secret key
3. aws-iam-authenticator
4. Terraform CLI
5. Kubectl

```
cd terraform eks
terraform init
terraform apply
```
# To interact with your cluster, run this command in your terminal:
```
aws eks --region us-east-1 update-kubeconfig --name my-eks-cluster
```


## Deploy Prometheous Stack via helm chart

### Prequsite
1. Kubernetes authentication
2. Helm3 Installed

```
cd helm-charts
helm install prometheous ./kube-prometheus-stack
```
