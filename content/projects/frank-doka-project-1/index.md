---
title: "Cloud Resume Challenge"
description: "Build a cloud-hosted resume website, showcasing cloud skills."
dateString: September 2023
draft: false
tags: ["AWS"]
weight: 201
cover:
    image: "images/cover.png"
---

## Intro

The AWS Cloud Resume Challenge is an engaging, hands-on initiative designed to elevate your AWS cloud skills. Participants are challenged to build a professional resume website hosted exclusively on AWS infrastructure. This practical project hones your ability to deploy, configure, and secure AWS services, including EC2, S3,Route 53, Lambda, DynamoDB and much more.

It offers an exceptional opportunity to showcase your expertise to prospective employers while developing proficiency in cloud computing. By completing this challenge, you not only bolster your AWS knowledge but also create a tangible asset for your career, making you a more competitive candidate in the ever-evolving field of cloud technology.

## Project Overview
**This is a high level overview of the steps I took during this challenge:**

1. **HTML Resume:** Start by creating a professional resume using HTML.

2. **CSS Styling:** Style your resume using CSS to enhance its visual appeal and formatting.

3. **Static Website:** Host your resume on a static S3 website. Optionally, consider utilizing an EC2 instance if required.

4. **HTTPS Security:** Ensure the security of your S3 website by enabling HTTPS. Utilize Amazon CloudFront for this purpose.

5. **Custom DNS:** Point a custom DNS name to your CloudFront distribution using Amazon Route 53 for a personalized web address.

6. **JavaScript Visitor Counter:** Implement a visitor counter on your website using JavaScript to display the number of site visitors.

7. **Database for Visitor Counter:** Use DynamoDB to store and manage the visitor counter data efficiently, benefiting from its on-demand pricing model.

8. **API Creation:** Develop an API that communicates with the database and accepts requests from your web app. AWS API Gateway combined with Lambda can help accomplish this.

9. **Python Integration:** Utilize Python for Lambda functions to enhance the functionality of your serverless architecture.

10. **Testing:** Implement robust testing for your Python code to ensure its reliability and performance.

11. **Infrastructure as Code (IaC):** Configure AWS resources like DynamoDB tables, API Gateway, and Lambda functions using an AWS SAM (Serverless Application Model) template. Deploy these resources effortlessly using AWS SAM CLI.

12. **Source Control:** Employ GitHub for version control, enabling seamless updates to both the back-end API and front-end website.

13. **CI/CD (Backend):** Implement GitHub Actions to automate tests and deployments. Whenever updates are pushed to your SAM template or Python code, tests are executed, and if successful, the SAM app is packaged and deployed to AWS.

14. **CI/CD (Frontend):** Maintain a separate GitHub repository for your website code. Configure GitHub Actions to automatically update the S3 bucket when code changes occur (consider adding logic to invalidate CloudFront cache in code). Avoid committing AWS credentials to your code.

15. **Blog Post Integration:** Include a link to a concise blog post within your resume text. This post should highlight key learnings and experiences gained throughout the project.


