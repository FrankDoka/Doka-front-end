---
title: "Backend technologies and APIs"
description: "Creating our backend foundation using AWS Services such as API Gateways, Lambda, and DynamoDB. Exploring IAM Permissions more indepth."
dateString: August 2023
draft: false
tags: ["AWS"]
weight: 97
cover:
    image: ""
---

# Getting Started with Backend Technologies and APIs

Today, we dived into the world of backend technologies and APIs, setting the foundation for our project's functionality.

## JavaScript Code to API to Database (DynamoDB)

Our mission for today was to establish the crucial link between our JavaScript code and the database. We opted for **Amazon DynamoDB** as our database solution and AWS services like **API Gateway** and **Lambda** to create a robust backend.

## Setting Up the Lambda Function

Our first task was to get a Lambda function talking to the database. We set up a Python Lambda function using the AWS Web Console, laying the groundwork for processing requests from our front-end application.

## DynamoDB Table Setup

Creating a DynamoDB table was a straightforward "point and click" process. This table would serve as our data store, enabling us to store and retrieve data efficiently.

## Writing Python Code for Lambda

To make our Lambda function functional, we wrote Python code that would interact with DynamoDB. We tested this code from the AWS Console to ensure that data could be successfully saved to the database.

## IAM Permissions Configuration

Ensuring secure access between our Lambda function and the DynamoDB table was paramount. We configured IAM permissions to manage access and control over who can interact with these AWS resources.

## Exploring SAM (Serverless Application Model)

We delved into the world of SAM, an open-source framework for building serverless applications. Our goal was to set up SAM locally, allowing us to develop and test Lambda functions and DynamoDB tables locally before deploying them to AWS.

## Creating the DynamoDB Database in AWS

We created a DynamoDB database in our AWS environment and established the Lambda function's connection to the database, with the appropriate IAM permissions to facilitate communication.

## API Development

With our backend infrastructure in place, we started building the API. The API would enable our front-end website to communicate with the Lambda function, facilitating data transfer between the user interface and the database.

## API Gateway Configuration

API Gateway was our choice for managing API endpoints. We configured it to route requests to our Lambda function, allowing for seamless data transfer between the website and the backend.

## Testing the API Locally

We used the API Gateway's internal test console to perform a "Hello World" test, ensuring that the API was correctly connected to our Lambda function.

## External Testing with Postman

To ensure that our API was ready for prime time, we grabbed its public URL from the API Gateway and conducted tests using external API testing services like Postman. Our goal was to verify that the Lambda function produced the expected output.

With these steps, we've made significant progress in establishing our backend infrastructure and API. Stay tuned as we continue to develop and refine our project, bringing it one step closer to completion.