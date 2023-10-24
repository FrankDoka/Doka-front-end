---
title: "CI / CD Pipeline for NGINX Server on a Docker Container Hosted in AWS"
description: "Automate the provisioning and deployment of a scalable and fault-tolerant web application using a CI/CD pipeline."
dateString: September 2023
draft: false
tags: ["AWS", "NGINX", "Automation", "CI/CD", "Terraform", "Docker", "Jenkins", "Ansible"]
weight: 101
cover:
    image: "images/jenkins-ansible.png"
---

# Continuous Deployment Pipeline for a Web Application on Docker Container Hosted in AWS

## Objective
To automate the provisioning and deployment of a web server within a Docker container on AWS. This project will incorporate tools and services such as **AWS, Terraform, Ansible, Jenkins, Docker, and OpenSSL**.

## Application Architecture and overview

1. Set up an NGINX server to serve a static webpage using OpenSSL for security.
2. Containerize the NGINX server using Docker.
3. Incorporate the user of Terraform to set up AWS infrastructure - providing scalability and reusability.
4. Setup configuration management using Ansible to manage our server configuration. Using dynamic inventory to manage our EC2 instances.
5. Create Jenkins pipeline to enhance automation for building, testing, deployment and streamlining updates.

## Project Phases

1. **[Understanding the Application and Tools](https://frankdoka.com/blog/ci-cd-docker-1)**
    - Delve into the application's design and get acquainted with the tools that will be employed

2. **[NGINX, OpenSSL, and the Static Site in Docker](https://frankdoka.com/blog/ci-cd-docker-2)**
    - Bundle NGINX, OpenSSL, and the static site into a Docker container.

3. **[Infrastructure as Code with Terraform](https://frankdoka.com/blog/ci-cd-docker-3)**
    - Use Terraform to set up the AWS infrastructure, providing a foundation for the Docker container deployment.

4. **[Ansible and Dynamic Inventory](https://frankdoka.com/blog/ci-cd-docker-4)**
    - Harness Ansible for configuration management of our server and orchestration. Use dynamic inventory to efficiently manage AWS EC2 instances.

5. **[Automated Deployments with Jenkins Pipeline](https://frankdoka.com/blog/ci-cd-docker-5)**
    - Craft and launch a Jenkins pipeline to automate the build, test, and deployment processes, ensuring consistent and streamlined updates.

## Conclusion
I demonstrated the synergy of automation and cloud solutions by integrating pivotal tools like Docker, Jenkins, Terraform, and Ansible to create a robust CI/CD pipeline. Ansible, with its dynamic inventory, further strengthened our deployment process, ensuring configuration consistency. The Jenkins pipeline enhanced the automation for deploying and also updating the web server.
