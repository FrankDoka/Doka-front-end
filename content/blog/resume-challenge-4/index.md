---
title: "API Backend continuation and Frontend integration"
description: "Integrating website frontend and backend services to create an example visitor counter stat."
dateString: 
draft: false
tags: ["AWS"]
weight: 96
cover:
    image: ""
---

# Progress in API Backend and Front-End Integration

In my journey into the world of API backend development, I initiated the crucial integration between my front-end and back-end systems.

## API Creation and Testing

- **API Gateway Route for Lambda Function**: I established an API Gateway route in front of my Lambda function, configuring it to handle POST requests. This setup paved the way for communication between my front-end and back-end components.

- **Internal Testing with API Gateway**: To ensure the functionality of my API, I harnessed the API Gateway's internal test console. I rigorously tested the API by making requests to my Lambda function and confirming that the responses aligned with my expectations.

- **External Testing with Postman**: Expanding my testing scope, I employed Postman to test my API externally. This thorough testing approach verified that my API functioned seamlessly when accessed from external sources.

- **Incrementing DynamoDB Count**: One of my pivotal achievements involved creating an API Gateway for Lambda, enabling it to invoke the Lambda function to increment the count in my DynamoDB table. I conducted comprehensive testing through different channels, including browsers and Postman, to ensure the count incremented as intended.

## Front-End and Back-End Integration

- **Connecting Front-End to Back-End**: The next critical milestone was to establish a seamless connection between my front-end (hosted on S3) and the back-end (my API). My objective was to display the visitor count on the homepage of my website.

- **Automated Tests**: I implemented automated testing procedures to validate the smooth operation of my integration. These tests ensured that my system consistently performed as expected.

  1. **JavaScript Visitor Counter**: I developed a JavaScript visitor counter that made HTTP requests to my API Gateway. Although this task was relatively straightforward, I encountered CORS (Cross-Origin Resource Sharing) issues between the browser and API. These issues were successfully addressed to enable the display of visitor counts on my web app.

  2. **Python Code Testing**: To ensure comprehensive testing, I created automated tests for my API. These tests, often referred to as "smoke tests" or end-to-end tests, verified the correctness of my Lambda code, the accuracy of permissions and configurations, and the successful deployment of resources. Cypress, a JavaScript testing framework, was utilized to call my API endpoint and perform a series of checks, including verifying updated values, correct database updates, handling of unexpected input, and edge case scenarios.

- **Front-End Updates and CI/CD**: I revisited the front end, integrating it into my GitHub repository and enhancing my CI/CD (Continuous Integration/Continuous Deployment) pipeline. I also reinforced security by updating AWS secret keys for access.

- **Hugo Shortcode for Visitor Count**: To simplify the display of the visitor count on my website, I crafted a Hugo shortcode and introduced a new Visitors tab for shortcode testing.

- **Front-End Integration Challenges**: While the front end successfully fetched data from DynamoDB and displayed the visitor count, challenges emerged when updating the count accurately. These challenges primarily stemmed from CORS policy restrictions.

- **CORS Policy Adjustment**: To overcome the CORS issue, I made essential changes to the CORS policy on AWS. These adjustments allowed for seamless communication between the website and the API, including GET method access.

With these achievements and challenges addressed, I am making substantial progress toward achieving a seamless integration between my front-end and back-end systems.
