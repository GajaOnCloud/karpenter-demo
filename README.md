# **Work in progress**
# Karpenter Demo Repository 

This repository provides a hands-on demonstration of **AWS Karpenter**, a Kubernetes node autoscaler that provisions and scales nodes efficiently for dynamic workloads. The demo is tailored for AWS Elastic Kubernetes Service (EKS) and showcases Karpenter's powerful features.

---

## 🚀 Features

- Dynamic scaling of Kubernetes nodes based on workload demands.
- Intelligent provisioning with EC2 instance flexibility (Spot and On-Demand).
- Cost-optimized autoscaling with rapid node provisioning.
- Advanced scheduling and bin packing for resource efficiency.

---

## 🛠️ Setup and Configuration

### Prerequisites

1. **AWS Account** with IAM permissions to manage EC2, EKS, and related services.
2. **Kubernetes cluster** running on AWS EKS.
3. **eksdemo** installed locally.
5. **AWS CLI** configured with access credentials.

### Wky eksdemo?

While creating an EKS cluster is fairly easy thanks to eksctl, manually installing and configuring applications on EKS is complex, time consuming and error-prone. One of the most powerful feature of eksdemo is its extensive application catalog. An application can be installed (including dependencies) with a single command.

For example, the command: eksdemo install karpenter -c <cluster-name> will:

- Create the EC2 Spot Service Linked Role (if it doesn't already exist)
- Create the Karpenter Controller IAM Role (IRSA)
- Create the Karpenter Node IAM Role
- Create an SQS Queue and EventBridge rules for native Spot Termination Handling
- Add an entry to the aws-auth ConfigMap for the Karpenter Node IAM Role
- Install the Karpenter Helm Chart
- Create default Karpenter NodePool and EC2NodeClass Custom Resources
- URL https://github.com/awslabs/eksdemo
---


### Step-by-Step Guide
<TBD>

### Documentation
For detailed documentation, visit the official Karpenter website - https://karpenter.sh/.

### Disclaimer
This repository is intended for demonstration purposes only. Use it as a reference and adapt configurations to your production needs.
