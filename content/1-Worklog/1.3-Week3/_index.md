---
title: "Worklog Week 3"
date: 2026-07-10
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---


### Week 3 Objectives:

* Understand Amazon EC2 and Compute services on AWS.
* Understand the components used when creating EC2: AMI, Instance Type, Key Pair, Security Group, EBS, User Data, and Metadata.
* Know how to launch, connect to, and manage an EC2 instance at a basic level.

### Tasks to be carried out this week:

| Day | Task | Start date | Completion date | References |
| --- | --- | --- | --- | --- |
| 2 | - Studied the overview of Amazon EC2 and the role of EC2 in cloud architecture.<br>- Learned about Instance Type, vCPU, RAM, instance family, and how to choose a suitable instance. | 04/05/2026 | 04/05/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://000004.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/concepts.html <br> https://www.youtube.com/watch?v=TQFwQAre0H4&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=59 |
| 3 | - Learned about AMI, operating system, root volume, and EC2 instance lifecycle.<br>- Took notes on EC2 states: pending, running, stopped, and terminated. | 05/05/2026 | 05/05/2026 | https://000004.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AMIs.html |
| 4 | - Learned about Key Pair and methods to remotely access EC2.<br>- Learned SSH for Linux instances and RDP for Windows instances.<br>- Took notes on key file permission issues when using SSH on Windows. | 06/05/2026 | 06/05/2026 | https://000004.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-key-pairs.html |
| 5 | - Learned about Amazon EBS, root volume, data volume, and snapshot.<br>- Learned how User Data is used to run scripts when EC2 is initialized.<br>- Took notes on using User Data to install a basic web server. | 07/05/2026 | 07/05/2026 | https://000004.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AmazonEBS.html<br>https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/user-data.html |
| 6 | - Learned about EC2 Metadata and the role of IAM Role for EC2.<br>- Summarized the process of creating an EC2 instance from the Console.<br>- Recorded a basic security checklist when deploying EC2. | 08/05/2026 | 08/05/2026 | https://000004.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/instancedata-data-retrieval.html<br>https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles_use_switch-role-ec2.html |

### Lab implementation steps for week 3:

* Open EC2 Console, choose Launch Instance, and name the instance according to the lab content.
* Choose a suitable AMI, such as Amazon Linux or Ubuntu, then choose a small instance type such as t2.micro/t3.micro if suitable for Free Tier.
* Create or select a Key Pair for SSH connection, download the .pem file, and store it in a safe folder.
* Configure Network Settings: choose VPC, subnet, and Security Group that allows SSH from personal IP.
* Check Storage, root volume, and EBS capacity attached to the instance.
* Launch the instance, wait until it is running, and check Public IPv4 address/Public DNS.
* Use SSH to connect to EC2 and verify the OS with basic commands such as hostname, uname, and df -h.
* Try reading EC2 metadata or checking IAM Role if the instance is attached to a role.
* Stop or terminate the instance after completing the lab to avoid costs.

### Results achieved in week 3:

* Understood the role of EC2 in Compute services.
* Understood the components required when creating an EC2 instance.
* Knew how to connect to EC2 using SSH/RDP at a basic level.
* Understood the role of EBS volume and snapshot.
* Knew that User Data can automate software installation when an instance is initialized.


---