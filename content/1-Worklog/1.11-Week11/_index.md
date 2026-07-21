---
title: "Worklog Week 11"
date: 2026-07-10
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---


### Objectives for Week 11:

* Deploy automated processing components for the project.
* Configure S3 Input Bucket, DynamoDB, EventBridge, Step Functions, AI Analyzer Lambda, and Cost Tool Lambda.
* Test the automatic workflow after users upload files.

### Tasks to be completed this week:

| Day | Task | Start Date | Completion Date | Reference Sources |
| --- | --- | --- | --- | --- |
| Monday | - Hold a group meeting to report progress.<br>- Recheck the upload backend, S3 Input Bucket, and DynamoDB review history table.<br>- Add required fields to review items: reviewId, fileName, status, uploadDate, and updatedAt. | 29/06/2026 | 29/06/2026 | https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html<br>https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Introduction.html<br>https://chatgpt.com/ |
| Tuesday | - Configure the S3 Input Bucket to send Object Created events to EventBridge.<br>- Create an EventBridge rule to capture new file upload events from the input bucket. | 30/06/2026 | 30/06/2026 | https://docs.aws.amazon.com/AmazonS3/latest/userguide/EventBridge.html<br>https://docs.aws.amazon.com/eventbridge/latest/userguide/eb-rules.html<br>https://chatgpt.com/ |
| Wednesday | - Create a Step Functions state machine to orchestrate the AI Workflow.<br>- Design states: AnalyzeArchitectureWithAI, EstimateCost, and GenerateReport.<br>- Configure input/output path between states. | 01/07/2026 | 01/07/2026 | https://docs.aws.amazon.com/step-functions/latest/dg/welcome.html<br>https://docs.aws.amazon.com/step-functions/latest/dg/concepts-amazon-states-language.html<br>https://chatgpt.com/ |
| Thursday | - Deploy AI Analyzer Lambda.<br>- Configure permission to read the S3 Input Bucket and invoke Amazon Bedrock.<br>- Test Lambda to read an image from S3 and return the detected AWS services. | 02/07/2026 | 02/07/2026 | https://docs.aws.amazon.com/lambda/latest/dg/welcome.html<br>https://docs.aws.amazon.com/bedrock/latest/userguide/what-is-bedrock.html<br>https://chatgpt.com/ |
| Friday | - Deploy Cost Tool Lambda.<br>- Call AWS Price List API to retrieve prices for services with mapping.<br>- Combine Bedrock to generate cost explanations and optimization suggestions.<br>- Test Step Functions execution through Analyzer and Cost Tool. | 03/07/2026 | 03/07/2026 | https://docs.aws.amazon.com/aws-cost-management/latest/APIReference/Welcome.html<br>https://docs.aws.amazon.com/bedrock/latest/userguide/what-is-bedrock.html<br>https://chatgpt.com/ |

### Lab implementation steps for Week 11:

* Open the S3 Input Bucket and enable Amazon EventBridge in the Properties section so the bucket sends events to EventBridge.
* Create an EventBridge rule with an event pattern to capture Object Created events from the input bucket.
* Configure the target of the EventBridge rule as the Step Functions state machine.
* Use an input transformer to pass bucket, key, and region to the workflow.
* Create a Step Functions state machine with the steps AnalyzeArchitectureWithAI, EstimateCost, and GenerateReport.
* Create AI Analyzer Lambda and configure MODEL_ID and BEDROCK_REGION.
* Grant AI Analyzer Lambda permission to read objects from the S3 Input Bucket and invoke the Bedrock model.
* Test AI Analyzer using a sample event containing bucket, key, and region.
* Create Cost Tool Lambda and configure permissions pricing:GetProducts and bedrock:InvokeModel.
* Test Step Functions with an uploaded object and check the output of each state.

### Results achieved in Week 11:

* EventBridge can capture upload events from the S3 Input Bucket.
* Step Functions can orchestrate Lambda functions in the correct order.
* AI Analyzer Lambda can connect to Amazon Bedrock to analyze architecture.
* Cost Tool Lambda can estimate costs for several common AWS services.
* The group tested the automatic workflow up to the analysis and cost estimation steps.


---