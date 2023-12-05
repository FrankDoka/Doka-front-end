---
title: "Azure Web Store deployed on Kubernetes"
description: "Create and Automate a N-Tiered Azure architecture using Kubernetes and CI/CD methodologies"
dateString: November 2023
draft: false
tags: ["Azure", "Kubernetes", "Automation", "CI/CD", "API Management", "Docker"]
weight: 100
cover:
    image: ""
---

# Azure Web Store

Built a comprehensive Azure architecture with functional code, CI/CD, and various services for exploring Azure technologies. The project, centered around a Web Store application, provides hands-on experience with Azure services, demonstrating best practices in cloud development.

## Overview:

### Application Deployment

Gain practical insights into Azure App Dev Services through the deployment of a full-featured Azure Store Application and its dependencies.

**Live Deployment:** TBD

### Useful Scenarios Covered:

- CI/CD into Azure App Service & Azure Kubernetes Service.
- N-Tiered Architecture with correlated telemetry in Azure Application Insights.
- User authentication via Azure B2C.
- API Management, Deployment Slots, and Azure SDKs for Java and Spring Boot.

## Guides:

### Part 1: Environment Setup and Docker Image Build

- **Setup your environment:** Prerequisites and environment setup.
- **Build the Docker Images:** Build Store Application and Services Docker Images.

### Part 2: Azure Container Registry and App Service

- **Push Docker Images to ACR:** Push Docker Images to Azure Container Registry.
- **Configure App Service:** Continuous deployment of ACR Docker image updates.
- **GitHub Action for CI/CD:** Configure GitHub Action for CI/CD into App Service.

### Part 3: Azure Kubernetes Cluster and Configuration

- **Create AKS Cluster:** Create an Azure Kubernetes Cluster.
- **Configure Ingress Controller:** Configure NGINX Ingress controller.
- **Azure DevOps Pipeline for AKS:** Configure Pipeline for CI/CD into Azure Kubernetes Service.

### Part 4: Integration and Identity Management

- **Connect App and Services:** Integration of  App and Services.
- **Configure Application Insights:** Configure Apps to use Application Insights.
- **Configure API Management:** Configure API Management in front of Services.

### Part 5: DataOps and Automated Testing

- **DataOps with Databricks:** Configure Pipeline for CI/CD into Azure Databricks.
- **Automated Regression Tests:** Configure pipelines for automated regression tests.
- **Build and Deploy Azure Functions:** Build and Deploy Azure Functions.

### Part 6: Power Apps and Logic App

- **Canvas Power App:** Build a Canvas Power App with a Custom Connector.
- **Logic App Configuration:** Build a Logic App to send an email from Service Bus topic.

### Part 7: Infrastructure as Code and SignalR

- **IaC with Bicep:** Build a Bicep IaC Template.
- **SignalR Configuration:** Configure SignalR for Real-Time Analytics in the Client Browser.
