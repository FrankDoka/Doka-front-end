---
title: "CI/CD App - Phase 3: Infrastructure as Code with Terraform"
description: "Setting up the AWS infrastructure using Terraform for our Docker container deployment."
dateString: October 2023
draft: false
tags: ["AWS", "Terraform", "Infrastructure", "IaC"]
weight: 78
cover:
    image: ""
---

# Infrastructure as Code with Terraform

Objective: To make use of Terraform's Infrastructure as Code (IaC) capabilities to create the necessary AWS infrastructure, providing a foundation for deploying the Docker-contained NGINX web server on AWS.

## **Terraform Configuration**

Terraform offers a systematic and script-driven approach to manage and provision cloud resources. The configuration will primarily focus on deploying an EC2 instance configured specifically for this project. We will be using variable names and collaborating with Ansibile and Dynamic Inventory to further automate the configuration.

1. **Setting Up Terraform**: Create a main.tf and a variables.tf to hold the Terraform configuration information. Since a limited amount of resources are being used, all definitions can be placed in our main.tf

[Terraform Main.tf](images/terraform-main.png)

We will use the variables.tf file to connect our project with our Ansibile Dynamic Inventory.

[Terraform Variables](images/terraform-variables.png)

## **Conclusion**

With the use of Terraform our infrastructure setup has been streamlined, ensuring consistency and reproducibility. With AWS resources now in place, it is time to look towards Ansible and Dynamic Inventory for our configuration needs.