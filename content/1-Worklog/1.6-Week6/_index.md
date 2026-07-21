---
title: "Worklog Week 6"
date: 2026-07-10
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---


### Week 6 Objectives:

* Understand basic security concepts on AWS.
* Understand Shared Responsibility Model, IAM, Cognito, KMS, Security Hub, and security best practices.
* Know how to organize AWS resource access more securely.

### Tasks to be carried out this week:

| Day | Task | Start date | Completion date | References |
| --- | --- | --- | --- | --- |
| 2 | - Studied the Shared Responsibility Model.<br>- Distinguished AWS security responsibilities and user responsibilities when deploying systems. | 25/05/2026 | 25/05/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://000005.awsstudygroup.com/vi/<br>https://aws.amazon.com/compliance/shared-responsibility-model/ |
| 3 | - Studied IAM in more detail: user, group, role, policy, and permission boundary at a conceptual level.<br>- Took notes on the least privilege principle and avoiding root user for daily tasks. | 26/05/2026 | 26/05/2026 | https://000002.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/IAM/latest/UserGuide/introduction.html <br> https://www.youtube.com/watch?v=N_vlJGAqZxo&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=151 |
| 4 | - Learned about IAM Policy and how to read JSON policies.<br>- Learned about Allow, Deny, Action, Resource, and Condition.<br>- Took notes on how to grant Lambda access to S3/DynamoDB within a specific scope. | 27/05/2026 | 27/05/2026 | https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies.html |
| 5 | - Learned about Amazon Cognito, KMS, and Security Hub at a high level.<br>- Took notes on using Cognito for authentication, KMS for encryption, and Security Hub for security checks. | 28/05/2026 | 28/05/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/cognito/latest/developerguide/what-is-amazon-cognito.html<br>https://docs.aws.amazon.com/kms/latest/developerguide/overview.html<br>https://docs.aws.amazon.com/securityhub/latest/userguide/what-is-securityhub.html <br> https://www.youtube.com/watch?v=pZ2fgEFK3Vs&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=152 |
| 6 | - Learned several S3 Security Best Practices.<br>- Summarized a security checklist: MFA, IAM least privilege, bucket policy, encryption, logging, and public access control. | 29/05/2026 | 29/05/2026 | https://docs.aws.amazon.com/AmazonS3/latest/userguide/security-best-practices.html |

### Lab implementation steps for week 6:

* Open IAM Console and create an IAM user according to the lab content if a separate practice user is needed.
* Create an IAM Group and attach a suitable policy to the group, prioritizing minimum permissions required by the lab.
* Create an IAM Policy in JSON format and carefully read Effect, Action, Resource, and Condition.
* Create an IAM Role for an AWS service such as EC2 or Lambda if the lab requires the service to access another resource.
* Try Switch Role or check user permissions after attaching the policy.
* Create a restricted policy to observe how IAM controls allowed and denied actions.
* Check S3 bucket security: Block Public Access, bucket policy, and encryption.
* Learn how KMS keys are used for data encryption and how Security Hub aggregates security findings.
* Delete test users/keys/policies if no longer used to reduce security risks.

### Results achieved in week 6:

* Understood the AWS Shared Responsibility Model.
* Understood that IAM is a key component for controlling access.
* Knew how to read a basic JSON policy.
* Understood the roles of Cognito, KMS, and Security Hub at a high level.
* Knew that permissions must be limited by service and resource when deploying Lambda.


---
