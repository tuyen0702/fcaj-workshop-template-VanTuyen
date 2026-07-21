---
title: "Worklog Week 6"
date: 2026-07-10
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---


### Objectives for Week 6:

* Understand basic security concepts on AWS.
* Understand the Shared Responsibility Model, IAM, Cognito, KMS, Security Hub, and security best practices.
* Learn how to organize access permissions to AWS resources more securely.

### Tasks to be completed this week:

| Day | Task | Start Date | Completion Date | Reference Sources |
| --- | --- | --- | --- | --- |
| Monday | - Study the Shared Responsibility Model.<br>- Distinguish AWS security responsibilities from user responsibilities when deploying a system. | 25/05/2026 | 25/05/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://000005.awsstudygroup.com/vi/<br>https://aws.amazon.com/compliance/shared-responsibility-model/ |
| Tuesday | - Study IAM in more detail: user, group, role, policy, and permission boundary at a conceptual level.<br>- Take notes on the least privilege principle and avoid using the root user for daily work. | 26/05/2026 | 26/05/2026 | https://000002.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/IAM/latest/UserGuide/introduction.html |
| Wednesday | - Learn about IAM Policy and how to read JSON policies.<br>- Learn about Allow, Deny, Action, Resource, and Condition.<br>- Take notes on how to grant Lambda permissions to access S3/DynamoDB within a specific scope. | 27/05/2026 | 27/05/2026 | https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies.html |
| Thursday | - Learn about Amazon Cognito, KMS, and Security Hub at an overview level.<br>- Take notes on Cognito for authentication, KMS for encryption, and Security Hub for security checks. | 28/05/2026 | 28/05/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/cognito/latest/developerguide/what-is-amazon-cognito.html<br>https://docs.aws.amazon.com/kms/latest/developerguide/overview.html<br>https://docs.aws.amazon.com/securityhub/latest/userguide/what-is-securityhub.html |
| Friday | - Learn some S3 Security Best Practices.<br>- Summarize a security checklist: MFA, IAM least privilege, bucket policy, encryption, logging, and public access control. | 29/05/2026 | 29/05/2026 | https://docs.aws.amazon.com/AmazonS3/latest/userguide/security-best-practices.html |

### Lab implementation steps for Week 6:

* Open the IAM Console and create an IAM user according to the lab content if a separate practice user is required.
* Create an IAM Group and attach a suitable policy to the group, prioritizing minimum permissions based on the lab needs.
* Create an IAM Policy in JSON format and carefully read the components Effect, Action, Resource, and Condition.
* Create an IAM Role for an AWS service such as EC2 or Lambda if the lab requires a service to access another resource.
* Try Switch Role or test user permissions after attaching policies.
* Create a restricted policy to observe how IAM controls allowed or denied actions.
* Check S3 bucket security: Block Public Access, bucket policy, and encryption.
* Learn about KMS key for data encryption and Security Hub for aggregating security findings.
* Delete test users/keys/policies if they are no longer used to reduce security risks.

### Results achieved in Week 6:

* Understood the shared responsibility model on AWS.
* Understood that IAM is an important component for access control.
* Learned how to read basic JSON policies.
* Understood the roles of Cognito, KMS, and Security Hub at an overview level.
* Understood the need to limit permissions by service and resource when deploying Lambda.


---