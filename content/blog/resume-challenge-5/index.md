---
title: "IaC, CI/CD Enhancements, Smoke testing"
description: "Diving into tools such as Terraform to utilize IaC. Enhancing CI/CD pipeline and testing."
dateString: 
draft: false
tags: ["AWS"]
weight: 95
cover:
    image: ""
---

# Smoke Testing, Infrastructure as Code (IAC), and CI/CD Enhancements

In this phase of my project, I focused on enhancing my project with smoke testing, delved into Infrastructure as Code (IAC) using AWS Serverless Application Model (SAM) and Terraform, and continued to refine my Continuous Integration/Continuous Deployment (CI/CD) pipeline.

## Smoke Testing

- **Install Cypress**: Installing Cypress, a powerful end-to-end testing framework. Cypress would be instrumental in performing smoke tests to validate my system's functionality.

- **Smoke Test Execution**: With Cypress in place, I conducted smoke tests to check the data being sent and to cover edge cases. These tests ensured that my system behaved as expected under various scenarios.

## Infrastructure as Code (IAC)

- **AWS SAM Template**: I explored AWS Serverless Application Model (SAM) templates, a convenient way to define my serverless infrastructure. This included configuring components like Lambda functions, DynamoDB, and API Gateway.

- **CloudFormation and Terraform**: I delved into two IAC tools, CloudFormation and Terraform, to manage my cloud resources. CloudFormation is AWS's native tool for IAC, while Terraform is a versatile, multi-cloud tool widely adopted in the industry. Terraform uses a domain-specific configuration language called HCL.

## CI/CD Backend

- **GitHub Actions Workflow**: I leveraged GitHub Actions to automate my CI/CD pipeline. This streamlined the process of deploying updates, ensuring that my SAM application package and Python code were properly tested before deployment.

- **Workflow Steps**:
   - **Build Step**: In this step, I packaged up my Lambda function code and installed any necessary dependencies. The output was a zipped Lambda function artifact and a configuration file ready for deploying resources.
   - **Deploy Step**: I utilized my chosen IAC tool (Terraform) to deploy AWS resources based on the defined templates.
   - **Smoke Test Step**: To ensure the API functioned as expected, I ran Cypress API tests, confirming that the deployed API met my requirements.

## Backend Infrastructure with Terraform

- **Terraform Configuration**: I began setting up my backend infrastructure as code using Terraform. This included creating a `main.tf` file and configuring an EC2 instance for testing purposes.

- **Lambda Function and DynamoDB Policies**: I reviewed my Lambda function code and ensured that the necessary policies and permissions were correctly defined.

- **DynamoDB Table Configuration**: I created the base DynamoDB table and continued to explore how to add items to it programmatically.

- **API Gateway Enhancements**: I improved my API Gateway configuration by attaching the Lambda function and configuring the GET function. Additionally, I addressed CORS (Cross-Origin Resource Sharing) settings, allowing the GET method.

## GitHub Repository Setup

- **Terraform and Backend Repository**: I initiated a GitHub repository dedicated to my backend code and testing. This repository would host my Terraform configurations and serve as a central hub for backend development.

I've made significant strides in my project, focusing on testing, infrastructure as code, and CI/CD enhancements. My commitment to automation and robust testing ensures a reliable and scalable project.
