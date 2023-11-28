---
title: "Azure Kubernetes Web Store - Part 1"
description: "Initiating Design: Environment Setup and Docker Image Building"
dateString: November 2023
draft: false
tags: ["Azure", "Kubernetes", "Docker", "CI/CD", "Pipeline"]
weight: 84
cover:
    image: ""
---

# Azure Web Store - Part 1

This is the first blog post in the creation of building a Web Store on Azure using various technologies such as Docker and Kubernetes. We will first discuss initial design considerations and focus on setting up the environment and creating the Docker Images for the different sections of the Web Store.

## Overview:

We will integrate Azure, Kubernetes, and Docker to create a powerful and scalable web store. The blog posts will go through the steps from start to finish, from the foundational design to advanced CI/CD pipelines.

### Components and Services
 Web App
 3 Micro Services - Order, Product, Service
 Azure B2C
 Application Insights
 API Management
 Function App
 Power App
 Regression Suite

## Part 1: Initiating Design

This foundational phase sets the groundwork for the project.

### Key Objectives:

1. **Initial Design:**
   - Define architectural considerations for the Graceful Healing Path Store on Azure Kubernetes.
   - Outline the structure and components for optimal performance.

2. **Environment Setup:**
   - Configure the Azure environment to support Kubernetes deployment.
   - Explore the integration of essential services and tools for seamless development.

3. **Docker Image Building:**
   - Dive into the process of crafting Docker images tailored for the Azure Kubernetes environment.
   - Understand best practices for image optimization and ensuring compatibility.

### Steps:

#### Creating Azure Resources

- Deploy App Service (Graceful Healing Path Application), App Service Plan, and Container Registry onto Azure.

#### 01 - Build the Docker Images

Build the Docker Images locally for testing and deploying outside of Azure.
The Docker Images were pre-constructed using Java / Spring Boot and contain the Azure App Service and the Azure Kubernertes Services (3 micro services).
The code for the Docker Images will be available on the Github Project post at the conclusion of the proejct.

##### Prerequisites (Local development):

- Install Docker Desktop.
- Log in to your GitHub account and create a new repository for the application.
- Setup SSH keys so that you can update your repository while you locally work on your application.

##### Build and Run the Graceful Healing Path Service Docker Image

We can run and deploy the Docker Images locally, outside of Azure, in order to build and test our Images. We are also able to Administer our Azure Kubernetes Cluster. Below is a few example commands of how to get the Application Service Docker Image running.

Navigate to directory - cd gracefulhealingpath/gracefulhealingpathservice
Setup a local bridge for communication - docker network create gracefulhealingpathbridge
Build the docker Image - docker build -t gracefulhealingpathpetservice .
Run the Service - docker run --rm --net gracefulhealingpathbridge --name gracefulhealingpathservice -p 8081:8081 -e GRACEFULHEALINGPATHSERVICE_SERVER_PORT=8081 -d gracefulhealingpathservice:latest
Test the Service - Navigate to http://localhost:8081 to test that it is working correctly.
Use the command "docker ps" which should show one container running and the image command used to start the application.

##### Repeat the Process for the other components
Repeat the process for our other components - make sure when you run them to change the port's that you are using.
    *Graceful Healing Path Product Service Docker Image
    *Graceful Healing Path Order Service Docker Image
    *Graceful healing Path App Docker Image

When you are finished, you can use the following command to kill the running containers : 
docker kill $(docker ps -q)


## Summary

In Part 1 - We sucessfully set our initial Azure deployment as well as built and tested our docker images locally. In the following Part, we will take the Docker Image and push it to the Azure Container registry, configure app services for continous deployments of our Docker image updates, and configure GitHub Actions for CI / CD into App Service.