---
title: "Worklog Week 2"
date: 2026-07-10
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---


### Week 2 Objectives:

* Understand Amazon VPC and basic networking components on AWS.
* Understand the roles of Subnet, Route Table, Internet Gateway, NAT Gateway, Security Group, and Network ACL.
* Know how to read a basic network model and identify connection flows in a VPC.

### Tasks to be carried out this week:

| Day | Task | Start date | Completion date | References |
| --- | --- | --- | --- | --- |
| 2 | - Studied the Amazon Virtual Private Cloud module.<br>- Learned the concepts of VPC, CIDR block, public subnet, and private subnet.<br>- Took notes on the role of VPC in isolating resources on AWS. | 27/04/2026 | 27/04/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://000003.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html <br> https://www.youtube.com/watch?v=O5CIvG0Wt78&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=28 |
| 3 | - Learned about Subnet and Route Table.<br>- Distinguished public subnet and private subnet based on the route to Internet Gateway.<br>- Redrew a simple VPC model with a public subnet and a private subnet. | 28/04/2026 | 28/04/2026 | https://000003.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/vpc/latest/userguide/configure-subnets.html |
| 4 | - Learned about Internet Gateway and NAT Gateway.<br>- Took notes on Internet access flows from public subnet and private subnet.<br>- Learned when NAT Gateway is needed and which factors may generate costs. | 29/04/2026 | 29/04/2026 | https://000003.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Internet_Gateway.html<br>https://docs.aws.amazon.com/vpc/latest/userguide/vpc-nat-gateway.html |
| 5 | - Learned about Security Group and Network ACL.<br>- Compared Security Group as stateful and Network ACL as stateless.<br>- Took notes on how to safely open inbound/outbound rules. | 30/04/2026 | 30/04/2026 | https://000003.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/vpc/latest/userguide/vpc-security-groups.html<br>https://docs.aws.amazon.com/vpc/latest/userguide/vpc-network-acls.html |
| 6 | - Learned about VPC Resource Map and how to check connections between components in a VPC.<br>- Summarized the steps to create VPC, subnet, route table, Internet Gateway, and Security Group.<br>- Recorded a basic network configuration checklist for a web application on AWS. | 01/05/2026 | 01/05/2026 | https://000003.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html |

### Lab implementation steps for week 2:

* Open VPC Console and select the correct practice Region, for example ap-southeast-1.
* Create a new VPC and define a suitable IPv4 CIDR block, for example 10.0.0.0/16.
* Create public and private subnets, and attach each subnet to an appropriate Availability Zone.
* Create an Internet Gateway, attach it to the VPC, and add a 0.0.0.0/0 route to the Internet Gateway in the public route table.
* Create a NAT Gateway in the public subnet and configure the private route table to access the Internet through the NAT Gateway if needed.
* Create a Security Group for an EC2/web server, opening only required ports such as SSH, HTTP, or HTTPS.
* Explore Network ACL, check inbound/outbound rules, and distinguish it from Security Group.
* Create an EC2 instance in a subnet to test network connectivity, then clean up unused resources to avoid costs.

### Results achieved in week 2:

* Understood that VPC is an isolated virtual network used to deploy AWS resources.
* Distinguished public subnet and private subnet.
* Understood the role of Route Table in traffic routing.
* Understood how Security Group and Network ACL control network access.
* Could describe a basic Internet connection flow inside a VPC.


---
