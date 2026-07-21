---
title: "Worklog Week 4"
date: 2026-07-10
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---


### Week 4 Objectives:

* Understand AWS storage services, focusing on Amazon S3.
* Know how to create an S3 Bucket, upload objects, configure access permissions, and enable Static Website Hosting.
* Understand basic concepts of bucket policy, object key, versioning, and storage class.

### Tasks to be carried out this week:

| Day | Task | Start date | Completion date | References |
| --- | --- | --- | --- | --- |
| 2 | - Studied the overview of storage services on AWS.<br>- Learned about Amazon S3, S3 Bucket, Object, Object Key, Region, and Storage Class. | 11/05/2026 | 11/05/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://000057.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html <br> https://www.youtube.com/watch?v=_yunukwcAwc&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=104 |
| 3 | - Learned how to create an S3 Bucket and upload objects.<br>- Learned about Block Public Access, Object Ownership, and object access permissions. | 12/05/2026 | 12/05/2026 | https://000057.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AmazonS3/latest/userguide/creating-bucket.html |
| 4 | - Learned about S3 Static Website Hosting.<br>- Took notes on index document, error document, and bucket website endpoint.<br>- Tried configuring a static website with a simple HTML file. | 13/05/2026 | 13/05/2026 | https://000057.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AmazonS3/latest/userguide/WebsiteHosting.html |
| 5 | - Learned about bucket policy and how to grant read access to objects for a static website.<br>- Learned about CORS in S3 and when CORS needs to be configured for a frontend. | 14/05/2026 | 14/05/2026 | https://000057.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AmazonS3/latest/userguide/example-bucket-policies.html<br>https://docs.aws.amazon.com/AmazonS3/latest/userguide/cors.html |
| 6 | - Learned about S3 Versioning, lifecycle, and several storage best practices.<br>- Summarized the steps to deploy a static website with S3.<br>- Took notes on common errors when accessing an S3 website. | 15/05/2026 | 15/05/2026 | https://000057.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AmazonS3/latest/userguide/Versioning.html<br>https://docs.aws.amazon.com/AmazonS3/latest/userguide/object-lifecycle-mgmt.html |

### Lab implementation steps for week 4:

* Open S3 Console, choose Create bucket, and set a globally unique bucket name.
* Choose an appropriate Region such as ap-southeast-1, then configure Object Ownership and Block Public Access according to the lab requirements.
* Upload static website files such as index.html, error.html, CSS, JavaScript, or images.
* In bucket Properties, enable Static website hosting and configure index document/error document.
* Create a bucket policy allowing public read object if the lab requires public website access.
* Check the website endpoint provided by S3 and test it in a browser.
* Enable Bucket Versioning to track object versions when files are uploaded again.
* Explore Lifecycle rules to transition or delete old objects if storage optimization is needed.
* Disable public access or delete the bucket after the lab if it is no longer used.

### Results achieved in week 4:

* Understood how S3 stores data as objects.
* Understood Bucket, Object, and Object Key structure.
* Understood the basic steps to enable Static Website Hosting.
* Understood how bucket policy and public access affect website accessibility.
* Knew that S3 can be used as a storage location for frontend files or uploaded files in the project.


---
