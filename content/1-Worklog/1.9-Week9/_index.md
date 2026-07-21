---
title: "Worklog Week 9"
date: 2026-07-10
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---


### Week 9 Objectives:

* Start researching and defining the direction of the group project.
* Analyze system requirements and choose the AI AWS Architecture Reviewer topic.
* Identify the main AWS services required in the project architecture.

### Tasks to be carried out this week:

| Day | Task | Start date | Completion date | References |
| --- | --- | --- | --- | --- |
| 2 | - Held a team meeting to begin the project phase.<br>- Discussed possible project directions that could be implemented on AWS.<br>- Agreed to focus on the problem of supporting AWS architecture diagram analysis using AI. | 15/06/2026 | 15/06/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/bedrock/latest/userguide/what-is-bedrock.html <br> https://chatgpt.com/ |
| 3 | - Analyzed requirements for the AI AWS Architecture Reviewer system.<br>- Defined the input as an architecture diagram image and the output as review results, cost estimation, and report.<br>- Took notes on main functions: upload diagram, analyze architecture, estimate cost, generate report, view history. | 16/06/2026 | 16/06/2026 | https://docs.aws.amazon.com/lambda/latest/dg/welcome.html<br>https://docs.aws.amazon.com/bedrock/latest/userguide/what-is-bedrock.html <br> https://chatgpt.com/ |
| 4 | - Researched suitable services for frontend/backend.<br>- Chose S3 + CloudFront for frontend, API Gateway + Lambda for upload backend, and DynamoDB for review history. | 17/06/2026 | 17/06/2026 | https://docs.aws.amazon.com/AmazonS3/latest/userguide/WebsiteHosting.html<br>https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/Introduction.html<br>https://docs.aws.amazon.com/apigateway/latest/developerguide/welcome.html <br> https://chatgpt.com/ |
| 5 | - Learned about EventBridge and Step Functions for automated workflows.<br>- Took notes on the flow S3 Object Created → EventBridge → Step Functions → Lambda processing. | 18/06/2026 | 18/06/2026 | https://docs.aws.amazon.com/eventbridge/latest/userguide/eb-what-is.html<br>https://docs.aws.amazon.com/step-functions/latest/dg/welcome.html <br> https://chatgpt.com/ |
| 6 | - Learned about Amazon Bedrock and the ability to use AI models to analyze architecture images.<br>- Identified the main processing Lambdas: AI Analyzer, Cost Tool, and PDF Generator.<br>- Summarized the planned architecture of the project.<br>- Proceeded to draw the complete architecture diagram. | 19/06/2026 | 19/06/2026 | https://www.youtube.com/watch?v=l8isyDe-GwY&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=2<br>https://chatgpt.com/ |

### Lab implementation steps for week 9:

* Define the project problem: users upload AWS architecture diagrams and the system automatically analyzes them.
* List main inputs/outputs: architecture image, detected services, Well-Architected review, cost estimation, and report.
* Explore S3 and CloudFront for serving the static frontend.
* Explore API Gateway and Lambda for building the upload backend.
* Explore DynamoDB for storing metadata and review history.
* Explore EventBridge and Step Functions for building an automated workflow after file upload.
* Explore Amazon Bedrock for AI-based architecture analysis.
* Explore AWS Price List API for cost estimation.
* Draw the overall architecture diagram and agree on the implementation scope within the team.

### Results achieved in week 9:

* The team selected the AI AWS Architecture Reviewer topic.
* Defined the input/output and main system functions.
* Selected the main AWS services for the architecture.
* Built the overall processing flow from upload to report generation.
* Prepared the foundation for task assignment and implementation in the following week.


---
