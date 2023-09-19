---
title: "Building the Front-End"
description: "Building the front end of our website using HTML,CSS,Javascript and Hugo. Hosting our website on AWS using S3, Cloudfront and Route 53."
dateString: August 2023
draft: false
tags: ["AWS"]
weight: 98
cover:
    image: ""
---

The second part of our cloud resume project journey! Today, we start building the front-end of our project, exploring new tools and techniques to enhance our skills and create a polished web presence.

## Crafting a Resume in HTML

Our first task was to create a digital resume. 

We decided to keep start simple and effective by coding it in **HTML**. This allowed us to structure the content precisely as we wanted it and provided a foundation for future styling.

## Styling with CSS

To make our resume visually appealing, we utilized **Cascading Style Sheets (CSS)**. 

With CSS, we transformed our plain HTML content into an aesthetically pleasing document that showcased our skills and experience.

## Hosting with a Static S3 Website, HTTPS, and DNS

With our resume ready, it was time to make it accessible to the world. 

We hosted it as a static website on **Amazon S3**, ensuring that it was served over **HTTPS** for security and that DNS was configured correctly for easy access.

## Configuring Route 53 and Routing Policies

To ensure seamless access to our website, we configured **Amazon Route 53**. This involved setting up routing policies and creating the necessary DNS records.

## Addressing Name Server Issues

One challenge we faced was related to name servers. We had to ensure that our domain was correctly configured with the name servers of the hosted zone. This step was crucial for proper domain resolution.

## Utilizing CloudFront for Enhanced Website Hosting

To boost the performance and security of our website, we utilized **Amazon CloudFront**.

This content delivery network (CDN) served as an intermediary between our basic S3 static hosting and the users, ensuring faster load times and added security.

## Creating SSL Certificate with ACM Manager

Security is paramount, so we secured our website with an **SSL certificate** from **AWS Certificate Manager (ACM)**. 

This step provided encryption and trustworthiness to our site, making it safer for visitors.

## Leveraging Hugo for Website Design

To give our website a professional and polished look, we turned to **Hugo**. 

This static site generator helped us create a visually appealing and responsive website with ease.

## Using GitHub and GitHub Actions for Deployment

For efficient website deployment, we employed **GitHub** and **GitHub Actions**. 

This streamlined the process and allowed us to automate deployments. However, we encountered a challenge related to images not showing up correctly.

## Overcoming Image Display Challenges

To address the image display issues, we implemented solutions like **PaperMod** and adjusted the content and static paths on our Hugo HTML website. These changes ensured that images were displayed correctly, enhancing the overall user experience.
