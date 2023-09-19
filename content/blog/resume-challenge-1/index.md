---
title: "AWS Accounts and Organization"
description: "Creating our AWS Accounts and Organization. Using AWS Services such as CodeCommit, CodePipeline and tools such as ORG-FORMATIONS"
dateString: August 2023
draft: false
tags: ["AWS"]
weight: 99
cover:
    image: ""
---

## Setting Up the Management Account

Establishment of a **Management Account**, which serves as the central hub for controlling our AWS resources. This account plays a pivotal role in orchestrating and managing our entire AWS infrastructure.

## Building an AWS Organization with org-formation tool

To streamline the organization of our AWS accounts and resources, we leveraged the powerful `org-formation` tool. This nifty tool automates the process, making it easier to configure and manage our AWS Organization. With `org-formation`, we can define the structure of our organization, establish clear hierarchies, and maintain consistency across our AWS environment.

This tool takes the idea behind AWS Control Tower and enhances it with more features and capabilities.

## Embracing CodeCommit and CodePipeline

To ensure efficient version control and continuous integration/continuous deployment (CI/CD) processes, we embraced **CodeCommit** and **CodePipeline**. 

These AWS services allow us to commit and push changes to our codebase seamlessly. With Git at our fingertips, we have a robust mechanism to manage code versions and automate the deployment pipeline.

For our front-end and back-end solutions later on in the project , we will be utilizing **GitHub** and **GitHub Actions**.

## Implementing Automated Billing Alerts

To keep our expenses in check, we set up automated billing alerts. These alerts notify us when our AWS costs reach predefined thresholds, ensuring that we are always aware of our spending.

## Integrating CodeCommit with Visual Studio Code

For a seamless development experience, we integrated CodeCommit with **Visual Studio Code (VS Code)**. This integration simplifies the code collaboration process and allows our developers to work efficiently within their preferred development environment.

## Creating a Development Account

To maintain a clear separation between our production and development environments, we established a dedicated **Development Account**. This account serves as a safe sandbox for testing changes before they are pushed to the production environment. It's a crucial step to ensure the stability and reliability of our systems.

## Setting Up AWS Single Sign-On (SSO)

Enhancing the login experience for our team members was a priority. We implemented **AWS Single Sign-On (SSO)** to provide a more convenient and secure way for users to access AWS services. With SSO, users can access multiple AWS accounts and applications using a single set of credentials.

## Leveraging IAM Identity Center for Role Federation

To further enhance our security posture and access management, we utilized **IAM Identity Center** for role federation. This ensures that users have the appropriate permissions to access AWS resources while maintaining a high level of security and control.

With these foundational steps in place, we've laid the groundwork for a robust and organized AWS environment.
