---
title: "AWS Accounts and Organization"
description: "Creating AWS Accounts and Organization. Using AWS Services such as CodeCommit, CodePipeline and tools such as ORG-FORMATIONS"
dateString: 
draft: false
tags: ["AWS"]
weight: 99
cover:
    image: ""
---

## Setting Up My Management Account

Established a **Management Account**, which serves as the central hub for controlling my AWS resources. This account plays a pivotal role in orchestrating and managing my entire AWS infrastructure.

## Building an AWS Organization with org-formation tool

To streamline the organization of my AWS accounts and resources, I've leveraged the powerful `org-formation` tool. This nifty tool automates the process, making it easier for me to configure and manage my AWS Organization. With `org-formation`, I can define the structure of my organization, establish clear hierarchies, and maintain consistency across my AWS environment.

This tool takes the idea behind AWS Control Tower and enhances it with more features and capabilities.

## Embracing CodeCommit and CodePipeline

To ensure efficient version control and continuous integration/continuous deployment (CI/CD) processes, I've embraced **CodeCommit** and **CodePipeline**. 

These AWS services allow me to commit and push changes to my codebase seamlessly. With Git at my fingertips, I have a robust mechanism to manage code versions and automate the deployment pipeline.

For my frontend and backend solutions later on in the project, I'll be utilizing **GitHub** and **GitHub Actions**.

## Implementing Automated Billing Alerts

Set up automated billing alerts. These alerts notify me when my AWS costs reach predefined thresholds, ensuring that I am always aware of my spending.

## Integrating CodeCommit with Visual Studio Code

For a seamless development experience, I've integrated CodeCommit with **Visual Studio Code (VS Code)**. This integration simplifies the code collaboration process and allows me to work efficiently within my preferred development environment.

## Creating a Development Account

To maintain a clear separation between my production and development environments, I've established a dedicated **Development Account**. This account serves as a safe sandbox for testing changes before they are pushed to the production environment. It's a crucial step to ensure the stability and reliability of my systems.

## Setting Up AWS Single Sign-On (SSO)

Enhancing the login experience for AWS sign-on to multiple AWS accounts through the use of roles. I implemented **AWS Single Sign-On (SSO)** to provide a more convenient and secure way for to access AWS services. With SSO, I can access multiple AWS accounts and applications using a single set of credentials.

## Leveraging IAM Identity Center for Role Federation

To further enhance my security posture and access management, I've utilized **IAM Identity Center** for role federation. This ensures that users have the appropriate permissions to access AWS resources while maintaining a high level of security and control.

With these foundational steps in place, I've laid the groundwork for a robust and organized AWS environment.
