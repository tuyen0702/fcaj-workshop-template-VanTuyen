---
title: "Worklog Week 8"
date: 2026-07-10
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---


### Objectives for Week 8:

* Understand monitoring, operations, and optimization on AWS.
* Learn about CloudWatch Logs, CloudWatch Alarms, SNS, Resource Tags, AWS Budgets, and Cost Management.
* Learn how to use logs and alarms to monitor a serverless system.

### Tasks to be completed this week:

| Day | Task | Start Date | Completion Date | Reference Sources |
| --- | --- | --- | --- | --- |
| Monday | - Study the overview of system operations on AWS.<br>- Learn about CloudWatch Metrics, CloudWatch Logs, and CloudWatch Dashboard. | 08/06/2026 | 08/06/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/WhatIsCloudWatch.html |
| Tuesday | - Learn about CloudWatch Alarms and how to set alert thresholds.<br>- Take notes on commonly monitored metrics: errors, duration, invocations, throttles, CPU, and memory. | 09/06/2026 | 09/06/2026 | https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/AlarmThatSendsEmail.html |
| Wednesday | - Learn about Amazon SNS and how to send notifications when an event or alarm occurs.<br>- Take notes on the model CloudWatch Alarm → SNS → Email notification. | 10/06/2026 | 10/06/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/sns/latest/dg/welcome.html |
| Thursday | - Learn about Resource Tags, Resource Groups, and how to use tags to organize resources.<br>- Take notes on tags by project, environment, owner, and cost center. | 11/06/2026 | 11/06/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/tag-editor/latest/userguide/tagging.html |
| Friday | - Learn about AWS Budgets, Cost Management, and cost optimization approaches.<br>- Take notes on approaches such as right-sizing, stopping unused resources, controlling data transfer, and using suitable storage classes. | 12/06/2026 | 12/06/2026 | https://docs.aws.amazon.com/cost-management/latest/userguide/what-is-costmanagement.html |

### Lab implementation steps for Week 8:

* Open the CloudWatch Console to view Metrics of resources that have been created, such as EC2, Lambda, or S3 if data is available.
* Open CloudWatch Logs to check log groups and log streams of Lambda or related services.
* Create a sample CloudWatch Alarm based on a suitable metric such as Lambda Errors or EC2 CPUUtilization.
* Create an SNS Topic, add an email subscription, and confirm the email subscription.
* Connect CloudWatch Alarm with the SNS Topic to send notifications when the alarm changes state.
* Add tags to resources using keys such as Project, Environment, Owner, or CostCenter.
* Learn about AWS Budgets and create a cost alert budget if needed.
* Summarize cost optimization methods: stopping unused resources, right-sizing, controlling data transfer, and cleaning up resources after labs.

### Results achieved in Week 8:

* Understood that CloudWatch is an important service for monitoring resources and applications.
* Understood how CloudWatch Logs helps debug Lambda.
* Understood how SNS can be used to send email notifications.
* Learned how to use tags to organize and manage resources by project.
* Understood basic cost optimization principles when learning and practicing AWS.


---