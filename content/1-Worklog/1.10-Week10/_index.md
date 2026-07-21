---
title: "Worklog Week 10"
date: 2026-07-10
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---


### Objectives for Week 10:

* Hold a group meeting to divide tasks among members.
* Design the overall project architecture and separate backend/frontend components.
* Deploy the foundation components: S3 Static Website, CloudFront, API Gateway, and Lambda Upload Service.

### Tasks to be completed this week:

| Day | Task | Start Date | Completion Date | Reference Sources |
| --- | --- | --- | --- | --- |
| Monday | - Hold a group meeting to assign tasks to each member.<br>- Define responsibility areas: frontend, upload backend, AI workflow, cost tool, report generator, and documentation. | 22/06/2026 | 22/06/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/<br>https://chatgpt.com/ |
| Tuesday | - Design the overall system architecture.<br>- Draw the processing flow: React Frontend → API Gateway → Lambda Upload Service → S3 Input Bucket → DynamoDB. | 23/06/2026 | 23/06/2026 | https://docs.aws.amazon.com/lambda/latest/dg/welcome.html<br>https://docs.aws.amazon.com/apigateway/latest/developerguide/welcome.html |
| Wednesday | - Configure S3 Static Website for the frontend.<br>- Prepare the React build files and configure the bucket to serve static content.<br>- Check the website URL after uploading the frontend. | 24/06/2026 | 24/06/2026 | https://docs.aws.amazon.com/AmazonS3/latest/userguide/WebsiteHosting.html<br>https://chatgpt.com/ |
| Thursday | - Configure CloudFront distribution for the frontend.<br>- Set the origin to S3, configure the default root object, and test access through the CloudFront domain. | 25/06/2026 | 25/06/2026 | https://docs.aws.amazon.com/AmazonS3/latest/userguide/website-hosting-cloudfront-walkthrough.html<br>https://chatgpt.com/ |
| Friday | - Design and deploy API Gateway + Lambda Upload Service.<br>- Configure route POST /upload, process multipart upload, validate files, store files in S3, and save metadata to DynamoDB. | 26/06/2026 | 26/06/2026 | https://docs.aws.amazon.com/apigateway/latest/developerguide/http-api-develop.html<br>https://docs.aws.amazon.com/lambda/latest/dg/python-handler.html<br>https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Introduction.html<br>https://chatgpt.com/ |

### Lab implementation steps for Week 10:

* Create an S3 bucket to host the frontend and upload the React build files after running the build command.
* Enable Static Website Hosting or prepare an S3 origin for CloudFront depending on the deployment approach.
* Create a CloudFront distribution, configure the origin pointing to S3, and test the CloudFront domain.
* Create an S3 Input Bucket to store architecture files uploaded by users.
* Create a DynamoDB table to store review history using reviewId as the partition key.
* Create the Lambda Upload Service and configure environment variables INPUT_BUCKET, TABLE_NAME, MAX_FILE_SIZE_MB, and ALLOWED_ORIGINS.
* Create an IAM role for Lambda with permission to PutObject into the S3 Input Bucket and PutItem into DynamoDB.
* Create an API Gateway HTTP API, add route POST /upload, and integrate it with Lambda Upload Service.
* Configure CORS so the frontend can call API Gateway.
* Test upload using the frontend or curl, then check the file in S3 and metadata item in DynamoDB.

### Results achieved in Week 10:

* The group assigned work clearly to members.
* Designed the overall architecture of the project.
* Configured frontend hosting using S3 and CloudFront.
* Created an API Gateway route for file upload.
* Lambda Upload Service can upload files to the S3 Input Bucket and save initial metadata to DynamoDB.


---