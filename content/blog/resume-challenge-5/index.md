---
title: "IaC, CI/CD Enhancements, smoke testing"
description: "Diving into tools such as Terraform to utilize IaC. Enhancing our CI/CD pipeline and testing."
dateString: September 2023
draft: false
tags: ["AWS"]
weight: 95
cover:
    image: ""
---

# Smoke Testing, Infrastructure as Code (IAC), and CI/CD Enhancements

We focused on enhancing our project with smoke testing, delved into Infrastructure as Code (IAC) using AWS Serverless Application Model (SAM) and Terraform, and continued to refine our Continuous Integration/Continuous Deployment (CI/CD) pipeline.

## Smoke Testing

- **Install Cypress**: We began the day by installing Cypress, a powerful end-to-end testing framework. Cypress would be instrumental in performing smoke tests to validate our system's functionality.

- **Smoke Test Execution**: With Cypress in place, we conducted smoke tests to check the data being sent and to cover edge cases. These tests ensured that our system behaved as expected under various scenarios.

## Infrastructure as Code (IAC)

- **AWS SAM Template**: We explored AWS Serverless Application Model (SAM) templates, a convenient way to define our serverless infrastructure. This included configuring components like Lambda functions, DynamoDB, and API Gateway.

- **CloudFormation and Terraform**: We delved into two IAC tools, CloudFormation and Terraform, to manage our cloud resources. CloudFormation is AWS's native tool for IAC, while Terraform is a versatile, multi-cloud tool widely adopted in the industry. Terraform uses a domain-specific configuration language called HCL.

## CI/CD Backend

- **GitHub Actions Workflow**: We leveraged GitHub Actions to automate our CI/CD pipeline. This streamlined the process of deploying updates, ensuring that our SAM application package and Python code were properly tested before deployment.

- **Workflow Steps**:
   - **Build Step**: In this step, we packaged up our Lambda function code and installed any necessary dependencies. The output was a zipped Lambda function artifact and a configuration file ready for deploying resources.
   - **Deploy Step**: We utilized our chosen IAC tool (Terraform) to deploy AWS resources based on the defined templates.
   - **Smoke Test Step**: To ensure the API functioned as expected, we ran Cypress API tests, confirming that the deployed API met our requirements.

## Backend Infrastructure with Terraform

- **Terraform Configuration**: We began setting up our backend infrastructure as code using Terraform. This included creating a `main.tf` file and configuring an EC2 instance for testing purposes.

- **Lambda Function and DynamoDB Policies**: We reviewed our Lambda function code and ensured that the necessary policies and permissions were correctly defined.

- **DynamoDB Table Configuration**: We created the base DynamoDB table and continued to explore how to add items to it programmatically.

- **API Gateway Enhancements**: We improved our API Gateway configuration by attaching the Lambda function and configuring the GET function. Additionally, we addressed CORS (Cross-Origin Resource Sharing) settings, allowing the GET method.

## GitHub Repository Setup

- **Terraform and Backend Repository**: We initiated a GitHub repository dedicated to our backend code and testing. This repository would host our Terraform configurations and serve as a central hub for backend development.

As Day 5 concludes, we've made significant strides in our project, focusing on testing, infrastructure as code, and CI/CD enhancements. Our commitment to automation and robust testing ensures a reliable and scalable project. Stay tuned for further updates as we continue to fine-tune and expand our system.