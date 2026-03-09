# Infrastructure-as-Code-IaaC-on-AWS-with-Terraform

### ****Project Overview****

This project demonstrates how to deploy a fully functional cloud infrastructure environment on Amazon Web Services (AWS) using Infrastructure as Code (IaC) with Terraform. Instead of manually configuring resources through the AWS console, this project automates the entire infrastructure deployment process. The infrastructure includes a custom Virtual Private Cloud (VPC), networking components, security configuration, and multiple EC2 instances.

The primary goal of this project is to showcase practical skills in:

* Cloud infrastructure architecture

* Infrastructure automation

* AWS networking concepts

* Terraform-based provisioning

* Reproducible and scalable cloud environments

This project simulates a small-scale infrastructure environment that could later be used for workloads such as container orchestration platforms, development environments, or distributed systems.

###  **Architecture Overview**

The infrastructure deployed in this project consists of the following components:

 * Custom Virtual Private Cloud (VPC)

 * Public Subnet

 * Internet Gateway

 * Route Table

 * Route Table Association

 * Security Group

 * Three EC2 Instances

These resources work together to create a network environment where compute instances can securely communicate internally while still allowing controlled access to the internet.

###  **Architecture Diagram**

<img width="1682" height="782" alt="Unt drawio (2)" src="https://github.com/user-attachments/assets/b48ef6f0-0ed0-46b3-9942-ff88424e265b" />

###  **Technologies Used**

* Terraform

* AWS EC2

* AWS VPC

* AWS Networking

* Infrastructure as Code
  
* Linux

###  Infrastructure Components 

VPC CIDR: 10.0.0.0/16

Provides isolated network environment.

###   Public Subnet 

CIDR: 10.0.2.0/24

Allows EC2 instances to communicate with the internet.

###   Security Group 

Allows inbound traffic:

SSH (22)

HTTP (80)

###   Kubernetes API (6443) 

etcd (2379)

###  EC2 Instances 

3 instances deployed:

Control Node
Worker Node 1
Worker Node 2

These will later support a Kubernetes cluster.

