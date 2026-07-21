---
title: "Worklog Week 2"
date: 2026-07-10
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---


### Objectives for Week 2:

* Understand Amazon VPC and basic networking components on AWS.
* Understand the roles of Subnet, Route Table, Internet Gateway, NAT Gateway, Security Group, and Network ACL.
* Be able to read basic network diagrams and identify connection flows inside a VPC.

### Tasks to be completed this week:

| Day | Task | Start Date | Completion Date | Reference Sources |
| --- | --- | --- | --- | --- |
| Monday | - Study the Amazon Virtual Private Cloud module.<br>- Learn the concepts of VPC, CIDR block, public subnet, and private subnet.<br>- Take notes on the role of VPC in isolating resources on AWS. | 27/04/2026 | 27/04/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://000003.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html |
| Tuesday | - Learn about Subnet and Route Table.<br>- Distinguish between public subnet and private subnet based on the route to the Internet Gateway.<br>- Redraw a simple VPC model including a public subnet and a private subnet. | 28/04/2026 | 28/04/2026 | https://000003.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/vpc/latest/userguide/configure-subnets.html |
| Wednesday | - Learn about Internet Gateway and NAT Gateway.<br>- Take notes on Internet access flow from public subnet and private subnet.<br>- Learn when NAT Gateway is needed and what cost factors may be generated. | 29/04/2026 | 29/04/2026 | https://000003.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Internet_Gateway.html<br>https://docs.aws.amazon.com/vpc/latest/userguide/vpc-nat-gateway.html |
| Thursday | - Learn about Security Group and Network ACL.<br>- Compare Security Group as a stateful mechanism and Network ACL as a stateless mechanism.<br>- Take notes on how to safely open inbound/outbound rules. | 30/04/2026 | 30/04/2026 | https://000003.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/vpc/latest/userguide/vpc-security-groups.html<br>https://docs.aws.amazon.com/vpc/latest/userguide/vpc-network-acls.html |
| Friday | - Learn about VPC Resource Map and how to check connectivity between components in a VPC.<br>- Summarize the steps to create a VPC, subnets, route tables, Internet Gateway, and Security Group.<br>- Write a basic network configuration checklist for a web application on AWS. | 01/05/2026 | 01/05/2026 | https://000003.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html |

### Lab implementation steps for Week 2:

* Open the VPC Console and select the correct practice Region, for example ap-southeast-1.
* Create a new VPC and define a suitable IPv4 CIDR block, for example 10.0.0.0/16.
* Create a public subnet and a private subnet, then assign each subnet to a suitable Availability Zone.
* Create an Internet Gateway, attach it to the VPC, and add a 0.0.0.0/0 route pointing to the Internet Gateway for the public route table.
* Create a NAT Gateway in the public subnet and configure the private route table to access the Internet through the NAT Gateway if needed.
* Create a Security Group for EC2/web server and only open required ports such as SSH, HTTP, or HTTPS.
* Learn about Network ACL, check inbound/outbound rules, and distinguish it from Security Group.
* Create an EC2 instance in a subnet to test network connectivity, then clean up unused resources to avoid unnecessary costs.

### Results achieved in Week 2:

* Understood that VPC is an isolated virtual network used to deploy AWS resources.
* Distinguished between public subnet and private subnet.
* Understood the role of Route Table in traffic routing.
* Understood how Security Group and Network ACL control network access.
* Able to describe the basic Internet connection flow inside a VPC.


---