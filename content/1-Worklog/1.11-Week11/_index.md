---
title: "Worklog Week 11"
date: 2026-07-10
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---


### Week 11 Objectives:

* Deploy automated processing components for the project.
* Configure S3 Input Bucket, DynamoDB, EventBridge, Step Functions, AI Analyzer Lambda, and Cost Tool Lambda.
* Test the automated workflow after users upload files.

### Tasks to be carried out this week:

| Day | Task | Start date | Completion date | References |
| --- | --- | --- | --- | --- |
| 2 | - Held a team meeting to report implementation progress.<br>- Rechecked upload backend, S3 Input Bucket, and DynamoDB review history table.<br>- Added necessary fields for review items: reviewId, fileName, status, uploadDate, updatedAt. | 29/06/2026 | 29/06/2026 | https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html<br>https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Introduction.html<br>https://chatgpt.com/ |
| 3 | - Configured S3 Input Bucket to send Object Created events to EventBridge.<br>- Created an EventBridge rule to capture new file upload events from the input bucket. | 30/06/2026 | 30/06/2026 | https://docs.aws.amazon.com/AmazonS3/latest/userguide/EventBridge.html<br>https://docs.aws.amazon.com/eventbridge/latest/userguide/eb-rules.html<br>https://chatgpt.com/ |
| 4 | - Created a Step Functions state machine to orchestrate the AI Workflow.<br>- Designed states: AnalyzeArchitectureWithAI, EstimateCost, and GenerateReport.<br>- Configured input/output paths between states. | 01/07/2026 | 01/07/2026 | https://docs.aws.amazon.com/step-functions/latest/dg/welcome.html<br>https://docs.aws.amazon.com/step-functions/latest/dg/concepts-amazon-states-language.html<br>https://chatgpt.com/ |
| 5 | - Deployed AI Analyzer Lambda.<br>- Configured permission to read from S3 Input Bucket and invoke Amazon Bedrock.<br>- Tested Lambda reading an image from S3 and returning the list of detected AWS services. | 02/07/2026 | 02/07/2026 | https://docs.aws.amazon.com/lambda/latest/dg/welcome.html<br>https://docs.aws.amazon.com/bedrock/latest/userguide/what-is-bedrock.html<br>https://chatgpt.com/ |
| 6 | - Deployed Cost Tool Lambda.<br>- Called AWS Price List API to get prices for services with supported mapping.<br>- Combined Bedrock to generate cost review and optimization suggestions.<br>- Tested Step Functions running through Analyzer and Cost Tool. | 03/07/2026 | 03/07/2026 | https://docs.aws.amazon.com/aws-cost-management/latest/APIReference/Welcome.html<br>https://docs.aws.amazon.com/bedrock/latest/userguide/what-is-bedrock.html<br>https://chatgpt.com/ |

### Lab implementation steps for week 11:

* In the S3 Input Bucket, enable Amazon EventBridge in Properties so the bucket sends events to EventBridge.
* Create an EventBridge rule with an event pattern that captures Object Created events from the input bucket.
* Configure the target of the EventBridge rule as the Step Functions state machine.
* Use an input transformer to pass bucket, key, and region into the workflow.
* Create a Step Functions state machine with AnalyzeArchitectureWithAI, EstimateCost, and GenerateReport steps.
* Create AI Analyzer Lambda and configure MODEL_ID and BEDROCK_REGION.
* Grant AI Analyzer Lambda permission to read objects from S3 Input Bucket and call the Bedrock model.
* Test AI Analyzer using a sample event containing bucket, key, and region.
* Create Cost Tool Lambda and configure permissions for pricing:GetProducts and bedrock:InvokeModel.
* Test Step Functions using an uploaded object and check the output of each state.

### Results achieved in week 11:

* EventBridge could capture file upload events from the S3 Input Bucket.
* Step Functions could orchestrate Lambdas in the correct order.
* AI Analyzer Lambda connected to Amazon Bedrock for architecture analysis.
* Cost Tool Lambda could estimate costs for several common AWS services.
* The team tested the automated workflow up to the analysis and cost estimation steps.


---
