---
title: "CI/CD App - Phase 1: Understanding the Application Architecture and Tools"
description: "Delving into the application's design and introducing the tools that will be used."
dateString: October 2023
draft: false
tags: ["Design", "NGINX", "Tools", "Automation", "CI/CD", "Docker"]
weight: 80
cover:
    image: ""
---

# Understanding the Application Architecture and Tools

Objective: To gain a foundational understanding of the project's architecture and the tools that will be pivotal in its execution.

## **Application Architecture**

- **NGINX Web Server**: Primary web server - set to serve a static webpage with OpenSSL.
- **Docker Container**: The NGINX server will be containerized using Docker to ensure consistent deployments and enhanced portability.

## **Toolset Introduction**

- **Docker**: A container platform that enables application encapsulation, ensuring a consistent environment from development to production.
- **Terraform**: An Infrastructure as Code (IaC) tool, Terraform allows provisioning and management of cloud resources using a script-driven approach.
- **Ansible**: A versatile automation tool employed for configuration management, application deployment, and task automation.
- **Jenkins**: As the CI/CD engine, Jenkins will automate significant parts of the development process, ensuring seamless and efficient deployments.

## **Project Hierarchy**
[Hierarchy](images/project_directory.png)

## **Conclusion**

In this Phase the application architecture and the toolset that will be used is discussed. The next phase will be about the creation of the Docker image and integrating NGINX with OpenSSL for the static website.
