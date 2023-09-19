---
title: "API Backend Continuation and Frontend Integration"
description: "Integrating our website Frontend and our Backend services to create an example Visitor Counter Stat."
dateString: September 2023
draft: false
tags: ["AWS"]
weight: 96
cover:
    image: ""
---

# API Backend Continuation and Front-End Integration

we continued our exploration of the API backend and initiated the crucial integration between the front end and back end. Let's dive into the details of our progress:

## API Creation and Testing

- **API Gateway Route for Lambda Function**: We set up an API Gateway route in front of our Lambda function, configuring it to handle POST requests. This step was essential for creating a pathway for communication between our front end and back end.

- **Internal Testing with API Gateway**: We utilized the API Gateway's internal test console to ensure that our API was functioning as expected. This involved making requests to our Lambda function and verifying that we received the correct responses.

- **External Testing with Postman**: To expand our testing scope, we tested our API using Postman. This allowed us to verify that our API worked seamlessly when accessed externally.

- **Incrementing DynamoDB Count**: We created an API Gateway for Lambda, which invoked the Lambda function to increment the count in our DynamoDB table. We tested this functionality through various means, including browser and Postman, to ensure that the count increased as expected.

## Front-End and Back-End Integration

- **Connecting Front-End to Back-End**: The next crucial step was integrating the front end (our resume site hosted on S3) with the back end (our API). We aimed to display the visitor count on the homepage of our site.

- **Automated Tests**: We implemented automated tests to confirm the smooth operation of our integration. These tests were designed to validate that our system always performed as expected.

  1. **JavaScript Visitor Counter**: We created a JavaScript visitor counter that made HTTP requests to our API Gateway. While this was a straightforward task, we encountered some CORS (Cross-Origin Resource Sharing) issues between the browser and API, which we addressed. The goal was to display the visitor count on our web app.

  2. **Python Code Testing**: For comprehensive testing, we wrote automated tests against our API. These tests, often referred to as "smoke tests" or end-to-end tests, verified that our Lambda code worked correctly, permissions and configurations were accurate, and resources were deployed successfully. We employed Cypress, a JavaScript testing framework, to call our API endpoint and perform a series of checks:

     - Ensuring the API returned an updated value.
     - Verifying that the API correctly updated the database.
     - Confirming that the API responded to unexpected input.
     - Checking edge cases in our function logic, such as handling uninitialized visitor counts.

- **Front-End Updates and CI/CD**: We revisited the front end, incorporating it into our GitHub repository and enhancing our CI/CD (Continuous Integration/Continuous Deployment) pipeline. We also updated AWS secret keys for secure access.

- **Hugo Shortcode for Visitor Count**: To make it easier to display the visitor count on our website, we created a Hugo shortcode and added a new Visitors tab to test shortcodes.

- **Front-End Integration Challenges**: While the front end successfully fetched data from DynamoDB and displayed the visitor count, we encountered issues with updating the count correctly. These issues were primarily related to CORS policy restrictions.

- **CORS Policy Adjustment**: To resolve the CORS issue, we made necessary changes to the CORS policy on AWS to allow the website and enable the GET method.

With these accomplishments and challenges tackled, we're well on our way to creating a seamless integration between our front-end and back-end systems. 
