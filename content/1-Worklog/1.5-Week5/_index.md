---
title: "Worklog Week 5"
date: 2026-07-10
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---


### Objectives for Week 5:

* Understand how to distribute website content using Amazon CloudFront.
* Learn more about Lightsail, EC2 Auto Scaling, CloudWatch, and services that support application deployment.
* Learn how to combine S3 Static Website with CloudFront in a frontend model.

### Tasks to be completed this week:

| Day | Task | Start Date | Completion Date | Reference Sources |
| --- | --- | --- | --- | --- |
| Monday | - Learn about Content Delivery Network and the role of Amazon CloudFront.<br>- Learn about Edge Location, cache, origin, and distribution. | 18/05/2026 | 18/05/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://000058.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/Introduction.html |
| Tuesday | - Learn how to use CloudFront with S3 Static Website.<br>- Take notes on origin domain, default root object, cache behavior, and HTTPS endpoint. | 19/05/2026 | 19/05/2026 | https://000058.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AmazonS3/latest/userguide/website-hosting-cloudfront-walkthrough.html |
| Wednesday | - Learn about Amazon Lightsail and cases where Lightsail can be used to deploy applications quickly.<br>- Compare EC2 and Lightsail at an overview level. | 20/05/2026 | 20/05/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/lightsail/latest/userguide/what-is-amazon-lightsail.html |
| Thursday | - Learn about EC2 Auto Scaling and the concept of application scaling.<br>- Take notes on Launch Template, Auto Scaling Group, scaling policy, and health check. | 21/05/2026 | 21/05/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/autoscaling/ec2/userguide/what-is-amazon-ec2-auto-scaling.html |
| Friday | - Learn basic CloudWatch monitoring for resources.<br>- Summarize the roles of S3, CloudFront, EC2/Lightsail, and CloudWatch in a web app model. | 22/05/2026 | 22/05/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/WhatIsCloudWatch.html |

### Lab implementation steps for Week 5:

* Prepare an S3 bucket with a static website or an origin that can be accessed.
* Open the CloudFront Console and create a new Distribution.
* Configure Origin Domain to point to the S3 website endpoint or S3 bucket origin according to the lab requirements.
* Configure Default cache behavior, Viewer protocol policy, and Allowed HTTP methods.
* Set Default root object as index.html if using a static website.
* Wait until the distribution status becomes Deployed, then access the CloudFront domain to test the website.
* Test caching by changing a file in S3 and observing the update time on CloudFront.
* Learn more about Lightsail for quick application deployment and EC2 Auto Scaling for increasing the number of instances when traffic grows.
* Summarize the CloudWatch metrics that should be monitored when the website is distributed through CloudFront.

### Results achieved in Week 5:

* Understood that CloudFront helps distribute content closer to users through edge locations.
* Understood the concepts of origin, distribution, and cache behavior.
* Learned how to combine S3 and CloudFront to host a static frontend.
* Understood the roles of Lightsail, Auto Scaling, and CloudWatch at an overview level.
* Prepared the foundation for frontend deployment in the project later.


---