---
title: "Worklog Week 9"
date: 2026-07-10
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---


### Objectives for Week 9:

* Start researching and defining the direction for the group project.
* Analyze system requirements and choose the project topic AI AWS Architecture Reviewer.
* Identify the main AWS services required in the project architecture.

### Tasks to be completed this week:

| Day | Task | Start Date | Completion Date | Reference Sources |
| --- | --- | --- | --- | --- |
| Monday | - Hold a group meeting to start the project phase.<br>- Discuss possible project directions that can be implemented on AWS.<br>- Agree to focus on the problem of supporting AWS architecture diagram analysis using AI. | 15/06/2026 | 15/06/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/bedrock/latest/userguide/what-is-bedrock.html |
| Tuesday | - Analyze requirements for the AI AWS Architecture Reviewer system.<br>- Define the input as an architecture diagram image and the output as review results, cost estimation, and report.<br>- Record the main functions: upload diagram, analyze architecture, estimate cost, generate report, and view history. | 16/06/2026 | 16/06/2026 | https://docs.aws.amazon.com/lambda/latest/dg/welcome.html<br>https://docs.aws.amazon.com/bedrock/latest/userguide/what-is-bedrock.html<br>https://chatgpt.com/ |
| Wednesday | - Research suitable services for frontend/backend.<br>- Choose S3 + CloudFront for frontend, API Gateway + Lambda for upload backend, and DynamoDB for review history. | 17/06/2026 | 17/06/2026 | https://docs.aws.amazon.com/AmazonS3/latest/userguide/WebsiteHosting.html<br>https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/Introduction.html<br>https://docs.aws.amazon.com/apigateway/latest/developerguide/welcome.html<br>https://chatgpt.com/ |
| Thursday | - Learn about EventBridge and Step Functions for automated workflows.<br>- Take notes on the flow S3 Object Created → EventBridge → Step Functions → Lambda processing. | 18/06/2026 | 18/06/2026 | https://docs.aws.amazon.com/eventbridge/latest/userguide/eb-what-is.html<br>https://docs.aws.amazon.com/step-functions/latest/dg/welcome.html<br>https://chatgpt.com/ |
| Friday | - Learn about Amazon Bedrock and the ability to use an AI model to analyze architecture images.<br>- Identify the main processing Lambdas: AI Analyzer, Cost Tool, and PDF Generator.<br>- Summarize the planned project architecture.<br>- Draw the complete architecture diagram. | 19/06/2026 | 19/06/2026 | https://www.youtube.com/watch?v=l8isyDe-GwY&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=2<br>https://chatgpt.com/ |

### Lab implementation steps for Week 9:

* Define the project problem: users upload an AWS architecture diagram and the system automatically analyzes it.
* List the main input/output: architecture image, detected service list, Well-Architected review, cost estimation, and report.
* Learn about S3 and CloudFront to serve the static frontend.
* Learn about API Gateway and Lambda to build the upload backend.
* Learn about DynamoDB to store metadata and review history.
* Learn about EventBridge and Step Functions to build an automated workflow after a file is uploaded.
* Learn about Amazon Bedrock to analyze architecture using AI.
* Learn about AWS Price List API for cost estimation.
* Draw the overall architecture diagram and agree on the implementation scope within the group.

### Results achieved in Week 9:

* The group selected the project topic AI AWS Architecture Reviewer.
* Defined the input/output and main functions of the system.
* Selected the main AWS services for the architecture.
* Built the overall processing flow from upload to report generation.
* Prepared the foundation for task assignment and implementation in the next week.


---