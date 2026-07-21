---
title: "Worklog Week 5"
date: 2026-07-10
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---


### Week 5 Objectives:

* Understand how to deliver website content using Amazon CloudFront.
* Learn more about Lightsail, EC2 Auto Scaling, CloudWatch, and services that support application deployment.
* Know how to combine S3 Static Website with CloudFront in the frontend model.

### Tasks to be carried out this week:

| Day | Task | Start date | Completion date | References |
| --- | --- | --- | --- | --- |
| 2 | - Studied Content Delivery Network and the role of Amazon CloudFront.<br>- Learned about Edge Location, cache, origin, and distribution. | 18/05/2026 | 18/05/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://000058.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/Introduction.html |
| 3 | - Learned how to use CloudFront with S3 Static Website.<br>- Took notes on origin domain, default root object, cache behavior, and HTTPS endpoint. | 19/05/2026 | 19/05/2026 | https://000058.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AmazonS3/latest/userguide/website-hosting-cloudfront-walkthrough.html <br> https://www.youtube.com/watch?v=5RxYavHbgVE&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=97 |
| 4 | - Learned about Amazon Lightsail and when Lightsail can be used for quick application deployment.<br>- Compared EC2 and Lightsail at a high level. | 20/05/2026 | 20/05/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/lightsail/latest/userguide/what-is-amazon-lightsail.html |
| 5 | - Learned about EC2 Auto Scaling and the concept of application scaling.<br>- Took notes on Launch Template, Auto Scaling Group, scaling policy, and health check. | 21/05/2026 | 21/05/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/autoscaling/ec2/userguide/what-is-amazon-ec2-auto-scaling.html <br> https://www.youtube.com/watch?v=bbLcPitXJSY&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=79 |
| 6 | - Learned basic CloudWatch for resource monitoring.<br>- Summarized the roles of S3, CloudFront, EC2/Lightsail, and CloudWatch in a web application model. | 22/05/2026 | 22/05/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/WhatIsCloudWatch.html |

### Lab implementation steps for week 5:

* Prepare an S3 bucket with a static website or an accessible origin.
* Open CloudFront Console and create a new Distribution.
* Configure Origin Domain to point to an S3 website endpoint or S3 bucket origin according to the lab requirements.
* Configure Default cache behavior, Viewer protocol policy, and Allowed HTTP methods.
* Set Default root object to index.html if using a static website.
* Wait until the distribution status becomes Deployed, then access the CloudFront domain to test the website.
* Check caching by modifying a file in S3 and observing the update time on CloudFront.
* Learn more about Lightsail for quick application deployment and EC2 Auto Scaling for increasing instance count when traffic grows.
* Summarize CloudWatch metrics that should be monitored when a website is delivered through CloudFront.

### Results achieved in week 5:

* Understood that CloudFront helps deliver content closer to users through edge locations.
* Understood the concepts of origin, distribution, and cache behavior.
* Knew how to combine S3 and CloudFront to host a static frontend.
* Understood the roles of Lightsail, Auto Scaling, and CloudWatch at a high level.
* Prepared the foundation for frontend deployment in the later project phase.


---
