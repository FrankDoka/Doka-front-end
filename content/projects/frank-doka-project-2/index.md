---
title: "Project Details - Login System and Text to Speech Conversion"
description: "Outline of Project Details for Login System with additional tools"
dateString: September 2023
draft: false
tags: ["AWS"]
weight: 94
cover:
    image: ""
---

## Setting Up Project Details

Description : Create a user login system that will integrate AWS Services. Have a user profile page and use AWS Cognito to allow users to have certain functions depending on the authorization of the user. Offer services such as text to speech in various languages conversions and also services such as offering document conversion. Offer possible AI image generation service among other services.

## AWS Services Used

AWS Serices Used: AWS Cognito, AWS Lambda, DynamoDB, SES, SNS, SQS, API Gateway, AWS Polly and possibly more.

## Frontend and Backend

Frontend: Login page with Registration (requiring username / password / email / bday etc.) and button to register / login to the system.
After Login: Default to user profile page with information and specific tabs that user has access too. Also have option to logout of the system.

Backend: AWS Cognito to handle User pool and Authentication.
         AWS Lambda functions to do handle user authorization credentials.
		 DynamoDB to store user data and other data.
		 AWS S3 to store text files for conversion and documents for conversion.
		 SES/SNS/SQS? To confirm email for validity of user creation and also for forgot password.
		 API + API Gateway to take data input from user.
		 AWS Polly text to speech conversion in multiple languages
		 Session management - best practices?


## Additional procedures
		 
Use CI/CD Methods + Github + Github actions to provide pipeline for the frontend and the backend components.
Use Terraform for the creation and update / maintanence of the resources required for the project.
Deploy on Dev environment + testing before moving to Production environment.
Design tool - Excalidraw - https://excalidraw.com/.

## Steps

1) Initial setup of the Project. Writing project description and details along with desired AWS services to use.
2) Design Diagram of the Project.
3) Implement rudimentary frontend + backend Login system using AWS Cognito.
4) Implement advanced frontend user interface with user profile page and access rights to certain content depending on user level.
5) With login system completed - start work on Text to speech conversion tool.
