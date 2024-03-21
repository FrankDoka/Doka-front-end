---
title: "Backend technologies and APIs"
description: "Creating backend foundation using AWS Services such as API Gateways, Lambda, and DynamoDB. Exploring IAM Permissions more indepth."
dateString: 
draft: false
tags: ["AWS"]
weight: 97
cover:
    image: ""
---

# Embarking on Backend Technologies and API Development

I delved into the realm of backend technologies and APIs, laying the essential groundwork for the functionality of my project.

## JavaScript Code to API to Database (DynamoDB)

My primary mission was to establish a seamless connection between my JavaScript code and the database. I chose **Amazon DynamoDB** as my database solution and employed AWS services like **API Gateway** and **Lambda** to construct a robust backend.

## Setting Up the Lambda Function

My initial task involved configuring a Python Lambda function through the AWS Web Console. This setup paved the way for processing requests from my front-end application.

## DynamoDB Table Setup

Creating a DynamoDB table was a straightforward process, achieved through simple "point and click" actions. This table serves as my data store, facilitating efficient data storage and retrieval. I then took this a step further and created a local DynamoDB database and learned to create the database using IaC.

## Writing Python Code for Lambda

To empower my Lambda function, I meticulously crafted Python code to interact with DynamoDB. Rigorous testing from the AWS Console ensured successful data storage in the database.

## IAM Permissions Configuration

Safeguarding access between my Lambda function and the DynamoDB table remained a priority. I meticulously configured IAM permissions to manage access and maintain control over interactions with these AWS resources.

## Exploring SAM (Serverless Application Model)

My journey included an exploration of SAM, an open-source framework tailored for building serverless applications. My aim was to set up SAM locally, enabling the development and testing of Lambda functions and DynamoDB tables in a local environment before deployment to AWS.

## Creating the DynamoDB Database in AWS

Within my AWS environment, I established a DynamoDB database and seamlessly configured the Lambda function's connection to it. IAM permissions were thoughtfully set up to facilitate smooth communication.

## API Development

With my backend infrastructure in place, I embarked on the development of the API. This API will serve as the conduit for communication between my front-end website and the Lambda function, facilitating seamless data exchange.

## API Gateway Configuration

My choice for managing API endpoints was API Gateway. Skillful configuration ensured that requests were efficiently routed to the Lambda function, enabling effective data transfer between the website and the backend.

## Testing the API Locally

I leveraged the internal test console of the API Gateway to conduct a "Hello World" test, ensuring the correctness of the API's connection to the Lambda function.

## External Testing with Postman

To confirm the readiness of my API for real-world usage, I obtained its public URL from the API Gateway and subjected it to rigorous testing using external API testing tools such as Postman. My objective was to verify that the Lambda function produced the expected output.

With these strategic steps, I've made significant progress in establishing my backend infrastructure and API.