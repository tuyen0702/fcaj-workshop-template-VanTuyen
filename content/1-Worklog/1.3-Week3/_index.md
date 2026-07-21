---
title: "Worklog Week 3"
date: 2026-07-10
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---


### Objectives for Week 3:

* Understand Amazon EC2 and the Compute service group on AWS.
* Understand the components required when creating an EC2 instance: AMI, Instance Type, Key Pair, Security Group, EBS, User Data, and Metadata.
* Be able to launch, connect to, and manage an EC2 instance at a basic level.

### Tasks to be completed this week:

| Day | Task | Start Date | Completion Date | Reference Sources |
| --- | --- | --- | --- | --- |
| Monday | - Study the overview of Amazon EC2 and its role in cloud architecture.<br>- Learn about Instance Type, vCPU, RAM, instance family, and how to choose a suitable instance. | 04/05/2026 | 04/05/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://000004.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/concepts.html |
| Tuesday | - Learn about AMI, operating system, root volume, and EC2 instance lifecycle.<br>- Take notes on EC2 states: pending, running, stopped, and terminated. | 05/05/2026 | 05/05/2026 | https://000004.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AMIs.html |
| Wednesday | - Learn about Key Pair and methods to remotely access EC2.<br>- Learn about SSH for Linux instances and RDP for Windows instances.<br>- Take notes on key file permission issues when using SSH on Windows. | 06/05/2026 | 06/05/2026 | https://000004.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-key-pairs.html |
| Thursday | - Learn about Amazon EBS, root volume, data volume, and snapshot.<br>- Learn how User Data runs scripts when EC2 is launched.<br>- Take notes on how to use User Data to install a basic web server. | 07/05/2026 | 07/05/2026 | https://000004.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AmazonEBS.html<br>https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/user-data.html |
| Friday | - Learn about EC2 Metadata and the role of IAM Role for EC2.<br>- Summarize the process of creating an EC2 instance from the Console.<br>- Write a basic security checklist when deploying EC2. | 08/05/2026 | 08/05/2026 | https://000004.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/instancedata-data-retrieval.html<br>https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles_use_switch-role-ec2.html |

### Lab implementation steps for Week 3:

* Open the EC2 Console, select Launch Instance, and name the instance according to the lab content.
* Choose a suitable AMI, such as Amazon Linux or Ubuntu, then choose a small instance type such as t2.micro/t3.micro if it is appropriate for Free Tier.
* Create or select a Key Pair for SSH connection, download the .pem file, and store it in a safe folder.
* Configure Network Settings: choose VPC, subnet, and Security Group allowing SSH from the personal IP address.
* Check the Storage section, root volume, and EBS volume size attached to the instance.
* Launch the instance, wait until it reaches the running state, then check its Public IPv4 address/Public DNS.
* Use SSH to connect to EC2 and check the operating system with basic commands such as hostname, uname, and df -h.
* Try reading EC2 metadata or checking IAM Role if the instance is attached to a role.
* Stop or terminate the instance after finishing the lab to avoid additional costs.

### Results achieved in Week 3:

* Understood the role of EC2 in the Compute service group.
* Understood the required components when creating an EC2 instance.
* Learned how to connect to EC2 using SSH/RDP at a basic level.
* Understood the role of EBS volume and snapshot.
* Understood that User Data can automate software installation when an instance starts.


---