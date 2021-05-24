# Kubernetes - Postgresql deployment

## Story

You're working on your postgreSQL Pod, and when checking the data inside, something is missing. It's all of the data. It turns out that one of the teammates you're working with frequently tests Pod in the cluster, and accidentally managed to delete yours. This is when the idea comes to your head. You should make you Pod persistent so that you lose none of that precious data.

---
## What I have learned during the project

- Work with AWS EKS
- How to create AWS cluster using eksctl
- Create Kubernetes deployment.yaml file with ConfigMap
- What is persistent volume, persistent volume claim and storage classes are in k8s
- How to deploy Postgresql in cluster and use volumes to persist data in it

---
## How to use

### Prerequisites

- AWS account
- AWS CLI
- Kubectl
- Eksctl

1. Use the following link to install AWS CLI: https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html
2. Basics to configure CLI and AWS account: https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html
3. Install kubectl as well: https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/
4. Create a cluster with eksctl: https://docs.aws.amazon.com/eks/latest/userguide/getting-started-eksctl.html
5. Use the following command with yaml files in terminal: ```kubectl apply -f <YAML FILE NAME>```
      - First create storage class, then persistent volume and peristent volume claim. Lastly configMap and deployment.
6. Now you have a running cluster on AWS with Postgresql deployed on it, and a persistent data storage attached to it.

---
## Background materials

- <i class="far fa-book-open"></i> [k8s volumes](https://kubernetes.io/docs/concepts/storage/volumes/)
- <i class="far fa-book-open"></i> [k8s persistent volumes](https://kubernetes.io/docs/concepts/storage/persistent-volumes/)
- <i class="far fa-book-open"></i> [k8s storage classes](https://kubernetes.io/docs/concepts/storage/storage-classes/)
- <i class="far fa-book-open"></i> [k8s StatefulSets](https://kubernetes.io/docs/concepts/workloads/controllers/statefulset/)
- <i class="far fa-video"></i> [k8s volumes explained](https://youtu.be/0swOh5C3OVM)

---
## Contributor
- Nguyen Anh Tuan (Bence)