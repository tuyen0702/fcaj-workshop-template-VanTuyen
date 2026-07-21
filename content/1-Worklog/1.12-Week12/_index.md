---
title: "Worklog Week 12"
date: 2026-07-10
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---


### Objectives for Week 12:

* Complete the AI Workflow of the project.
* Deploy PDF Generator Lambda, S3 Report Bucket, ReportLab Layer, and update DynamoDB after analysis is completed.
* Test the full workflow and complete the report.

### Tasks to be completed this week:

| Day | Task | Start Date | Completion Date | Reference Sources |
| --- | --- | --- | --- | --- |
| Monday | - Deploy PDF Generator Lambda.<br>- Receive analysis result and cost result from Step Functions.<br>- Call Amazon Bedrock to generate the final review content for the report. | 06/07/2026 | 06/07/2026 | https://docs.aws.amazon.com/lambda/latest/dg/welcome.html<br>https://docs.aws.amazon.com/bedrock/latest/userguide/what-is-bedrock.html<br>https://chatgpt.com/ |
| Tuesday | - Configure S3 Report Bucket to store report-data.json, report.html, and report.pdf.<br>- Write logic to upload reports to S3 using the structure reports/{reviewId}/. | 07/07/2026 | 07/07/2026 | https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html<br>https://docs.aws.amazon.com/lambda/latest/dg/python-handler.html<br>https://chatgpt.com/ |
| Wednesday | - Create a ReportLab Layer for Lambda to export PDF files.<br>- Add DejaVuSans fonts to support Vietnamese display in PDF.<br>- Attach the layer to PDF Generator Lambda and test PDF generation. | 08/07/2026 | 08/07/2026 | https://docs.aws.amazon.com/lambda/latest/dg/chapter-layers.html<br>https://docs.aws.amazon.com/lambda/latest/dg/python-layers.html<br>https://chatgpt.com/ |
| Thursday | - Add logic to update review history in DynamoDB after report generation succeeds.<br>- Update status from uploaded to completed and store score, detectedServices, recommendations, risks, costResult, and reportFiles. | 09/07/2026 | 09/07/2026 | https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Introduction.html<br>https://docs.aws.amazon.com/amazondynamodb/latest/APIReference/API_UpdateItem.html<br>https://chatgpt.com/ |
| Friday | - Test the full flow from frontend file upload to Step Functions, Bedrock analysis, cost estimation, report generation, and history display on the frontend.<br>- Hold a group meeting to complete the report, review screenshots, and prepare presentation content. | 10/07/2026 | 10/07/2026 | https://docs.aws.amazon.com/eventbridge/latest/userguide/eb-what-is.html<br>https://docs.aws.amazon.com/step-functions/latest/dg/welcome.html<br>https://docs.aws.amazon.com/bedrock/latest/userguide/what-is-bedrock.html |

### Lab implementation steps for Week 12:

* Create an S3 Report Bucket to store report results for each review.
* Create PDF Generator Lambda and configure environment variables REPORT_BUCKET, TABLE_NAME, MODEL_ID, and BEDROCK_REGION.
* Grant PDF Generator Lambda permissions: PutObject to the S3 Report Bucket, UpdateItem to DynamoDB, and InvokeModel to Bedrock.
* Write logic to receive analysis result and cost result from Step Functions.
* Generate report-data.json containing structured data, report.html for browser viewing, and report.pdf for download.
* Open CloudShell in the ap-southeast-1 Region and create a ReportLab Layer for Python 3.14.
* Install reportlab and pillow into the python folder of the layer, create a fonts folder, and add DejaVuSans.ttf/DejaVuSans-Bold.ttf.
* Zip the layer, download the zip file, create a new Lambda Layer, and attach it to PDF Generator Lambda.
* Register Vietnamese fonts in the ReportLab code so the PDF displays Vietnamese accents correctly.
* Update DynamoDB review history after the workflow completes: status completed, score, recommendations, risks, costResult, and reportFiles.
* Upload a test architecture from the frontend, check Step Functions execution, verify the report in S3, and check history on the web.

### Results achieved in Week 12:

* PDF Generator Lambda can generate HTML/PDF reports.
* S3 Report Bucket stores report files by reviewId.
* ReportLab Layer works and supports PDF generation.
* DynamoDB review history is updated after the workflow completes.
* Frontend can display review history and completed status.
* The group completed the report and tested the main project workflow.


---