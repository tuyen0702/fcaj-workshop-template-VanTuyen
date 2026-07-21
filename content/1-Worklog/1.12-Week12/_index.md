---
title: "Worklog Week 12"
date: 2026-07-10
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---


### Week 12 Objectives:

* Complete the AI Workflow of the project.
* Deploy PDF Generator Lambda, S3 Report Bucket, ReportLab Layer, and DynamoDB update after analysis completion.
* Test the full workflow and complete the report.

### Tasks to be carried out this week:

| Day | Task | Start date | Completion date | References |
| --- | --- | --- | --- | --- |
| 2 | - Deployed PDF Generator Lambda.<br>- Received analysis result and cost result from Step Functions.<br>- Called Amazon Bedrock to generate final review content for the report. | 06/07/2026 | 06/07/2026 | https://docs.aws.amazon.com/lambda/latest/dg/welcome.html<br>https://docs.aws.amazon.com/bedrock/latest/userguide/what-is-bedrock.html<br>https://chatgpt.com/ |
| 3 | - Configured S3 Report Bucket to store report-data.json, report.html, and report.pdf.<br>- Wrote logic to upload reports to S3 using the structure reports/{reviewId}/. | 07/07/2026 | 07/07/2026 | https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html<br>https://docs.aws.amazon.com/lambda/latest/dg/python-handler.html <br> https://chatgpt.com/ |
| 4 | - Created a ReportLab Layer for Lambda to export PDF files.<br>- Added DejaVuSans font to support Vietnamese display in PDF.<br>- Attached the layer to PDF Generator Lambda and tested PDF generation. | 08/07/2026 | 08/07/2026 | https://docs.aws.amazon.com/lambda/latest/dg/chapter-layers.html<br>https://docs.aws.amazon.com/lambda/latest/dg/python-layers.html <br> https://chatgpt.com/ |
| 5 | - Added logic to update review history in DynamoDB after report generation succeeds.<br>- Updated status from uploaded to completed, and stored score, detectedServices, recommendations, risks, costResult, and reportFiles. | 09/07/2026 | 09/07/2026 | https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Introduction.html<br>https://docs.aws.amazon.com/amazondynamodb/latest/APIReference/API_UpdateItem.html <br> https://chatgpt.com/ |
| 6 | - Tested the full flow from frontend upload to Step Functions, Bedrock analysis, cost estimation, report generation, and review history display on the frontend.<br>- Held a team meeting to finalize the report, review screenshots, and prepare presentation content. | 10/07/2026 | 10/07/2026 | https://docs.aws.amazon.com/eventbridge/latest/userguide/eb-what-is.html<br>https://docs.aws.amazon.com/step-functions/latest/dg/welcome.html<br>https://docs.aws.amazon.com/bedrock/latest/userguide/what-is-bedrock.html |

### Lab implementation steps for week 12:

* Create an S3 Report Bucket to store report results for each review.
* Create PDF Generator Lambda and configure environment variables REPORT_BUCKET, TABLE_NAME, MODEL_ID, and BEDROCK_REGION.
* Grant PDF Generator Lambda permissions: PutObject to S3 Report Bucket, UpdateItem to DynamoDB, and InvokeModel with Bedrock.
* Write logic to receive analysis result and cost result from Step Functions.
* Create report-data.json for structured data, report.html for browser viewing, and report.pdf for download.
* Open CloudShell in region ap-southeast-1 and create a ReportLab Layer for Python 3.14.
* Install reportlab and pillow into the python directory of the layer, create a fonts folder, and add DejaVuSans.ttf/DejaVuSans-Bold.ttf.
* Zip the layer, download the zip file, create a new Lambda Layer, and attach it to PDF Generator Lambda.
* Register Vietnamese fonts in ReportLab code so the PDF displays Vietnamese accents correctly.
* Update DynamoDB review history after the workflow completes: status completed, score, recommendations, risks, costResult, and reportFiles.
* Upload a test architecture from the frontend, verify that Step Functions runs successfully, check the report in S3, and check the history on the web.

### Results achieved in week 12:

* PDF Generator Lambda generated HTML/PDF reports.
* S3 Report Bucket stored report files by reviewId.
* ReportLab Layer worked and supported PDF file generation.
* DynamoDB review history was updated after the workflow completed.
* Frontend could display review history and completed status.
* The team completed the report and tested the main project workflow.


---