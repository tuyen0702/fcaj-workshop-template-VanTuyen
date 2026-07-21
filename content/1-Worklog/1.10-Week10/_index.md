---
title: "Worklog Week 10"
date: 2026-07-10
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---


### Week 10 Objectives:

* Hold a team meeting to assign tasks to each member.
* Design the overall project architecture and separate backend/frontend components.
* Deploy foundational components: S3 Static Website, CloudFront, API Gateway, and Lambda Upload Service.

### Tasks to be carried out this week:

| Day | Task | Start date | Completion date | References |
| --- | --- | --- | --- | --- |
| 2 | - Held a team meeting to assign implementation tasks to each member.<br>- Defined responsibility areas: frontend, upload backend, AI workflow, cost tool, report generator, and documentation. | 22/06/2026 | 22/06/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/ <br> https://chatgpt.com/ |
| 3 | - Designed the overall architecture of the system.<br>- Drew the processing flow: React Frontend → API Gateway → Lambda Upload Service → S3 Input Bucket → DynamoDB. | 23/06/2026 | 23/06/2026 | https://docs.aws.amazon.com/lambda/latest/dg/welcome.html<br>https://docs.aws.amazon.com/apigateway/latest/developerguide/welcome.html <br> https://chatgpt.com/ |
| 4 | - Configured S3 Static Website for the frontend.<br>- Prepared the React build files and configured the bucket to serve static content.<br>- Checked the website URL after uploading the frontend. | 24/06/2026 | 24/06/2026 | https://docs.aws.amazon.com/AmazonS3/latest/userguide/WebsiteHosting.html <br> https://chatgpt.com/ |
| 5 | - Configured CloudFront distribution for the frontend.<br>- Set up the origin pointing to S3, default root object, and tested access through the CloudFront domain. | 25/06/2026 | 25/06/2026 | https://docs.aws.amazon.com/AmazonS3/latest/userguide/website-hosting-cloudfront-walkthrough.html <br> https://chatgpt.com/ |
| 6 | - Designed and implemented API Gateway + Lambda Upload Service.<br>- Configured the POST /upload route, handled multipart upload, validated files, stored files in S3, and saved metadata to DynamoDB. | 26/06/2026 | 26/06/2026 | https://docs.aws.amazon.com/apigateway/latest/developerguide/http-api-develop.html<br>https://docs.aws.amazon.com/lambda/latest/dg/python-handler.html<br>https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Introduction.html <br> https://chatgpt.com/ |

### Lab implementation steps for week 10:

* Create an S3 bucket to host the frontend and upload the React build files after running the build command.
* Enable Static Website Hosting or prepare an S3 origin for CloudFront depending on the deployment approach.
* Create a CloudFront distribution, configure the origin to point to S3, and test the CloudFront domain.
* Create an S3 Input Bucket to store architecture files uploaded by users.
* Create a DynamoDB table to store review history using reviewId as the partition key.
* Create Lambda Upload Service and configure environment variables INPUT_BUCKET, TABLE_NAME, MAX_FILE_SIZE_MB, and ALLOWED_ORIGINS.
* Create an IAM role for Lambda with permission to PutObject into the S3 Input Bucket and PutItem into DynamoDB.
* Create an API Gateway HTTP API, add the POST /upload route, and integrate it with Lambda Upload Service.
* Configure CORS so the frontend can call API Gateway.
* Test upload using the frontend or curl, then check the file in S3 and metadata item in DynamoDB.

### Results achieved in week 10:

* The team assigned tasks clearly.
* Designed the overall architecture of the project.
* Configured frontend hosting using S3 and CloudFront.
* Created the API Gateway route for file upload.
* Lambda Upload Service could upload files to the S3 Input Bucket and save initial metadata to DynamoDB.


---
