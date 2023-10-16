---
title: "Project: CI / CD Pipeline for a Web Application on a Docker Container Hosted in AWS"
description: "Automate the provisioning and deployment of a scalable and fault-tolerant web application using a CI/CD pipeline."
dateString: October 2023
draft: false
tags: ["AWS", "NGINX", "Automation", "CI/CD", "Terraform", "Docker", "Jenkins", "Ansible"]
weight: 100
cover:
    image: ""
---

# Continuous Deployment Pipeline for a Web Application on Docker Container Hosted in AWS

## Objective
To automate the provisioning and deployment of a web server within a Docker container on AWS. This project will incorporate tools and services such as **AWS, Terraform, Ansible, Jenkins, Docker, and OpenSSL**.

## Application Architecture

1. Set up an NGINX server to serve a static webpage, with OpenSSL for security.
2. Containerize the NGINX server using Docker.

## Project Phases

1. **[Understanding the Application and Tools](https://frankdoka.com/blog/CI-CD-Docker-1)**
    - Delve into the application's design and get acquainted with the tools that will be employed.

2. **[NGINX, OpenSSL, and the Static Site in Docker](https://frankdoka.com/blog/CI-CD-Docker-2)**
    - Bundle NGINX, OpenSSL, and the static site into a Docker container.

3. **[Infrastructure as Code with Terraform](https://frankdoka.com/blog/CI-CD-Docker-3)**
    - Use Terraform to set up the AWS infrastructure, providing a foundation for the Docker container deployment.

4. **[Ansible and Dynamic Inventory](https://frankdoka.com/blog/CI-CD-Docker-4)**
    - Harness Ansible for configuration management and orchestration. Use dynamic inventory to efficiently manage AWS EC2 instances.

5. **[Automated Deployments with Jenkins Pipeline](https://frankdoka.com/blog/CI-CD-Docker-5)**
    - Craft and launch a Jenkins pipeline to automate the build, test, and deployment processes, ensuring consistent and streamlined updates.

## Conclusion
I demonstrated the synergy of automation and cloud solutions by integrating pivotal tools like Docker, Jenkins, Terraform, and Ansible to create a robust CI/CD pipeline. Ansible, with its dynamic inventory, further strengthened our deployment process, ensuring configuration consistency across environments.